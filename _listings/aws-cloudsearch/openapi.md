swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 1
info:
  title: AWS CloudSearch
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeAvailabilityOptions:
    get:
      summary: Describe Availability Options
      description: Gets the availability options configured for a domain.
      operationId: DescribeAvailabilityOptions
      x-api-path-slug: actiondescribeavailabilityoptions-get
      parameters:
      - in: query
        name: Deployed
        description: Whether to display the deployed configuration (true) or include
          any pending changes (false)
        type: string
      - in: query
        name: DomainName
        description: The name of the domain you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Availability Options
  /?Action=UpdateAvailabilityOptions:
    get:
      summary: Update Availability Options
      description: Configures the availability options for a domain.
      operationId: UpdateAvailabilityOptions
      x-api-path-slug: actionupdateavailabilityoptions-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: MultiAZ
        description: You expand an existing search domain to a second Availability
          Zone by setting the Multi-AZ option to true
        type: string
      responses:
        200:
          description: OK
      tags:
      - Availability Options