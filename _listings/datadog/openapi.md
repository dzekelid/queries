swagger: "2.0"
x-collection-name: Datadog
x-complete: 1
info:
  title: DataDog Merged API
  version: 1.0.0
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