---
swagger: "2.0"
x-collection-name: Datadog
x-complete: 0
info:
  title: DataDog API Get Query
  version: 1.0.0
  description: This end point allows you to query for metrics from any time period.
basePath: api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /query:
    get:
      summary: Get Query
      description: This end point allows you to query for metrics from any time period.
      operationId: getQuery
      x-api-path-slug: query-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
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