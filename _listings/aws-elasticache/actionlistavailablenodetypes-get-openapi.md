---
swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 0
info:
  title: Amazon ElastiCache API List Available Node Types
  version: 1.0.0
  description: .
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListAvailableNodeTypes:
    get:
      summary: List Available Node Types
      description: .
      operationId: listAvailableNodeTypes
      x-api-path-slug: actionlistavailablenodetypes-get
      parameters:
      - in: query
        name: AvailableNodeTypes.member.N
        description: 'Type: array of AvailableNodeType objects'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Node Types
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