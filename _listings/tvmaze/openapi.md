---
swagger: "2.0"
x-collection-name: TVmaze
x-complete: 1
info:
  title: TVmaze user
  description: access-to-the-user-api-is-only-possible-for-users-with-a-premiumhttpwww-tvmaze-compremium-account--a-user-can-only-access-their-own-user-data-authentication-uses-http-basic--use-the-tvmaze-username-as-authentication-username-and-the-tvmaze-api-key-as-authentication-password--your-api-key-can-be-found-on-your-dashboardhttpwww-tvmaze-comdashboard--to-try-out-these-api-calls-from-this-page-click-the-authorize-button-on-top-and-input-your-credentials-
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
  /user/votes/episodes:
    get:
      summary: Get User Votes Episodes
      description: Get user votes episodes.
      operationId: getUserVotesEpisodes
      x-api-path-slug: uservotesepisodes-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Episodes
  /user/votes/episodes/{episode_id}:
    delete:
      summary: Delete User Votes Episodes
      description: Delete user votes episodes.
      operationId: deleteUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Episodes
    get:
      summary: Get User Votes Episodes
      description: Get user votes episodes.
      operationId: getUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Episodes
    parameters:
      summary: Parameters User Votes Episodes
      description: Parameters user votes episodes.
      operationId: parametersUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Votes
      - Episodes
    put:
      summary: Put User Votes Episodes
      description: Put user votes episodes.
      operationId: putUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-put
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
      - Votes
      - Episodes
---