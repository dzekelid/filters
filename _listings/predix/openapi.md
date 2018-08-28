swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
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