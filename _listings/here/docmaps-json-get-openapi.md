---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Route Match Extension API Map Data Availability and Freshness
  description: |-
    *Request the release date and area covered by each available map region*

    To make a request for release date information, use the `maps.json` endpoint.



    * **app_id**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

    * **app_code**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
  version: 1.0.0
host: pde.cit.api.here.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /doc/maps.json:
    get:
      summary: Map Data Availability and Freshness
      description: |-
        *Request the release date and area covered by each available map region*

        To make a request for release date information, use the `maps.json` endpoint.



        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
      operationId: DocMapsJsonGet
      x-api-path-slug: docmaps-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      responses:
        200:
          description: OK
      tags:
      - Map
      - Data
      - Availability
      - Freshness
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