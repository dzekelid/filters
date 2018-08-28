swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/tickets:
    get:
      summary: List tickets by filters
      description: List tickets by filters.
      operationId: getRestTickets
      x-api-path-slug: resttickets-get
      parameters:
      - in: query
        name: confidential
        description: Filter that restricts the search result to tickets of a specific
          confidential value
      - in: query
        name: contactId
        description: Filter that restricts the search result to tickets with a specified
          contact ID
      - in: query
        name: customerClassId
        description: Filter that restricts the search result to tickets with a specified
          customer class ID
      - in: query
        name: deadlineAt
        description: Filter that restricts the search result to tickets with a specified
          deadline
      - in: query
        name: fulltext
        description: Filter that restricts the search result to tickets with full-text
          search
      - in: query
        name: id
        description: Filter that restricts the search result to tickets of a specific
          ticket ID
      - in: query
        name: ownerId
        description: Filter that restricts the search result to tickets with a specified
          owner ID
      - in: query
        name: parentTicketId
        description: Filter that restricts the search result to tickets with a specified
          parent ticket ID
      - in: query
        name: plentyId
        description: Filter that restricts the search result to tickets with a specified
          client (store) ID
      - in: query
        name: priorityId
        description: Filter that restricts the search result to tickets of a specific
          ticket priority ID
      - in: query
        name: progress
        description: Filter that restricts the search result to tickets with a specified
          progress in percent
      - in: query
        name: resubmissionAt
        description: Filter that restricts the search result to tickets with a specified
          resubmission date
      - in: query
        name: roleId
        description: Filter that restricts the search result to tickets with a specified
          role ID
      - in: query
        name: source
        description: Filter that restricts the search result to tickets with a specific
          source value
      - in: query
        name: statusGroupId
        description: Filter that restricts the search result to tickets with a specified
          status group ID
      - in: query
        name: statusId
        description: Filter that restricts the search result to tickets with a specified
          status ID
      - in: query
        name: title
        description: Filter that restricts the search result to tickets with a specified
          phrase in title
      - in: query
        name: typeId
        description: Filter that restricts the search result to tickets of specific
          ticket types
      responses:
        200:
          description: OK
      tags:
      - List
      - Tickets
      - By
      - Filters
  /rest/orders:
    get:
      summary: List orders by filter options
      description: List orders by filter options.
      operationId: getRestOrders
      x-api-path-slug: restorders-get
      parameters:
      - in: query
        name: clientId
        description: Filter that restricts the search result to order from one client
      - in: query
        name: contactId
        description: Filter that restricts the search result to orders of one order
          contact
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to orders that were created
          on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to orders that were created
          within a certain period of time
      - in: query
        name: externalOrderId
        description: Filter that restricts the search result to an external order
          id
      - in: query
        name: hasDocument
        description: Filter that restricts the search result to orders which hold
          the given document type
      - in: query
        name: includedItem
        description: Filter that restricts the search result to orders with a certain
          item
      - in: query
        name: includedVariation
        description: Filter that restricts the search result to orders with a certain
          variation
      - in: query
        name: isEbayPlus
        description: Filter that restricts the search result to orders with ebay plus
      - in: query
        name: itemsPerPage
        description: The number of orders to be displayed per page
      - in: query
        name: orderIds
        description: Filter that restricts the search result to orders
      - in: query
        name: orderType
        description: Filter that restricts the search result to orders of specific
          order types
      - in: query
        name: outgoingItemsBookedAtFrom
        description: Filter that restricts the search result to orders where the outgoing
          items were booked on the specified date
      - in: query
        name: outgoingItemsBookedAtTo
        description: Filter that restricts the search result to orders where the outgoing
          items were booked within a specified period of time
      - in: query
        name: ownerUserId
        description: Filter that restricts the search result to orders of one owner
      - in: query
        name: page
        description: The page to get
      - in: query
        name: paidAtFrom
        description: Filter that restricts the search result to orders that received
          a payment on the specified date
      - in: query
        name: paidAtTo
        description: Filter that restricts the search result to orders that received
          a payment within a certain period of time
      - in: query
        name: paymentStatus
        description: Filter that restricts the search result to order with a specific
          payment status
      - in: query
        name: referrerId
        description: Filter that restricts the search result to orders from one order
          referrer
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to orders with a specific
          shipping profile
      - in: query
        name: statusFrom
        description: Filter that restricts the search result to orders in a specific
          order status
      - in: query
        name: statusTo
        description: Filter that restricts the search result to orders within a range
          of order statuses
      - in: query
        name: supplierId
        description: Filter that restricts the search result to orders that include
          order items with variations from a supplier
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to orders that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to orders that were last
          updated within a specified period of time
      - in: query
        name: warehouseId
        description: Filter that restricts the search result to orders with a specific
          main warehouse
      - in: query
        name: with
        description: Load additional relations for an order
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - By
      - Filter
      - Options