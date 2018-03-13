---
swagger: "2.0"
info:
  title: ServiceBusManagementClient
  description: Azure Service Bus client
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
  /subscriptions/{subscriptionId}/providers/Microsoft.ServiceBus/CheckNameAvailability:
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
        type: get
      tags:
        description: This is a default description.
        type: get
  Resource:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  NamespaceCreateOrUpdateParameters:
    properties:
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  NamespaceListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  NamespaceResource:
    properties: []
  NamespaceProperties:
    properties:
      provisioningState:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      createdAt:
        description: This is a default description.
        type: get
      updatedAt:
        description: This is a default description.
        type: get
      serviceBusEndpoint:
        description: This is a default description.
        type: get
      createACSNamespace:
        description: This is a default description.
        type: get
      enabled:
        description: This is a default description.
        type: get
  NamespaceUpdateParameters:
    properties:
      tags:
        description: This is a default description.
        type: get
  Sku:
    properties:
      name:
        description: This is a default description.
        type: get
      tier:
        description: This is a default description.
        type: get
      capacity:
        description: This is a default description.
        type: get
  SharedAccessAuthorizationRuleCreateOrUpdateParameters:
    properties:
      location:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  SharedAccessAuthorizationRuleListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  SharedAccessAuthorizationRuleResource:
    properties: []
  SharedAccessAuthorizationRuleProperties:
    properties:
      rights:
        description: This is a default description.
        type: get
  ResourceListKeys:
    properties:
      primaryConnectionString:
        description: This is a default description.
        type: get
      secondaryConnectionString:
        description: This is a default description.
        type: get
      primaryKey:
        description: This is a default description.
        type: get
      secondaryKey:
        description: This is a default description.
        type: get
      keyName:
        description: This is a default description.
        type: get
  RegenerateKeysParameters:
    properties:
      Policykey:
        description: This is a default description.
        type: get
  QueueCreateOrUpdateParameters:
    properties:
      name:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
  QueueListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  QueueResource:
    properties: []
  QueueProperties:
    properties:
      lockDuration:
        description: This is a default description.
        type: get
      accessedAt:
        description: This is a default description.
        type: get
      autoDeleteOnIdle:
        description: This is a default description.
        type: get
      createdAt:
        description: This is a default description.
        type: get
      defaultMessageTimeToLive:
        description: This is a default description.
        type: get
      duplicateDetectionHistoryTimeWindow:
        description: This is a default description.
        type: get
      enableBatchedOperations:
        description: This is a default description.
        type: get
      deadLetteringOnMessageExpiration:
        description: This is a default description.
        type: get
      enableExpress:
        description: This is a default description.
        type: get
      enablePartitioning:
        description: This is a default description.
        type: get
  MessageCountDetails:
    properties:
      activeMessageCount:
        description: This is a default description.
        type: get
      deadLetterMessageCount:
        description: This is a default description.
        type: get
      scheduledMessageCount:
        description: This is a default description.
        type: get
      transferDeadLetterMessageCount:
        description: This is a default description.
        type: get
      transferMessageCount:
        description: This is a default description.
        type: get
  TopicCreateOrUpdateParameters:
    properties:
      name:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
  TopicListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  TopicResource:
    properties: []
  TopicProperties:
    properties:
      accessedAt:
        description: This is a default description.
        type: get
      autoDeleteOnIdle:
        description: This is a default description.
        type: get
      createdAt:
        description: This is a default description.
        type: get
      defaultMessageTimeToLive:
        description: This is a default description.
        type: get
      duplicateDetectionHistoryTimeWindow:
        description: This is a default description.
        type: get
      enableBatchedOperations:
        description: This is a default description.
        type: get
      enableExpress:
        description: This is a default description.
        type: get
      enablePartitioning:
        description: This is a default description.
        type: get
      enableSubscriptionPartitioning:
        description: This is a default description.
        type: get
      filteringMessagesBeforePublishing:
        description: This is a default description.
        type: get
  SubscriptionCreateOrUpdateParameters:
    properties:
      location:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  SubscriptionListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  SubscriptionResource:
    properties: []
  SubscriptionProperties:
    properties:
      accessedAt:
        description: This is a default description.
        type: get
      autoDeleteOnIdle:
        description: This is a default description.
        type: get
      createdAt:
        description: This is a default description.
        type: get
      defaultMessageTimeToLive:
        description: This is a default description.
        type: get
      deadLetteringOnFilterEvaluationExceptions:
        description: This is a default description.
        type: get
      deadLetteringOnMessageExpiration:
        description: This is a default description.
        type: get
      enableBatchedOperations:
        description: This is a default description.
        type: get
      isReadOnly:
        description: This is a default description.
        type: get
      lockDuration:
        description: This is a default description.
        type: get
      maxDeliveryCount:
        description: This is a default description.
        type: get
  CheckNameAvailability:
    properties:
      name:
        description: This is a default description.
        type: get
  CheckNameAvailabilityResult:
    properties:
      nameAvailable:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  OperationListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  Operation:
    properties:
      name:
        description: This is a default description.
        type: get
x-collection-name: Azure Service Bus
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