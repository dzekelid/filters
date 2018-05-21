{
  "info": {
    "name": "AWS Simple Email Service API Delete Receipt Filter",
    "_postman_id": "e05b6758-61be-4116-aa41-e9d1ab898a74",
    "description": "Deletes the specified IP address filter.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "27c301e5-3dc7-4e07-b8c1-2ac6426beeb1",
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
              "id": "925809e0-770e-4382-bfce-33bb4c274394"
            }
          ]
        },
        {
          "id": "87f6c2ce-3a6e-4e07-a3fd-08caf6c27b56",
          "name": "deleteReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptFilter?FilterName=FilterName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69ca7967-af1e-40d8-8d69-6dba422e0274"
            }
          ]
        }
      ]
    }
  ]
}