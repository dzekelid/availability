---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph List Available Drives
  description: List available drives Retrieve the list of Drive resources available
    for a target User or Group. Your app can also request the set of document libraries
    on the SharePoint root site.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /drives:
    get:
      summary: List Available Drives
      description: List available drives Retrieve the list of Drive resources available
        for a target User or Group. Your app can also request the set of document
        libraries on the SharePoint root site.
      operationId: ListAvailableDrives
      x-api-path-slug: drives-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Available
      - Drives
  /me/drives:
    get:
      summary: List Available Drives
      description: List available drives Retrieve the list of Drive resources available
        for a target User or Group. Your app can also request the set of document
        libraries on the SharePoint root site.
      operationId: ListAvailableDrives
      x-api-path-slug: medrives-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Available
      - Drives
  /groups/{id}/drives:
    get:
      summary: List Available Drives
      description: List available drives Retrieve the list of Drive resources available
        for a target User or Group. Your app can also request the set of document
        libraries on the SharePoint root site.
      operationId: ListAvailableDrives
      x-api-path-slug: groupsiddrives-get
      parameters:
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Available
      - Drives
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