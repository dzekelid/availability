---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 0
info:
  title: Entertainment Express Get GoWatchIt Episode Availability.
  description: Returns GoWatchit episode availability by Entertainment Episode ID.
    Special permission is required to access this endpoint.
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GoWatchIt/Episodes/{Id}/Availabilities:
    get:
      summary: Get GoWatchIt Episode Availability.
      description: Returns GoWatchit episode availability by Entertainment Episode
        ID. Special permission is required to access this endpoint.
      operationId: GetGoWatchItEpisodeAvailabilities
      x-api-path-slug: gowatchitepisodesidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Episode
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Episodes
      - Id
      - Availabilities
  /GoWatchIt/Movies/{Id}/Availabilities:
    get:
      summary: Get GoWatchIt Movie Availability.
      description: Returns GoWatchIt movie availability by Entertainment Movie ID.  Special
        permission is required to access this endpoint.  Contact [Sales](mailto:Sales@InternetVideoArchive.com)
        for more information.
      operationId: GetGoWatchItMovieAvailabilities
      x-api-path-slug: gowatchitmoviesidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Movie
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Movies
      - Id
      - Availabilities
  /GoWatchIt/Seasons/{Id}/Availabilities:
    get:
      summary: Get GoWatchIt Season Availability.
      description: Returns GoWatchIt season availability by Entertainment Season ID.  Special
        permission is required to access this endpoint.  Contact [Sales](mailto:Sales@InternetVideoArchive.com)
        for more information.
      operationId: GetGoWatchItSeasonAvailabilities
      x-api-path-slug: gowatchitseasonsidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Season
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Seasons
      - Id
      - Availabilities
  /GoWatchIt/Shows/{Id}/Availabilities:
    get:
      summary: Get GoWatchItShow Availability.
      description: Returns GoWatchIt show availability by Entertainment Show ID.  Special
        permission is required to access this endpoint. Please contact [Sales](mailto:Sales@InternetVideoArchive.com)
        for more information.
      operationId: GetGoWatchItShowAvailabilities
      x-api-path-slug: gowatchitshowsidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Show
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Shows
      - Id
      - Availabilities
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