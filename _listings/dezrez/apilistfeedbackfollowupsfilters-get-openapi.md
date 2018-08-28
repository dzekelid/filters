---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get all saved feedback follow up list filters
  version: 1.0.0
  description: Get all saved feedback follow up list filters.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/list/followups/filters:
    get:
      summary: Get all saved follow up list filters
      description: Get all saved follow up list filters.
      operationId: List_GetFollowUpListFiltersByroleTypeBycontext
      x-api-path-slug: apilistfollowupsfilters-get
      parameters:
      - in: query
        name: context
        description: Filter context
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleType
        description: Filter roleType
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Follow
      - Up
      - List
      - Filters
  /api/list/feedback/followups/filters:
    get:
      summary: Get all saved feedback follow up list filters
      description: Get all saved feedback follow up list filters.
      operationId: List_GetFeedbackFollowUpListFiltersByroleTypeBycontext
      x-api-path-slug: apilistfeedbackfollowupsfilters-get
      parameters:
      - in: query
        name: context
        description: Filter context
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleType
        description: Filter roleType
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Feedback
      - Follow
      - Up
      - List
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