---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Customer APIs Retrieves organizations available
    for collaboration
  description: "Retrieves organizations in a specific business role that are available
    for collaboration.  \nThese organizations may have been approved for or blocked
    from collaboration, or they're still pending for approval.\nThe login user must
    be from a customer."
  version: 1.0.0
host: hostname
basePath: /dim/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collaborationTemplates:
    get:
      summary: Retrieves available collaboration room templates
      description: Retrieves available collaboration room templates.
      operationId: retrieves-available-collaboration-room-templates
      x-api-path-slug: collaborationtemplates-get
      parameters:
      - in: query
        name: typeId
        description: The ID of a collaboration room template
      - in: query
        name: typeName
        description: The name of a collaboration room template
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Available
      - Collaboration
      - Room
      - Templates
  /organizations/visible:
    get:
      summary: Retrieves organizations available for collaboration
      description: "Retrieves organizations in a specific business role that are available
        for collaboration.  \nThese organizations may have been approved for or blocked
        from collaboration, or they're still pending for approval.\nThe login user
        must be from a customer."
      operationId: retrieves-organizations-in-a-specific-business-role-that-are-available-for-collaboration--these-orga
      x-api-path-slug: organizationsvisible-get
      parameters:
      - in: query
        name: activeServices
        description: The types of service that a supplier provides
      - in: query
        name: approved
        description: Specify approved=true to restrict the search to organizations
          that are approved for collaboration
      - in: query
        name: roleCode
        description: The code for the business role of the organizations
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Organizations
      - Availablecollaboration
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