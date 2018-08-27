---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Route Match Extension API Available Map Data Layers
  description: |-
    *Request which data layers can be accessed within a specified map region and release*

    To make a request for data layer availability information, use the `layers.json` endpoint, supplying the `release` and `region` parameters.



    * **region**  `text`
     \- Map Coverage Region.    e.g. `APAC`, `NA`, `EU`

    * **release**  `text`
     \- Map release quarter    e.g. `2014Q4` or `LATEST`

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
  /doc/layers.json:
    get:
      summary: Available Map Data Layers
      description: |-
        *Request which data layers can be accessed within a specified map region and release*

        To make a request for data layer availability information, use the `layers.json` endpoint, supplying the `release` and `region` parameters.



        * **region**  `text`
         \- Map Coverage Region.    e.g. `APAC`, `NA`, `EU`

        * **release**  `text`
         \- Map release quarter    e.g. `2014Q4` or `LATEST`

        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
      operationId: DocLayersJsonGet
      x-api-path-slug: doclayers-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: region
      - in: query
        name: release
      responses:
        200:
          description: OK
      tags:
      - Available
      - Map
      - Data
      - Layers
  /doc/attributes.json:
    get:
      summary: Available Attributes
      description: "*Request which map data layers contain which attributes*\n\nTo
        make a request for map data layer information, use the `attributes``.json`
        endpoint, supplying the `release` and `region` parameters.\n  \n\n\n\n* **region**
        \ `text`\n \\- Map Coverage Region.    e.g. `APAC`, `NA`, `EU`\n\n* **release**
        \ `text`\n \\- Map release quarter    e.g. `2014Q4` or `LATEST`\n\n* **app_id**
        \ `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication
        of the client application.    You must include an `app_id` with every request.\n\n*
        **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for
        the authentication of the client application.    You must include an `app_code`
        with every request."
      operationId: DocAttributesJsonGet
      x-api-path-slug: docattributes-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: region
      - in: query
        name: release
      responses:
        200:
          description: OK
      tags:
      - Available
      - Attributes
  /doc/layer.json:
    get:
      summary: Available Attributes within a Map Data Layer
      description: |-
        *Request which attributes are available within a specified map data layer*

        To make a request for map data layer information, use the `layer``.json` endpoint, supplying the `release`, `layer` and `region` parameters.



        * **region**  `text`
         \- Map Coverage Region.    e.g. `APAC`, `NA`, `EU`

        * **release**  `text`
         \- Map release quarter    e.g. `2014Q4` or `LATEST`

        * **layer**  `text`
         \- Thematic layer

        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
      operationId: DocLayerJsonGet
      x-api-path-slug: doclayer-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: layer
      - in: query
        name: region
      - in: query
        name: release
      responses:
        200:
          description: OK
      tags:
      - Available
      - Attributes
      - Within
      - Map
      - Data
      - Layer
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