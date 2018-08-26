---
swagger: "2.0"
x-collection-name: BBC
x-complete: 0
info:
  title: BBC Nitro Get raw formats
  description: Get raw formats
  termsOfService: http://www.bbc.co.uk/terms/
  contact:
    name: Open Nitro Project
    url: http://developer.bbc.co.uk/
    email: nitro@bbc.co.uk
  version: 1.0.0
host: programmes.api.bbc.com
basePath: /nitro/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/episodes/{pid}:
    get:
      summary: Get raw episode
      description: Get raw episode
      operationId: Get_Raw_episode
      x-api-path-slug: v1episodespid-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Episodes
      - Pid
  /v1/episodes/{pid}/ancestors/:
    get:
      summary: Get raw ancestors
      description: Get raw ancestors
      operationId: Get_Raw_ancestors
      x-api-path-slug: v1episodespidancestors-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Episodes
      - Pid
      - Ancestors
  /v1/episodes/{pid}/formats/:
    get:
      summary: Get raw formats
      description: Get raw formats
      operationId: Get_Raw_formats
      x-api-path-slug: v1episodespidformats-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Episodes
      - Pid
      - Formats
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