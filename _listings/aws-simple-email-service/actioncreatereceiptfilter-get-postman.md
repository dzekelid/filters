{
  "info": {
    "name": "AWS Simple Email Service API Create Receipt Filter",
    "_postman_id": "79f1458c-5078-4d9c-8af9-7a5cbca314c3",
    "description": "Creates a new IP address filter.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "dc9f344e-a906-448b-82ea-4559e517a823",
          "name": "createReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptFilter?Filter=Filter",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a10038cd-3582-42ce-8762-457d7ff139d2"
            }
          ]
        }
      ]
    }
  ]
}