---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Views Find all instances of the Deck matched by filter.
  version: 1.0.0
  description: Find all instances of the deck matched by filter..
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /decks:
    get:
      summary: Find all instances of the Deck matched by filter.
      description: Find all instances of the deck matched by filter..
      operationId: getDecks
      x-api-path-slug: decks-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields, where, include, order, offset, and limit
      responses:
        200:
          description: OK
      tags:
      - Find
      - ""
      - Instances
      - Of
      - Deck
      - Matched
      - By
      - Filter
  /cards:
    get:
      summary: Find all instances of the Card matched by filter.
      description: Find all instances of the card matched by filter..
      operationId: getCards
      x-api-path-slug: cards-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields, where, include, order, offset, and limit
      responses:
        200:
          description: OK
      tags:
      - Find
      - ""
      - Instances
      - Of
      - Card
      - Matched
      - By
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