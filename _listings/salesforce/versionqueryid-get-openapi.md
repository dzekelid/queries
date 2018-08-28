---
swagger: "2.0"
x-collection-name: Salesforce
x-complete: 0
info:
  title: Salesforce Sandbox Get Version Query
  description: 'Retrieves the remaining SOQL query results using the identifier within
    the field "nextRecordsUrl" value (i.e. "nextRecordsUrl" : "/services/data/v24.0/query/01gD0000002HU6KIAW-2000")
    located at the end of the initial query results. Requests the next batch of records
    and you could repeat (using the corresponding identifier) until all records have
    been retrieved.'
  version: 1.0.0
host: na14.salesforce.com
basePath: /services/data/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{version}/query:
    get:
      summary: Get Version Query
      description: Executes the specified SOQL query. If the initial query returns
        only part of the results, the end of the response will contain a field called
        nextRecordsUrl. In such cases, use the resource {version}/query/{id} to request
        the next batch of records and repeat until all records have been retrieved.
      operationId: getVersionQuery
      x-api-path-slug: versionquery-get
      parameters:
      - in: query
        name: q
        description: A SOQL query
      - in: path
        name: version
        description: An API version
      responses:
        200:
          description: OK
      tags:
      - Version
      - Query
  /{version}/query/{id}:
    get:
      summary: Get Version Query
      description: 'Retrieves the remaining SOQL query results using the identifier
        within the field "nextRecordsUrl" value (i.e. "nextRecordsUrl" : "/services/data/v24.0/query/01gD0000002HU6KIAW-2000")
        located at the end of the initial query results. Requests the next batch of
        records and you could repeat (using the corresponding identifier) until all
        records have been retrieved.'
      operationId: getVersionQuery
      x-api-path-slug: versionqueryid-get
      parameters:
      - in: path
        name: id
        description: An identifier used to retrieve the remaining results
      - in: path
        name: version
        description: An API version
      responses:
        200:
          description: OK
      tags:
      - Version
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