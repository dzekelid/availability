---
swagger: "2.0"
info:
  title: Relay API
  description: Use these API to manage Azure Relay resources through Azure Resources
    Manager.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.Relay/CheckNameAvailability:
    post:
      summary: Namespaces Check Name Availability
      description: Check the give namespace name availability
      operationId: Namespaces_CheckNameAvailability
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters to check availability of the given namespace name
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - namespaces name availability
definitions:
  TrackedResource:
    properties:
      location:
        description: This is a default description.
        type: post
      tags:
        description: This is a default description.
        type: post
  Resource:
    properties:
      id:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  HybridConnectionListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  HybridConnection:
    properties: []
  HybridConnectionProperties:
    properties:
      createdAt:
        description: This is a default description.
        type: post
      updatedAt:
        description: This is a default description.
        type: post
      listenerCount:
        description: This is a default description.
        type: post
      requiresClientAuthorization:
        description: This is a default description.
        type: post
      userMetadata:
        description: This is a default description.
        type: post
  WcfRelaysListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  WcfRelay:
    properties: []
  WcfRelayProperties:
    properties:
      relayType:
        description: This is a default description.
        type: post
      createdAt:
        description: This is a default description.
        type: post
      updatedAt:
        description: This is a default description.
        type: post
      listenerCount:
        description: This is a default description.
        type: post
      requiresClientAuthorization:
        description: This is a default description.
        type: post
      requiresTransportSecurity:
        description: This is a default description.
        type: post
      isDynamic:
        description: This is a default description.
        type: post
      userMetadata:
        description: This is a default description.
        type: post
  RelayNamespaceListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  RelayNamespace:
    properties: []
  RelayNamespaceProperties:
    properties:
      provisioningState:
        description: This is a default description.
        type: post
      createdAt:
        description: This is a default description.
        type: post
      updatedAt:
        description: This is a default description.
        type: post
      serviceBusEndpoint:
        description: This is a default description.
        type: post
      metricId:
        description: This is a default description.
        type: post
  Sku:
    properties:
      name:
        description: This is a default description.
        type: post
      tier:
        description: This is a default description.
        type: post
  AuthorizationRuleListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  AuthorizationRule:
    properties: []
  AuthorizationRuleProperties:
    properties:
      rights:
        description: This is a default description.
        type: post
  AuthorizationRuleKeys:
    properties:
      primaryConnectionString:
        description: This is a default description.
        type: post
      secondaryConnectionString:
        description: This is a default description.
        type: post
      primaryKey:
        description: This is a default description.
        type: post
      secondaryKey:
        description: This is a default description.
        type: post
      keyName:
        description: This is a default description.
        type: post
  RegenerateKeysParameters:
    properties:
      policyKey:
        description: This is a default description.
        type: post
  ErrorResponse:
    properties:
      code:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  CheckNameAvailability:
    properties:
      name:
        description: This is a default description.
        type: post
  CheckNameAvailabilityResult:
    properties:
      nameAvailable:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  RelayNamespaceUpdateParameter:
    properties:
      tags:
        description: This is a default description.
        type: post
  OperationListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  Operation:
    properties:
      name:
        description: This is a default description.
        type: post
x-collection-name: Azure Relay
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