{
  "info": {
    "name": "Pay Run.IO Get a list of all available data object tempaltes",
    "_postman_id": "588fbaad-5975-413c-8114-149f4e667b2f",
    "description": "Returns a collection of links to all the available data object templates",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "195b8b5b-3224-4450-81be-3edb653719bd",
          "name": "GetTemplates",
          "request": {
            "url": "http://api.test.payrun.io/Templates",
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of links to all the available data object templates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e714fc16-58e6-47db-b9c8-df01d6306fec"
            }
          ]
        }
      ]
    }
  ]
}