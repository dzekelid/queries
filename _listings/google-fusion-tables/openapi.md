swagger: "2.0"
x-collection-name: Google Fusion Tables
x-complete: 1
info:
  title: Fusion Tables
  description: api-for-working-with-fusion-tables-data-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /fusiontables/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /query:
    get:
      summary: Execute SQL Statement
      description: "Executes a SQL statement which can be any of \n- SELECT\n- SHOW\n-
        DESCRIBE"
      operationId: fusiontables.query.sqlGet
      x-api-path-slug: query-get
      parameters:
      - in: query
        name: hdrs
        description: Whether column names are included (in the first row)
      - in: query
        name: sql
        description: A SQL statement which can be any of - SELECT- SHOW- DESCRIBE
      - in: query
        name: typed
        description: 'Whether typed values are returned in the (JSON) response: numbers
          for numeric values and parsed geometries for KML values'
      responses:
        200:
          description: OK
      tags:
      - Query
    post:
      summary: Execute Fusion Table SQL Statement
      description: "Executes a Fusion Tables SQL statement, which can be any of \n-
        SELECT\n- INSERT\n- UPDATE\n- DELETE\n- SHOW\n- DESCRIBE\n- CREATE statement."
      operationId: fusiontables.query.sql
      x-api-path-slug: query-post
      parameters:
      - in: query
        name: hdrs
        description: Whether column names are included in the first row
      - in: query
        name: sql
        description: A Fusion Tables SQL statement, which can be any of - SELECT-
          INSERT- UPDATE- DELETE- SHOW- DESCRIBE- CREATE
      - in: query
        name: typed
        description: 'Whether typed values are returned in the (JSON) response: numbers
          for numeric values and parsed geometries for KML values'
      responses:
        200:
          description: OK
      tags:
      - Query