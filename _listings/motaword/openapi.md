---
swagger: "2.0"
x-collection-name: MotaWord
x-complete: 1
info:
  title: Mota Word
  description: use-motaword-api-to-post-and-track-your-translation-projects-
  version: alpha-0.1.0
host: api.motaword.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    get:
      summary: Available endpoints
      description: The root endpoint will provide you a JSON Swagger definition.
      operationId: getEndpoints
      x-api-path-slug: get
      responses:
        200:
          description: OK
      tags:
      - ""
---