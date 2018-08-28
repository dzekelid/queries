swagger: "2.0"
x-collection-name: Framesocket
x-complete: 1
info:
  title: Framesocket
  description: framesocket-is-the-best-way-for-developers-and-content-owners-to-tackle-video-projects-of-any-size-
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