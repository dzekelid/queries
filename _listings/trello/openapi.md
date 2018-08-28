swagger: "2.0"
x-collection-name: Trello
x-complete: 1
info:
  title: Trello
  description: this-document-describes-the-rest-api-of-trello-as-published-by-trello-com---a-hrefhttpstrello-comdocsindex-html-target-blankofficial-documentationa--a-hrefhttpstrello-comdocsapi-target-blankthe-html-pages-that-were-scraped-in-order-to-generate-this-specification-a
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