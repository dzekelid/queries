---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Views Queries tags of Card.
  version: 1.0.0
  description: Queries tags of card..
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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
  /v1/datapoints:
    get:
      summary: Query Datapoints
      description: "Both the GET and POST methods can be used to query time series
        data. Use the query API with the GET HTTP method by passing the query JSON
        as a URL query parameter. The advantage of using the GET method is that requests
        and responses can be cached in proxy servers and browsers.  In cases where
        the query JSON is very long and exceeds query parameter length (for some browsers),
        use POST as a convenience method to query the time series API. POST requests
        have no restrictions on data length, however, requests are never cached. The
        Time Series service API is designed this way to support complex, nested time
        series queries on one or more tags and their attributes, with start and end
        times, along with aggregations and filters.Response JSON (Status 200)\n{\n\t\"tags\":
        [{\n\t\t\"name\": \"ALT_SENSOR\",\n\t\t\"results\": [{\n\t\t\t\"filters\":
        {\n\t\t\t\t\"attributes\": {\n\t\t\t\t\t\"host\": [\n\t\t\t\t\t\t\"test\"\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"measurements\":
        {\n\t\t\t\t\t\"condition\": \"le\",\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t36\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"qualities\":
        {\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t\"3\"\n\t\t\t\t\t]\n\t\t\t\t}\n\t\t\t},\n\t\t\t\"attributes\":
        {\n\t\t\t\t\"host\": [\"test\"]\n\t\t\t},\n\t\t\t\"values\": [\n\t\t\t\t[1449709894000,
        5, 3],\n\t\t\t\t[1449709895000, 7, 3]\n\t\t\t]\n\t\t}],\n\t\t\"stats\": {\n\t\t\t\"rawCount\":
        2\n\t\t}\n\t}]\n}"
      operationId: query
      x-api-path-slug: v1datapoints-get
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Content-Type
      - in: header
        name: Predix-Zone-Id
      - in: query
        name: query
        description: Valid JSON string
      responses:
        200:
          description: Successful response
      tags:
      - Query
      - Datapoints
    post:
      summary: Query Datapoints
      description: "Both the GET and POST methods can be used to query time series
        data. Use the query API with the GET HTTP method by passing the query JSON
        as a URL query parameter. The advantage of using the GET method is that requests
        and responses can be cached in proxy servers and browsers.  In cases where
        the query JSON is very long and exceeds query parameter length (for some browsers),
        use POST as a convenience method to query the time series API. POST requests
        have no restrictions on data length, however, requests are never cached. The
        Time Series service API is designed this way to support complex, nested time
        series queries on one or more tags and their attributes, with start and end
        times, along with aggregations and filters.  Following is a sample request
        message: Request JSON{\n\t\"start\": \"24h-ago\",\n\t\"end\": \"12h-ago\",\n\t\"tags\":
        [{\n\t\t\"name\": \"ALT_SENSOR\",\n\t\t\"limit\": 1000,\n\t\t\"order\": \"desc\",\n\t\t\"suppressGroupByType\":
        true|false,\n\t\t\"aggregations\": [{\n\t\t\t\"type\": \"avg\",\n\t\t\t\"interval\":
        \"1h\"\n\t\t}],\n\t\t\"filters\": {\n\t\t\t\"attributes\": {\n\t\t\t\t\"host\":
        [\n\t\t\t\t\t\"test\"\n\t\t\t\t]\n\t\t\t},\n\t\t\t\"measurements\": {\n\t\t\t\t\"condition\":
        \"le\",\n\t\t\t\t\"values\": [\n\t\t\t\t\t\"36\"\n\t\t\t\t]\n\t\t\t},\n\t\t\t\"qualities\":
        {\n\t\t\t\t\"values\": [\n\t\t\t\t\t\"3\"\n\t\t\t\t]\n\t\t\t}\n\t\t},\n\t\t\"groups\":
        [{\n\t\t\t\"name\": \"attribute\",\n\t\t\t\"attributes\": [\n\t\t\t\t\"host\",
        \"subtenant\"\n\t\t\t]\n\t\t}]\n\t}]\n}\nResponse JSON (Status 200){\n\t\"tags\":
        [{\n\t\t\"name\": \"ALT_SENSOR\",\n\t\t\"results\": [{\n\t\t\t\"filters\":
        {\n\t\t\t\t\"attributes\": {\n\t\t\t\t\t\"host\": [\n\t\t\t\t\t\t\"test\"\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"measurements\":
        {\n\t\t\t\t\t\"condition\": \"le\",\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t36\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"qualities\":
        {\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t\"3\"\n\t\t\t\t\t]\n\t\t\t\t}\n\t\t\t},\n\t\t\t\"attributes\":
        {\n\t\t\t\t\"host\": [\"test\"]\n\t\t\t},\n\t\t\t\"values\": [\n\t\t\t\t[1449709894000,
        5, 3],\n\t\t\t\t[1449709895000, 7, 3]\n\t\t\t]\n\t\t}],\n\t\t\"stats\": {\n\t\t\t\"rawCount\":
        2\n\t\t}\n\t}]\n}"
      operationId: get
      x-api-path-slug: v1datapoints-post
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Content-Type
      - in: header
        name: Predix-Zone-Id
      - in: body
        name: Query Request JSON
        description: Query Request (JSON)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Query
      - Datapoints
  /v1/collections/{collectionName}/assets/{assetId}/query:
    post:
      summary: Return locations for an asset by query condition for given customer
        id and collection name.
      description: |-
        Returns the locations for an asset by three types of query for a given customer id and collection name.
        The returned locations are in descending order of time.
        Three types of query:
        1. type=latest: The latest n locations will be returned.
        2. type=timeperiod: Locations within a time period will be returned.
        3. type=bbox: Locations within a time period and a spatial bounding box will be returned.
      operationId: returns-the-locations-for-an-asset-by-three-types-of-query-for-a-given-customer-id-and-collection-na
      x-api-path-slug: v1collectionscollectionnameassetsassetidquery-post
      parameters:
      - in: body
        name: body
        description: The parameters for the query for asset locations
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Return
      - Locationsan
      - Asset
      - By
      - Query
      - Conditiongiven
      - Customer
      - Id
      - Collection
      - Name
  /v1/query/queryByObject:
    post:
      summary: Query by Object
      description: Query image by object.
      operationId: dozicheck
      x-api-path-slug: v1queryquerybyobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: formData
        name: checkResultDisplayNumber
        description: 'Result display number: Specify number of verification result
          to retrieve'
      - in: formData
        name: idSpecificationFlag
        description: 'ID specification flag (0: Query with all registered objects
          , 1: Query with specified object by individual ID)'
      - in: formData
        name: individualId
        description: 'Individual ID: Use CSV form when specifying multiple IDs'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: queryImage
        description: 'Query image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Query
      - By
      - Object
  /v1/query/queryByGroup:
    post:
      summary: Query by Group
      description: Query image per group.
      operationId: groupzicheck
      x-api-path-slug: v1queryquerybygroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: formData
        name: checkResultDisplayNumber
        description: 'Result display number: Specify number of verification result
          to retrieve'
      - in: formData
        name: groupId
        description: 'Group ID: Use CSV form when specifying multiple IDs'
      - in: formData
        name: idSpecificationFlag
        description: 'ID specification flag(0: Query with all registered objects ,
          1: Query with specified object by groupId)'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: queryImage
        description: 'Query image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Query
      - By
      - Group
  /decks/{id}/cards:
    get:
      summary: Queries cards of Deck.
      description: Queries cards of deck..
      operationId: getDecksCards
      x-api-path-slug: decksidcards-get
      parameters:
      - in: query
        name: filter
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Queries
      - Cards
      - Of
      - Deck
  /decks/{id}/tags:
    get:
      summary: Queries tags of Deck.
      description: Queries tags of deck..
      operationId: getDecksTags
      x-api-path-slug: decksidtags-get
      parameters:
      - in: query
        name: filter
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Queries
      - Tags
      - Of
      - Deck
  /cards/{id}/tags:
    get:
      summary: Queries tags of Card.
      description: Queries tags of card..
      operationId: getCardsTags
      x-api-path-slug: cardsidtags-get
      parameters:
      - in: query
        name: filter
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Queries
      - Tags
      - Of
      - Card
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