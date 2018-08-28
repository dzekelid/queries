swagger: "2.0"
x-collection-name: Botify
x-complete: 1
info:
  title: Botify
  description: botify-saas-api
  version: 1.0.0
host: api.botify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/suggested_filters:
    post:
      summary: Post Analyses Username Project Slug Analysis Slug Urls Suggested Filters
      description: Return most frequent segments (= suggested patterns in the previous
        version) for a Botify Query.
      operationId: postAnalysesUsernameProjectSlugAnalysisSlugUrlsSuggestedFilters
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlssuggested-filters-post
      parameters:
      - in: query
        name: area
        description: Analysis context
      - in: body
        name: UrlsAggsQuery
        description: UrlsAggs query
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Suggested
      - Filters