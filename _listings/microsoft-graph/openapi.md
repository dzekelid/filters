---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraphmicrosoftcom-microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /workbook/tables(&lt;id|name&gt;)/clearFilters:
    post:
      summary: Table Clear Filters
      description: 'Table: clearFilters Clears all the filters currently applied on
        the table.'
      operationId: Table:ClearFilters
      x-api-path-slug: workbooktablesltidnamegtclearfilters-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      responses:
        200:
          description: OK
      tags:
      - Table
      - Clear
      - Filters
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/clearFilters:
    post:
      summary: Table Clear Filters
      description: 'Table: clearFilters Clears all the filters currently applied on
        the table.'
      operationId: Table:ClearFilters
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtclearfilters-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      responses:
        200:
          description: OK
      tags:
      - Table
      - Clear
      - Filters
  /workbook/tables(&lt;id|name&gt;)/reapplyFilters:
    post:
      summary: Table Reapply Filters
      description: 'Table: reapplyFilters Reapplies all the filters currently on the
        table.'
      operationId: Table:ReapplyFilters
      x-api-path-slug: workbooktablesltidnamegtreapplyfilters-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      responses:
        200:
          description: OK
      tags:
      - Table
      - Reapply
      - Filters
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/reapplyFilters:
    post:
      summary: Table Reapply Filters
      description: 'Table: reapplyFilters Reapplies all the filters currently on the
        table.'
      operationId: Table:ReapplyFilters
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtreapplyfilters-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      responses:
        200:
          description: OK
      tags:
      - Table
      - Reapply
      - Filters
---