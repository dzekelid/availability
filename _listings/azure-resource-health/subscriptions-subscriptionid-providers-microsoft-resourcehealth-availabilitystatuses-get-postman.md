{
  "info": {
    "name": "Azure Resource Health API Availability Statuses List By Subscription Id",
    "_postman_id": "10acab3f-27ad-4adf-930c-2df49be557eb",
    "description": "Lists the current availability status for all the resources in the subscription. Use the nextLink property in the response to get the next page of availability statuses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "availability statuses subscription id",
      "item": [
        {
          "id": "1f2fcb0f-d14c-4b0c-845a-b1d8a543f972",
          "name": "AvailabilityStatuses_ListBySubscriptionId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.ResourceHealth/availabilityStatuses"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the current availability status for all the resources in the subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9a6f743-ce47-4b40-9892-45d188bbc251"
            }
          ]
        }
      ]
    }
  ]
}