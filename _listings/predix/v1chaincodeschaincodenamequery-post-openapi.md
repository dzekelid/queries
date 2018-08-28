---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix BlockChain Post Chaincodes Query
  description: Performs query operation on the chaincode and returns the result
  version: 1.0.0
host: predix-apphub-arcs-prod.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v2/config/orchestrations/defaulttagquery:
    get:
      summary: Get the default tag query corresponding for the tenant.
      description: Returns all information (query string, fieldnamespecifier, tagnamespecifer,
        description etc.) associated with the default tag query. An error is returned
        if tag query does not exist for the tenant.
      operationId: retrieveDefaultTagQuery
      x-api-path-slug: apiv2configorchestrationsdefaulttagquery-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Default
      - Tag
      - Query
      - Correspondingthe
      - Tenant
    post:
      summary: Create the default tag query corresponding for the tenant.
      description: Creates the default tag query including all information (query
        string, fieldnamespecifier, tagnamespecifer, description etc.) associated
        with the query.
      operationId: createDefaultTagQuery
      x-api-path-slug: apiv2configorchestrationsdefaulttagquery-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: tag names default query
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Default
      - Tag
      - Query
      - Correspondingthe
      - Tenant
  /v1/chaincodes/{chaincodeName}/query:
    post:
      summary: Post Chaincodes Query
      description: Performs query operation on the chaincode and returns the result
      operationId: performs-query-operation-on-the-chaincode-and-returns-the-result
      x-api-path-slug: v1chaincodeschaincodenamequery-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: chaincodeName
        description: chain code name
      - in: body
        name: payload
        description: payload of function and args
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: predix-zone-id
        description: tenantId
      responses:
        200:
          description: OK
      tags:
      - Chaincodes
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