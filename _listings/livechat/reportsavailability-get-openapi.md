---
swagger: "2.0"
x-collection-name: LiveChat
x-complete: 0
info:
  title: LiveChat Availability
  description: Shows how long an agent (or a group or the whole account) was available
    for chatting during a specified period. When querying for one day, the results
    are shown in minutes per every hour, otherwise in hours for each day.
  version: 1.0.0
host: api.livechatinc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/availability:
    get:
      summary: Availability
      description: Shows how long an agent (or a group or the whole account) was available
        for chatting during a specified period. When querying for one day, the results
        are shown in minutes per every hour, otherwise in hours for each day.
      operationId: ReportsAvailabilityGet
      x-api-path-slug: reportsavailability-get
      parameters:
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - Availability
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