---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Update an item availability
  description: Updates an item availability.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/availabilities/{id}:
    get:
      summary: Get an item availability
      description: Gets an item availability. The ID of the availability must be specified.
      operationId: getRestAvailabilities
      x-api-path-slug: restavailabilitiesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Item
      - Availability
    put:
      summary: Update an item availability
      description: Updates an item availability.
      operationId: putRestAvailabilities
      x-api-path-slug: restavailabilitiesid-put
      parameters:
      - in: body
        name: /rest/availabilities/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Item
      - Availability
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