---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Get Available Fax Cover Pages
  description: "Returns fax cover pages available for the current extension.\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [page] value is invalid\n\n\n401\nCMN-405\nLogin
    to extension required"
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/dictionary/fax-cover-page:
    get:
      summary: Get Available Fax Cover Pages
      description: "Returns fax cover pages available for the current extension.\nUsage
        Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [page] value is invalid\n\n\n401\nCMN-405\nLogin
        to extension required"
      operationId: listFaxCoverPages
      x-api-path-slug: restapiv1-0dictionaryfaxcoverpage-get
      parameters:
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Available
      - Fax
      - Cover
      - Pages
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