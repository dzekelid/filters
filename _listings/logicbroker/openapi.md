swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Shipments:
    get:
      summary: Get shipments for given filters
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_SearchShipment
      x-api-path-slug: apiv1shipments-get
      parameters:
      - in: query
        name: Filters.advanced
        description: Advanced query options
      - in: query
        name: Filters.from
        description: Beginning of time search window
      - in: query
        name: Filters.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: Filters.page
        description: Page number
      - in: query
        name: Filters.pageSize
        description: Page size
      - in: query
        name: Filters.partnerPO
        description: The partners purchase order number
      - in: query
        name: Filters.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: Filters.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: Filters.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: Filters.status
        description: The status of the document
      - in: query
        name: Filters.to
        description: End of time search window
      responses:
        200:
          description: OK
      tags:
      - Shipmentsgiven
      - Filters
  /api/v1/Invoices:
    get:
      summary: Get invoices based on provided filters
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Invoice_SearchInvoice
      x-api-path-slug: apiv1invoices-get
      parameters:
      - in: query
        name: filters.advanced
        description: Advanced query options
      - in: query
        name: filters.from
        description: Beginning of time search window
      - in: query
        name: filters.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: filters.page
        description: Page number
      - in: query
        name: filters.pageSize
        description: Page size
      - in: query
        name: filters.partnerPO
        description: The partners purchase order number
      - in: query
        name: filters.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: filters.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: filters.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: filters.status
        description: The status of the document
      - in: query
        name: filters.to
        description: End of time search window
      responses:
        200:
          description: OK
      tags:
      - Invoices
      - Based
      - "On"
      - Provided
      - Filters
  /api/v1/Attachments:
    get:
      summary: Get a list of all attachments matching a given filter.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Attachment_GetList
      x-api-path-slug: apiv1attachments-get
      parameters:
      - in: query
        name: acknowledged
        description: Acknowledged flag
      - in: query
        name: logicbrokerKey
        description: Logicbroker key
      - in: query
        name: page
        description: Page number
      - in: query
        name: receiverId
        description: Receiver account number
      - in: query
        name: type
        description: Attachment type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Attachments
      - Matching
      - Given
      - Filter