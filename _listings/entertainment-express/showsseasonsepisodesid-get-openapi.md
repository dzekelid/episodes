---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 0
info:
  title: Entertainment Express Returns an Episode object for a requested Episode ID.
  description: Returns the episode details for a specific episode ID.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---