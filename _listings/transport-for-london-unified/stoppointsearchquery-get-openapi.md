---
swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 0
info:
  title: Transport for London Unified Stop Point  Search query
  description: Search stoppoints by their common name, or their 5-digit countdown
    bus stop code..
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