---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Get a list of all available schemas
  description: Returns a collection of links to all the available data object schemas
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Schemas:
    get:
      summary: Get a list of all available schemas
      description: Returns a collection of links to all the available data object
        schemas
      operationId: GetSchemas
      x-api-path-slug: schemas-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Available
      - Schemas
  /Templates:
    get:
      summary: Get a list of all available data object tempaltes
      description: Returns a collection of links to all the available data object
        templates
      operationId: GetTemplates
      x-api-path-slug: templates-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Available
      - Data
      - Object
      - Tempaltes
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---