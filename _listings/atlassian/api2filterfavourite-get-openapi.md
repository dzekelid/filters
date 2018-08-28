---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get favourite filters
  description: Returns the favorite filters of the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL)).
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/filter:
    get:
      summary: Get filters
      description: |-
        Returns all filters. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** None, however only the following filters are returned:

        *   Filters owned by the user.
        *   Filters shared with a group that the user is a member of.
        *   Filters shared with a private project that the user can browse.
        *   Filters shared with a public project, even if the user is anonymous.
        *   Filters shared with the public, even if the user is anonymous.
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.getFilters_get
      x-api-path-slug: api2filter-get
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      responses:
        200:
          description: OK
      tags:
      - Filters
  /api/2/filter/favourite:
    get:
      summary: Get favourite filters
      description: Returns the favorite filters of the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL)).
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.getFavouriteFilters_get
      x-api-path-slug: api2filterfavourite-get
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      responses:
        200:
          description: OK
      tags:
      - Favourite
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