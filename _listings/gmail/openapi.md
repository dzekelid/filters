---
swagger: "2.0"
x-collection-name: Gmail
x-complete: 1
info:
  title: Gmail
  description: access-gmail-mailboxes-including-sending-user-email-
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
  /{userId}/settings/filters/{id}:
    delete:
      summary: Delete Message Filter
      description: Deletes a filter.
      operationId: gmail.users.settings.filters.delete
      x-api-path-slug: useridsettingsfiltersid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the filter to be deleted
      - in: path
        name: userId
        description: Users email address
      responses:
        200:
          description: OK
      tags:
      - Filters
    get:
      summary: Get Message Filter
      description: Gets a filter.
      operationId: gmail.users.settings.filters.get
      x-api-path-slug: useridsettingsfiltersid-get
      parameters:
      - in: path
        name: id
        description: The ID of the filter to be fetched
      - in: path
        name: userId
        description: Users email address
      responses:
        200:
          description: OK
      tags:
      - Filters
---