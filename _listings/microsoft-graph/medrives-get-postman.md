{
  "info": {
    "name": "Microsoft Graph API List Available Drives",
    "_postman_id": "3a069abc-ce36-4fcf-aee3-723e6e008690",
    "description": "List available drives Retrieve the list of Drive resources available for a target User or Group. Your app can also request the set of document libraries on the SharePoint root site.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "fe3d44b6-f461-4f49-b120-6f626a288f36",
          "name": "ListAvailableDrives",
          "request": {
            "url": "http://graph.microsoft.com/me/drives",
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
              "id": "93b2228f-7802-4b5b-af00-d83a6ebc0660"
            }
          ]
        }
      ]
    }
  ]
}