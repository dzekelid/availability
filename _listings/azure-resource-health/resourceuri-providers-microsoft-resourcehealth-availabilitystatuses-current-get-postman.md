{
  "info": {
    "name": "Azure Resource Health API Availability Statuses Get By Resource",
    "_postman_id": "133b40ad-9d00-482a-b1ce-33b3af334727",
    "description": "Gets current availability status for a single resource",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "availability statuses resource",
      "item": [
        {
          "id": "b676fbf1-ffa5-4d9a-ad83-b4cb6c80146b",
          "name": "AvailabilityStatuses_GetByResource",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                ":resourceUri/providers/Microsoft.ResourceHealth/availabilityStatuses/current"
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
                  "id": "resourceUri",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets current availability status for a single resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8b5abdc-3021-4b03-b5b3-2c064e3e13a6"
            }
          ]
        }
      ]
    }
  ]
}