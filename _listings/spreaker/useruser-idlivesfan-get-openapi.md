---
swagger: "2.0"
x-collection-name: Spreaker
x-complete: 0
info:
  title: Spreaker API Get Favorite Live Episodes
  version: v1
  description: ""
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /episodes/live:
    get:
      summary: Get Live Episodes
      description: Retrieves all live episodes at the moment of the request
      operationId: getEpisodesLive
      x-api-path-slug: episodeslive-get
      parameters:
      - in: query
        name: show_id
        description: An list of show_id applied as a filter
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Live
      - Episodes
  /lives/top:
    get:
      summary: Get Top Live Episodes
      description: Retrieves live episodes sorted by rank
      operationId: getLivesTop
      x-api-path-slug: livestop-get
      parameters:
      - in: query
        name: I
        description: The rank is language - based
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Top
      - Live
      - Episodes
  /search/{query}:
    get:
      summary: Search users, shows and episodes
      description: Search users, shows and episodes
      operationId: getSearchQuery
      x-api-path-slug: searchquery-get
      parameters:
      - in: path
        name: query
        description: Search query
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Search
      - Users
      - ""
      - Shows
      - Episodes
  /show/{show_id}/episodes:
    get:
      summary: Get Show Episodes
      description: Retrieves all listenable episodes by show (both live and podcast,
        ordered by published_at DESC).
      operationId: getShowShowEpisodes
      x-api-path-slug: showshow-idepisodes-get
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Show
      - Episodes
  /show/{show_id}/episodes/all:
    get:
      summary: Get All Show Episodes
      description: Retrieves all episodes by show (both live and podcast, ordered
        by published_at DESC).
      operationId: getShowShowEpisodesAll
      x-api-path-slug: showshow-idepisodesall-get
      parameters:
      - in: path
        name: show_id
        description: The unique show id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Show
      - Episodes
  /user/{user_id}/episodes:
    get:
      summary: Get User Episodes
      description: Retrieves all listenable episodes by user (both live and podcast,
        ordered by published_at DESC).
      operationId: getUserUserEpisodes
      x-api-path-slug: useruser-idepisodes-get
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - User
      - Episodes
  /user/{user_id}/lives/fan:
    get:
      summary: Get Favorite Live Episodes
      description: ""
      operationId: getUserUserLivesFan
      x-api-path-slug: useruser-idlivesfan-get
      parameters:
      - in: path
        name: /user/{user_id}/lives/fan
        description: Users id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Favorite
      - Live
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