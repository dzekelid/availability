swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Inventory/Availability/{sku}:
    get:
      summary: Get the availability of an item across all suppliers.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Inventory_GetAvailability
      x-api-path-slug: apiv1inventoryavailabilitysku-get
      parameters:
      - in: path
        name: sku
        description: Merchant SKU
      responses:
        200:
          description: OK
      tags:
      - Availability
      - Of
      - Item
      - Across
      - ""
      - Suppliers