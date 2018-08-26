---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeAvailablePatches:
    get:
      summary: Describe Available Patches
      description: Lists all patches that could possibly be included in a patch baseline.
      operationId: describeAvailablePatches
      x-api-path-slug: actiondescribeavailablepatches-get
      parameters:
      - in: query
        name: Filters
        description: Filters used to scope down the returned patches
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patches to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Available
      - Patches
---