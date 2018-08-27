swagger: "2.0"
x-collection-name: PayRun
x-complete: 1
info:
  title: Pay Run.IO
  description: open-scableable-transparent-payroll-api-
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