---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook Graph (Achievement Type) API
  description: api-for-managing-facebook-achievement-types
  termsOfService: https://www.facebook.com/policies/
  version: 1.0.0
host: graph.facebook.com
basePath: /v3.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /&#123;user-id&#125;/stream_filters:
    get:
      summary: Get User Stream Filters
      description: User Stream Filters
      operationId: getUserStreamFilters
      x-api-path-slug: 123userid125stream-filters-get
      parameters:
      - in: query
        name: "200"
        description: Permissions error
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Stream
      - Filters
---