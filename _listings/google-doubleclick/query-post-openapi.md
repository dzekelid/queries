---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Create Query
  version: 1.0.0
  description: Creates a query.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /queries:
    get:
      summary: Get Stored Queries
      description: Retrieves stored queries.
      operationId: doubleclickbidmanager.queries.listqueries
      x-api-path-slug: queries-get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Query
  /queries/{queryId}/reports:
    get:
      summary: Get Stored Reports
      description: Retrieves stored reports.
      operationId: doubleclickbidmanager.reports.listreports
      x-api-path-slug: queriesqueryidreports-get
      parameters:
      - in: path
        name: queryId
        description: Query ID with which the reports are associated
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Query
  /query:
    post:
      summary: Create Query
      description: Creates a query.
      operationId: doubleclickbidmanager.queries.createquery
      x-api-path-slug: query-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Query
  /query/{queryId}:
    delete:
      summary: Delete Stored Query
      description: Deletes a stored query as well as the associated stored reports.
      operationId: doubleclickbidmanager.queries.deletequery
      x-api-path-slug: queryqueryid-delete
      parameters:
      - in: path
        name: queryId
        description: Query ID to delete
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Query
    get:
      summary: Get Stored Query
      description: Retrieves a stored query.
      operationId: doubleclickbidmanager.queries.getquery
      x-api-path-slug: queryqueryid-get
      parameters:
      - in: path
        name: queryId
        description: Query ID to retrieve
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Query
    post:
      summary: Run Stored Query
      description: Runs a stored query to generate a report.
      operationId: doubleclickbidmanager.queries.runquery
      x-api-path-slug: queryqueryid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: queryId
        description: Query ID to run
      responses:
        200:
          description: OK
      tags:
      - Advertising
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