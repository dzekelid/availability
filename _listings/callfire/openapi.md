swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /keywords/{keyword}/available:
    get:
      summary: Check for a specific keyword
      description: Searches for the specific keyword to purchase on the CallFire platform.
        Returns 'true' if keyword is available.
      operationId: isKeywordAvailable
      x-api-path-slug: keywordskeywordavailable-get
      parameters:
      - in: path
        name: keyword
        description: To specify a keyword to search for
      responses:
        200:
          description: OK
      tags:
      - Keywords
      - Keyword
      - Available