---
swagger: "2.0"
x-collection-name: SYNQ Video
x-complete: 0
info:
  title: SYNQ Video Perform a JavaScript query to return video objects matching any
    desired criteria.
  description: Find videos matching any criteria, by running a JavaScript function
    over each video object. A detailed tutorial on how to use this functionality is
    available on the [documentation page](https://www.synq.fm/queries-video-api/).
  version: 1.9.1
host: api.synq.fm
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /video/query:
    post:
      summary: Perform a JavaScript query to return video objects matching any desired
        criteria.
      description: Find videos matching any criteria, by running a JavaScript function
        over each video object. A detailed tutorial on how to use this functionality
        is available on the [documentation page](https://www.synq.fm/queries-video-api/).
      operationId: query
      x-api-path-slug: videoquery-post
      parameters:
      - in: formData
        name: api_key
      - in: formData
        name: filter
        description: JavaScript code to be run over each video object, to determine
          what should be returend
      responses:
        200:
          description: OK
      tags:
      - Video
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