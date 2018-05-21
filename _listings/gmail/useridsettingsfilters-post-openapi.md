---
swagger: "2.0"
x-collection-name: Gmail
x-complete: 0
info:
  title: Gmail Create Message Filters
  description: Creates a filter.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /gmail/v1/users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{userId}/settings/filters:
    get:
      summary: Get Message Filters
      description: Lists the message filters of a Gmail user.
      operationId: gmail.users.settings.filters.list
      x-api-path-slug: useridsettingsfilters-get
      parameters:
      - in: path
        name: userId
        description: Users email address
      responses:
        200:
          description: OK
      tags:
      - Filters
    post:
      summary: Create Message Filters
      description: Creates a filter.
      operationId: gmail.users.settings.filters.create
      x-api-path-slug: useridsettingsfilters-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
        description: Users email address
      responses:
        200:
          description: OK
      tags:
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