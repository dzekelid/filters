{
  "info": {
    "name": "AWS Simple Email Service API List Receipt Filters",
    "_postman_id": "f5d85aa9-1dd8-4669-9c7f-707fa8a0d7a0",
    "description": "Lists the IP address filters associated with your AWS account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "0f1ef523-6e1c-43d4-9b74-8cb95647caa3",
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
              "id": "bb5c33dc-7e7b-4fea-b10e-38d477c29eee"
            }
          ]
        },
        {
          "id": "a90be9c0-bfce-4d8d-b379-f499c5178bb3",
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
              "id": "bbd7ec1f-2a53-48f3-8043-607a48cb714c"
            }
          ]
        },
        {
          "id": "00dadcb9-10b9-4403-8e81-6011efdcb033",
          "name": "listReceiptFilters",
          "request": {
            "url": "http://example.com/api/?Action=ListReceiptFilters?Filters.member.N=Filters.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the IP address filters associated with your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2400d10-f2ce-4504-ac16-c88f4d894700"
            }
          ]
        }
      ]
    }
  ]
}