---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 1
info:
  title: Entertainment Express
  description: your-gateway-to-building-incredible-movie-tv-and-game-content-discovery-experiences-
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Changes/Episodes/History/:
    get:
      summary: Returns list of unique EpisodeId changes greater than or equal to date
        (UTC)
      description: For each updated episode ID, pull the full episode data for that
        ID and update.
      operationId: GetEpisodeChangeHistory
      x-api-path-slug: changesepisodeshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Episodes
      - History
  /Changes/Episodes/HistoryWithEntity/:
    get:
      summary: Returns list of unique EpisodeId and Entity changes greater than or
        equal to date (UTC).
      description: Lists each episode ID that has changed as well as the entity in
        the object that changed.
      operationId: GetEpisodeChangeHistoryWithEntity
      x-api-path-slug: changesepisodeshistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Episodes
      - HistoryWithEntity
  /GoWatchIt/Episodes/{Id}/Availabilities:
    get:
      summary: Get GoWatchIt Episode Availability.
      description: Returns GoWatchit episode availability by Entertainment Episode
        ID. Special permission is required to access this endpoint.
      operationId: GetGoWatchItEpisodeAvailabilities
      x-api-path-slug: gowatchitepisodesidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Episode
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Episodes
      - Id
      - Availabilities
  /Shows/Seasons/Episodes/{Id}:
    get:
      summary: Returns an Episode object for a requested Episode ID.
      description: Returns the episode details for a specific episode ID.
      operationId: GetEpisode
      x-api-path-slug: showsseasonsepisodesid-get
      parameters:
      - in: path
        name: Id
        description: Required ID of an Episode
      - in: query
        name: Includes
        description: List of additional objects to include in the episode response
      responses:
        200:
          description: OK
      tags:
      - Shows
      - Seasons
      - Episodes
      - Id
  /Shows/{Id}/Seasons/{SeasonNumber}/Episodes/{EpisodeNumber}:
    get:
      summary: Get Episode by ShowId, Season Number and Episode Number.
      description: Requires a valid ShowId, Season Number and Episode Number.
      operationId: GetEpisodeByEpisodeNumber
      x-api-path-slug: showsidseasonsseasonnumberepisodesepisodenumber-get
      parameters:
      - in: path
        name: EpisodeNumber
        description: Required EpisodeNumber
      - in: path
        name: Id
        description: Required Id of the Show
      - in: query
        name: Includes
        description: List of additional objects to include in the episode response
      - in: path
        name: SeasonNumber
        description: Required SeasonNumber
      responses:
        200:
          description: OK
      tags:
      - Shows
      - Id
      - Seasons
      - SeasonNumber
      - Episodes
      - EpisodeNumber
  /Shows/Seasons/Episode/:
    get:
      summary: Get Episode by ShowId, Season Number and Episode Number.
      description: Some use cases find it useful to be able to pass a season number
        and episode number of a known show to get the data for that exact episode.
      operationId: GetEpisodeByNumber
      x-api-path-slug: showsseasonsepisode-get
      parameters:
      - in: query
        name: EpisodeNumber
        description: Required EpisodeNumber
      - in: query
        name: Id
        description: Required Id of the Show
      - in: query
        name: SeasonNumber
        description: Required SeasonNumber
      responses:
        200:
          description: OK
      tags:
      - Shows
      - Seasons
      - Episode
---