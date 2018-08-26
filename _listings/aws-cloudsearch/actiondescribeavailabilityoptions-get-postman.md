{
  "info": {
    "name": "AWS CloudSearch Describe Availability Options",
    "_postman_id": "b04591f3-a51b-46bc-b7e4-4582fab8dac7",
    "description": "Gets the availability options configured for a domain.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Availability Options",
      "item": [
        {
          "id": "4af48b1d-9c5e-480f-953c-4091b0fe6d67",
          "name": "DescribeAvailabilityOptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAvailabilityOptions?Deployed=Deployed&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the availability options configured for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba9924ec-4bb7-4bec-968b-c149119b96cd"
            }
          ]
        }
      ]
    }
  ]
}