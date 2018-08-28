---
swagger: "2.0"
x-collection-name: Google Analytics
x-complete: 0
info:
  title: Google Analytics Update Filter
  description: Updates an existing filter. This method supports patch semantics.
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /analytics/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /management/accounts/{accountId}/filters:
    get:
      summary: Get Filters
      description: Lists all filters for an account
      operationId: analytics.management.filters.list
      x-api-path-slug: managementaccountsaccountidfilters-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve filters for
      - in: query
        name: max-results
        description: The maximum number of filters to include in this response
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      responses:
        200:
          description: OK
      tags:
      - Filter
    post:
      summary: Create Filter
      description: Create a new filter.
      operationId: analytics.management.filters.insert
      x-api-path-slug: managementaccountsaccountidfilters-post
      parameters:
      - in: path
        name: accountId
        description: Account ID to create filter for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Filter
  /management/accounts/{accountId}/filters/{filterId}:
    delete:
      summary: Delete Filter
      description: Delete a filter.
      operationId: analytics.management.filters.delete
      x-api-path-slug: managementaccountsaccountidfiltersfilterid-delete
      parameters:
      - in: path
        name: accountId
        description: Account ID to delete the filter for
      - in: path
        name: filterId
        description: ID of the filter to be deleted
      responses:
        200:
          description: OK
      tags:
      - Filter
    get:
      summary: Get Filter
      description: Returns a filters to which the user has access.
      operationId: analytics.management.filters.get
      x-api-path-slug: managementaccountsaccountidfiltersfilterid-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve filters for
      - in: path
        name: filterId
        description: Filter ID to retrieve filters for
      responses:
        200:
          description: OK
      tags:
      - Filter
    patch:
      summary: Update Filter
      description: Updates an existing filter. This method supports patch semantics.
      operationId: analytics.management.filters.patch
      x-api-path-slug: managementaccountsaccountidfiltersfilterid-patch
      parameters:
      - in: path
        name: accountId
        description: Account ID to which the filter belongs
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: filterId
        description: ID of the filter to be updated
      responses:
        200:
          description: OK
      tags:
      - Filter
    put:
      summary: Update Filter
      description: Updates an existing filter.
      operationId: analytics.management.filters.update
      x-api-path-slug: managementaccountsaccountidfiltersfilterid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID to which the filter belongs
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: filterId
        description: ID of the filter to be updated
      responses:
        200:
          description: OK
      tags:
      - Filter
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