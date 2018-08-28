swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 1
info:
  title: Transport for London Unified
  description: our-unified-api-brings-together-data-across-all-modes-of-transport-into-a-single-restful-api--this-api-provides-access-to-the-most-highly-requested-realtime-and-status-infomation-across-all-the-modes-of-transport-in-a-single-and-consistent-way--access-to-the-developer-documentation-is-available-at-httpsapi-tfl-gov-uk
  version: v1
host: api.tfl.gov.uk
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Line/Search/{query}:
    get:
      summary: Line  Search query
      description: Search for lines or routes matching the query string.
      operationId: Line_Search
      x-api-path-slug: linesearchquery-get
      parameters:
      - in: query
        name: modes
        description: Optionally filter by the specified modes
      - in: path
        name: query
        description: Search term e
      - in: query
        name: serviceTypes
        description: A comma seperated list of service types to filter on
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Search
      - Query
  /StopPoint/Search/{query}:
    get:
      summary: Stop Point  Search query
      description: Search stoppoints by their common name, or their 5-digit countdown
        bus stop code..
      operationId: StopPoint.Search.query.get
      x-api-path-slug: stoppointsearchquery-get
      parameters:
      - in: query
        name: faresOnly
        description: True to only return stations in that have Fares data available
          for single fares to another station
      - in: query
        name: includeHubs
        description: If true, returns results including HUBs
      - in: query
        name: lines
        description: An optional, parameter separated list of the lines to filter
          by
      - in: query
        name: maxResults
        description: An optional result limit, defaulting to and with a maximum of
          50
      - in: query
        name: modes
        description: An optional, parameter separated list of the modes to filter
          by
      - in: path
        name: query
        description: The query string, case-insensitive
      - in: query
        name: tflOperatedNationalRailStationsOnly
        description: If the national-rail mode is included, this flag will filter
          the national rail stations so that only those operated by TfL are returned
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Search
      - Query