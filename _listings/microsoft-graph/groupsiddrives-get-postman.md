{
  "info": {
    "name": "Microsoft Graph API List Available Drives",
    "_postman_id": "a50372c2-3129-4b4d-9725-f7a8d05ef8a9",
    "description": "List available drives Retrieve the list of Drive resources available for a target User or Group. Your app can also request the set of document libraries on the SharePoint root site.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "a80ce850-525c-41d1-9879-263d0e2357cc",
          "name": "ListAvailableDrives",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/drives"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
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
              "id": "9c97c73a-e902-4101-9d7d-6f92a2f789f8"
            }
          ]
        }
      ]
    }
  ]
}