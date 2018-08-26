---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
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
---