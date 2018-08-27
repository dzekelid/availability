---
swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 0
info:
  title: AWS Elastic Beanstalk API List Available Solution Stacks
  version: 1.0.0
  description: Returns a list of the available solution stack names.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CheckDNSAvailability:
    get:
      summary: Check D N S Availability
      description: Checks if the specified CNAME is available.
      operationId: checkDNSAvailability
      x-api-path-slug: actioncheckdnsavailability-get
      parameters:
      - in: query
        name: CNAMEPrefix
        description: The prefix used when this CNAME is reserved
        type: string
      responses:
        200:
          description: OK
      tags:
      - DNS
  /?Action=ListAvailableSolutionStacks:
    get:
      summary: List Available Solution Stacks
      description: Returns a list of the available solution stack names.
      operationId: listAvailableSolutionStacks
      x-api-path-slug: actionlistavailablesolutionstacks-get
      parameters:
      - in: query
        name: SolutionStackDetails.member.N
        description: A list of available solution stacks and their SolutionStackDescription
        type: string
      - in: query
        name: SolutionStacks.member.N
        description: A list of available solution stacks
        type: string
      responses:
        200:
          description: OK
      tags:
      - Solution Stacks
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