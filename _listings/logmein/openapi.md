swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 1
info:
  title: GoToWebinar API
  description: todo-add-description
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    get:
      summary: Get Tickets
      description: "Retrieves a query-able set of tickets for a specific partner system.\n\n
        \                                                        \nRequest Parameters\n
        \                         \n    field      data type      description    \n
        \   userToken      string      The token identifying and authenticating the
        user in the partner system that this object is being created on behalf of
        this user.    \n\n\nQuery Parameters (* Optional)\n\n    field      data type
        \     description    \n    q *      string      A query string used to search
        for objects in the partner system. (It is up to the partner system to determine
        how the query string is matched. Match against fields like: ticket title,
        ticket body, requester name, ticket ID, ticket comments, tags, etc. Ideally
        the matching should be performed using a \u2018contains\u2019 type operation
        and in a case-insensitive way.)                                         \n
        \   limit *      integer      The maximum number of records to be fetched.
        Default value is 10. Suggested value is less than or equal to 10 for optimal
        performance.                                         \n    offset *      number
        \     Zero based offset for the first record to return. Default value is 0."
      operationId: UnnammedEndpointGet
      x-api-path-slug: get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: q
      - in: query
        name: userToken
      responses:
        200:
          description: OK
      tags:
      - Tickets