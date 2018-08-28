---
swagger: "2.0"
x-collection-name: The TVDB
x-complete: 0
info:
  title: The TVDB Get Series Filter Params
  description: Returns the list of keys available for the `/series/{id}/filter` route
  version: 2.1.2
host: api-dev.thetvdb.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /series/{id}/filter:
    get:
      summary: Get Series Filter
      description: Returns a series records, filtered by the supplied comma-separated
        list of keys. Query keys can be found at the `/series/{id}/filter/params`
        route.
      operationId: series.id.filter.get
      x-api-path-slug: seriesidfilter-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Filter
  /series/{id}/filter/params:
    get:
      summary: Get Series Filter Params
      description: Returns the list of keys available for the `/series/{id}/filter`
        route
      operationId: series.id.filter.params.get
      x-api-path-slug: seriesidfilterparams-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Filter
      - Params
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