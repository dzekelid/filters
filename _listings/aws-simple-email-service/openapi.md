---
swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 1
info:
  title: AWS Simple Email Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateReceiptFilter:
    get:
      summary: Create Receipt Filter
      description: Creates a new IP address filter.
      operationId: createReceiptFilter
      x-api-path-slug: actioncreatereceiptfilter-get
      parameters:
      - in: query
        name: Filter
        description: A data structure that describes the IP address filter to create,
          which consists of a name, an IP address range, and whether to allow or block
          mail from it
        type: string
      responses:
        200:
          description: OK
      tags:
      - Receipt Filters
  /?Action=DeleteReceiptFilter:
    get:
      summary: Delete Receipt Filter
      description: Deletes the specified IP address filter.
      operationId: deleteReceiptFilter
      x-api-path-slug: actiondeletereceiptfilter-get
      parameters:
      - in: query
        name: FilterName
        description: The name of the IP address filter to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Receipt Filters
  /?Action=ListReceiptFilters:
    get:
      summary: List Receipt Filters
      description: Lists the IP address filters associated with your AWS account.
      operationId: listReceiptFilters
      x-api-path-slug: actionlistreceiptfilters-get
      parameters:
      - in: query
        name: Filters.member.N
        description: A list of IP address filter data structures, which each consist
          of a name, an IP address range, and whether to allow or block mail from
          it
        type: string
      responses:
        200:
          description: OK
      tags:
      - Receipt Filters
---