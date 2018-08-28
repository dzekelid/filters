---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List tickets by filters
  description: List tickets by filters.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---