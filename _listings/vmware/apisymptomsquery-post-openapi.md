---
swagger: "2.0"
x-collection-name: VMWare
x-complete: 0
info:
  title: VMWare vRealize Operations Query Symptoms
  description: 'TODO: Add Description'
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/alerts/query:
    post:
      summary: Query Alerts
      description: 'TODO: Add Description'
      operationId: ApiAlertsQueryPost
      x-api-path-slug: apialertsquery-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Query
  /api/resources/query:
    post:
      summary: Get Resources
      description: 'TODO: Add Description'
      operationId: ApiResourcesQueryPost
      x-api-path-slug: apiresourcesquery-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Query
  /api/symptoms/query:
    post:
      summary: Query Symptoms
      description: 'TODO: Add Description'
      operationId: ApiSymptomsQueryPost
      x-api-path-slug: apisymptomsquery-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Symptoms
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