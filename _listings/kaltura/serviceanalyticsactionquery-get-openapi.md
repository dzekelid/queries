---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Analytics Action Query
  description: report query action allows to get a analytics data for specific query
    dimensions, metrics and filters.
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/analytics/action/query:
    get:
      summary: Get Service Analytics Action Query
      description: report query action allows to get a analytics data for specific
        query dimensions, metrics and filters.
      operationId: analytics.query
      x-api-path-slug: serviceanalyticsactionquery-get
      parameters:
      - in: query
        name: filter[dimensions]
        description: Comma separated dimensions list
      - in: query
        name: filter[filters]
      - in: query
        name: filter[from_time]
        description: Query start time (in local time) MM/dd/yyyy HH:mi
      - in: query
        name: filter[metrics]
        description: Comma separated metrics list
      - in: query
        name: filter[orderBy]
        description: Query order by metric/dimension
      - in: query
        name: filter[to_time]
        description: Query end time (in local time) MM/dd/yyyy HH:mi
      - in: query
        name: filter[utcOffset]
        description: Timezone offset from UTC (in minutes)
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Analytics
      - Action
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