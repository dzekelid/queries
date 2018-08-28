---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Put Members Savedsearches Savedsearch Query
  description: Put members savedsearches savedsearch query.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /members/{idMember}/savedSearches/{idSavedSearch}/query:
    put:
      summary: Put Members Savedsearches Savedsearch Query
      description: Put members savedsearches savedsearch query.
      operationId: updateMembersSavedSearchesQueryByIdMemberByIdSavedSearch
      x-api-path-slug: membersidmembersavedsearchesidsavedsearchquery-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Saved Searches Query to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: path
        name: idSavedSearch
        description: idSavedSearch
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Savedsearches
      - Savedsearch
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