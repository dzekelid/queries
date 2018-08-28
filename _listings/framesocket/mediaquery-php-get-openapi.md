---
swagger: "2.0"
x-collection-name: Framesocket
x-complete: 0
info:
  title: Framesocket Query Media
  description: Query Media
  version: 1.0.0
host: www.framesocket.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media/query.php:
    get:
      summary: Query Media
      description: Query Media
      operationId: getMediaQuery.php
      x-api-path-slug: mediaquery-php-get
      parameters:
      - in: query
        name: andkeywords
        description: Comma separated list of title words
      - in: query
        name: andtitlewords
        description: Comma separated list of title words
      - in: query
        name: customid
        description: Custom ID
      - in: query
        name: hash
        description: Media Hash Code
      - in: query
        name: key
        description: Your account username
      - in: query
        name: limit
        description: Must be a valid integer
      - in: query
        name: orkeywords
        description: Comma separated list of title words
      - in: query
        name: ortitlewords
        description: Comma separated list of title words
      - in: query
        name: secret
        description: Your account API secret
      - in: query
        name: sig
        description: This is an md5 hash of your gatekeeper concatenated with your
          request action
      - in: query
        name: sort
        description: Must be a valid sorting option, either newest or oldest firs
      - in: query
        name: status
        description: Must be a valid status code
      - in: query
        name: type
        description: Must be a valid type, either image or video
      responses:
        200:
          description: OK
      tags:
      - Media
      - Query
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