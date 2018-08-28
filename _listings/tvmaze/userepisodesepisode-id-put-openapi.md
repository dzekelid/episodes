---
swagger: "2.0"
x-collection-name: TVmaze
x-complete: 0
info:
  title: TVmaze user Put User Episodes
  description: Set `marked_at` to `NULL` or leave it out to use the current time.
  version: "1.0"
host: api.tvmaze.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/episodes:
    get:
      summary: Get User Episodes
      description: Get user episodes.
      operationId: getUserEpisodes
      x-api-path-slug: userepisodes-get
      parameters:
      - in: query
        name: show_id
        description: Only return episodes from this specific show
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Episodes
  /user/episodes/{episode_id}:
    delete:
      summary: Delete User Episodes
      description: Delete user episodes.
      operationId: deleteUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Episodes
    get:
      summary: Get User Episodes
      description: Get user episodes.
      operationId: getUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Episodes
    parameters:
      summary: Parameters User Episodes
      description: Parameters user episodes.
      operationId: parametersUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Episodes
    put:
      summary: Put User Episodes
      description: Set `marked_at` to `NULL` or leave it out to use the current time.
      operationId: putUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Episodes
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