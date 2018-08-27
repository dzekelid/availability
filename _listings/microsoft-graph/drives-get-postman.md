{
  "info": {
    "name": "Microsoft Graph API List Available Drives",
    "_postman_id": "6121e8bd-36dc-41ad-baa8-10f6bed29e98",
    "description": "List available drives Retrieve the list of Drive resources available for a target User or Group. Your app can also request the set of document libraries on the SharePoint root site.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "d0a0bc4b-2197-450e-8762-4684f8c90f61",
          "name": "ListAvailableDrives",
          "request": {
            "url": "http://graph.microsoft.com/drives",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List available drives Retrieve the list of Drive resources available for a target User or Group"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "e575cedd-82ab-438b-94c9-21dc168f82bd"
            }
          ]
        }
      ]
    }
  ]
}