{
  "info": {
    "name": "Azure Resource Health API Availability Statuses List By Resource Group",
    "_postman_id": "ccd58495-3b3b-42bb-b380-aae1cc50d394",
    "description": "Lists the current availability status for all the resources in the resource group. Use the nextLink property in the response to get the next page of availability statuses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "availability statuses resource group",
      "item": [
        {
          "id": "e29b2ebf-ebb8-4ca2-acee-9fcfb26fb45d",
          "name": "AvailabilityStatuses_ListByResourceGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ResourceHealth/availabilityStatuses"
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
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the current availability status for all the resources in the resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3825191a-cd74-48a5-bd05-3c68f3079999"
            }
          ]
        }
      ]
    }
  ]
}