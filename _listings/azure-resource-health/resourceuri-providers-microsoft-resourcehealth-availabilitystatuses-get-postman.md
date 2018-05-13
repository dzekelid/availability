{
  "info": {
    "name": "Azure Resource Health API Availability Statuses List",
    "_postman_id": "c2330732-39e0-41a7-b82d-57498fc732e6",
    "description": "Lists the historical availability statuses for a single resource. Use the nextLink property in the response to get the next page of availability status",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "availability statuses",
      "item": [
        {
          "id": "20601e58-bcc0-4695-a98d-e5a28008668a",
          "name": "AvailabilityStatuses_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                ":resourceUri/providers/Microsoft.ResourceHealth/availabilityStatuses"
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
            "description": "Lists the historical availability statuses for a single resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34d638ab-5697-4ff3-a32d-6f245558a68b"
            }
          ]
        }
      ]
    }
  ]
}