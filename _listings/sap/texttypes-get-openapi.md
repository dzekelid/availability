---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Translation Hub Returns a list of the text types available in SAP Translation
    Hub.
  description: In SAP products, short texts, such as those used on user interfaces
    (UIs), are characterized by various text types. The type of a specific text is
    determined by the UI element that it describes. For example,  button texts are
    described by the text type ```XBUT```. <br> The text type resource returns a list
    of the text types that are available in SAP Translation Hub. You can combine the
    '/text type' resource with the '/suggestion' resource to narrow down the results
    of the suggestion resource.
  contact:
    name: SAP Translation Hub team
    email: translationhub@sap.com
  version: 1.0.0
host: sandbox.api.sap.com
basePath: /translationhub/api/v1
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
  /texttypes:
    get:
      summary: Returns a list of the text types available in SAP Translation Hub.
      description: In SAP products, short texts, such as those used on user interfaces
        (UIs), are characterized by various text types. The type of a specific text
        is determined by the UI element that it describes. For example,  button texts
        are described by the text type ```XBUT```. <br> The text type resource returns
        a list of the text types that are available in SAP Translation Hub. You can
        combine the '/text type' resource with the '/suggestion' resource to narrow
        down the results of the suggestion resource.
      operationId: in-sap-products-short-texts-such-as-those-used-on-user-interfaces-uis-are-characterized-by-various-t
      x-api-path-slug: texttypes-get
      parameters:
      - in: header
        name: Content-Type
        description: Specifies the nature of the data in the body so that the receiving
          agent can process the data accordingly
      - in: query
        name: search
        description: Allows you to search for a specific text type, such as message
      responses:
        200:
          description: Successful response
      tags:
      - Returns
      - List
      - Of
      - Text
      - Types
      - Available
      - In
      - SAP
      - Translation
      - Hub
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