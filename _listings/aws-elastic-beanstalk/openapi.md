---
swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 1
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
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
---