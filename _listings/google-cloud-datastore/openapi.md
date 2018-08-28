swagger: "2.0"
x-collection-name: Google Cloud Datastore
x-complete: 1
info:
  title: Google Cloud Datastore
  description: accesses-the-schemaless-nosql-database-to-provide-fully-managed-robust-scalable-storage-for-your-application-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: datastore.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}:runQuery:
    post:
      summary: Queries for Entities
      description: Queries for entities.
      operationId: datastore.projects.runQuery
      x-api-path-slug: v1projectsprojectidrunquery-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The ID of the project against which to make the request
      responses:
        200:
          description: OK
      tags:
      - Query