---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Filter Apply
  description: 'Filter: apply Apply the given filter criteria on the given column.'
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
        description: Bearer
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
        description: Bearer
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
        description: Bearer
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
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Reapply
      - Filters
  /workbook/tables(&lt;id|name&gt;)/columns(&lt;id|name&gt;)/filter/apply:
    post:
      summary: Filter Apply
      description: 'Filter: apply Apply the given filter criteria on the given column.'
      operationId: Filter:Apply
      x-api-path-slug: workbooktablesltidnamegtcolumnsltidnamegtfilterapply-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Filter
      - Apply
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/columns(&lt;id|name&gt;)/filter/apply:
    post:
      summary: Filter Apply
      description: 'Filter: apply Apply the given filter criteria on the given column.'
      operationId: Filter:Apply
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtcolumnsltidnamegtfilterapply-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Filter
      - Apply
  /workbook/tables(&lt;id|name&gt;)/columns(&lt;id|name&gt;)/filter/clear:
    post:
      summary: Filter Clear
      description: 'Filter: clear Clear the filter on the given column.'
      operationId: Filter:Clear
      x-api-path-slug: workbooktablesltidnamegtcolumnsltidnamegtfilterclear-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Filter
      - Clear
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/columns(&lt;id|name&gt;)/filter/clear:
    post:
      summary: Filter Clear
      description: 'Filter: clear Clear the filter on the given column.'
      operationId: Filter:Clear
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtcolumnsltidnamegtfilterclear-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Filter
      - Clear
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