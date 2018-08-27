---
swagger: "2.0"
x-collection-name: TradeStation
x-complete: 0
info:
  title: TradeStation Request Available Activation Triggers
  description: To place orders with activation triggers, a valid TriggerKey must be
    sent with the order.  This resource provides the available trigger methods with
    their corresponding key.
  termsOfService: http://elasticbeanstalk-us-east-1-525856068889.s3.amazonaws.com/wp-content/uploads/2014/03/Guidelines_For_Acceptance.pdf
  contact:
    name: TradeStation API Team
    url: https://developer.tradestation.com/webapi
    email: webapi@tradestation.com
  version: 1.0.0
host: api.tradestation.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orderexecution/activationtriggers:
    get:
      summary: Request Available Activation Triggers
      description: To place orders with activation triggers, a valid TriggerKey must
        be sent with the order.  This resource provides the available trigger methods
        with their corresponding key.
      operationId: getActivationTriggers
      x-api-path-slug: orderexecutionactivationtriggers-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      responses:
        200:
          description: Successful response
      tags:
      - Request
      - Available
      - Activation
      - Triggers
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