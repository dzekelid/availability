---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Auto-picks attendees and the next available appointment slot given
    the parameters in the request.
  version: 1.0.0
  description: Auto-picks attendees and the next available appointment slot given
    the parameters in the request..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/appointment/suggest:
    post:
      summary: Auto-picks attendees and the next available appointment slot given
        the parameters in the request.
      description: Auto-picks attendees and the next available appointment slot given
        the parameters in the request..
      operationId: Appointment_SuggestAppointmentSlotByrequest
      x-api-path-slug: apiappointmentsuggest-post
      parameters:
      - in: body
        name: request
        description: An appointment suggest request containing information about the
          desired appointment
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Auto-picks
      - Attendees
      - Next
      - Available
      - Appointment
      - Slot
      - Given
      - Parameters
      - In
      - Request
  /api/dashboard/available:
    get:
      summary: Get all available dashboards
      description: Get all available dashboards.
      operationId: Dashboard_AvailableDashboards
      x-api-path-slug: apidashboardavailable-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Available
      - Dashboards
  /api/tenantreferncing/products:
    get:
      summary: Gets the available products for tenant referencing
      description: Gets the available products for tenant referencing.
      operationId: TenantReferencing_GetProducts
      x-api-path-slug: apitenantreferncingproducts-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Available
      - Productstenant
      - Referencing
  /api/workflow/triggers:
    get:
      summary: Lists the available triggers that are able to start workflows.
      description: Lists the available triggers that are able to start workflows..
      operationId: Workflow_GetTriggerTypes
      x-api-path-slug: apiworkflowtriggers-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Available
      - Triggers
      - That
      - Are
      - Able
      - To
      - Start
      - Workflows
  /api/workflow/listWorkflows:
    get:
      summary: Lists available workflows
      description: Lists available workflows.
      operationId: Workflow_ListWorkflowsByskipBytake
      x-api-path-slug: apiworkflowlistworkflows-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: skip
        description: Used for paging results
      - in: query
        name: take
        description: Used for paging results
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Available
      - Workflows
  /api/admin/system/CreateNewSystemFeature:
    post:
      summary: Creates a new system wide feature available for activation.
      description: Creates a new system wide feature available for activation..
      operationId: System_CreateNewSystemFeatureBysaveNewFeatureCommad
      x-api-path-slug: apiadminsystemcreatenewsystemfeature-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: saveNewFeatureCommad
        description: The save new feature commad
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - System
      - Wide
      - Feature
      - Availableactivation
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