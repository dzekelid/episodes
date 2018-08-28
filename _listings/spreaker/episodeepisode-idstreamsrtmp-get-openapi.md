---
swagger: "2.0"
x-collection-name: Spreaker
x-complete: 0
info:
  title: Spreaker API Get Episode Streams
  version: v1
  description: The response contains a collection of RTMP / RTMPT streams.
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
  /episode/<episode_id>/image:
    put:
      summary: Change Episode Image
      description: Change Episode Image
      operationId: putEpisode<episode>Image
      x-api-path-slug: episodeepisode-idimage-put
      parameters:
      - in: path
        name: episode_id
        description: The unique episode id
      - in: query
        name: image_id
        description: The id of the image to set to the episode
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Change
      - Episode
      - Image
  /episode/{episode_id}:
    delete:
      summary: Delete Episode
      description: Deletes an episode. Theres no way to recover a deleted episode.
      operationId: deleteEpisodeEpisode
      x-api-path-slug: episodeepisode-id-delete
      parameters:
      - in: path
        name: episode_id
        description: The unique episode id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
    get:
      summary: Get Episode
      description: Retrieves an episode by unique identifier.
      operationId: getEpisodeEpisode
      x-api-path-slug: episodeepisode-id-get
      parameters:
      - in: path
        name: episode_id
        description: The episode unique id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
    put:
      summary: Edit Episode
      description: Edit episode info (eg. title, description, category, tags, ...)
      operationId: putEpisodeEpisode
      x-api-path-slug: episodeepisode-id-put
      parameters:
      - in: query
        name: category_id
        description: Episode category
      - in: query
        name: description
        description: Episode description, max length 10k chars
      - in: path
        name: episode_id
        description: the episode id
      - in: query
        name: tags
        description: Episode tags (comma separated)
      - in: query
        name: title
        description: Episode title, max length 40 chars
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Edit
      - Episode
  /episode/{episode_id}/media:
    get:
      summary: Get Episode Media List
      description: Get Episode Media List
      operationId: getEpisodeEpisodeMedia
      x-api-path-slug: episodeepisode-idmedia-get
      parameters:
      - in: path
        name: episode_id
        description: Unique id of episode
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
      - Media
      - List
  /episode/{episode_id}/streams/icy:
    get:
      summary: Get Episode Streams
      description: The response contains a collection of ICY streams.
      operationId: getEpisodeEpisodeStreamsIcy
      x-api-path-slug: episodeepisode-idstreamsicy-get
      parameters:
      - in: query
        name: episode_id
        description: The episode id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
      - Streams
  /episode/{episode_id}/streams/rtmp:
    get:
      summary: Get Episode Streams
      description: The response contains a collection of RTMP / RTMPT streams.
      operationId: getEpisodeEpisodeStreamsRtmp
      x-api-path-slug: episodeepisode-idstreamsrtmp-get
      parameters:
      - in: path
        name: episode_id
        description: The episode id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
      - Streams
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