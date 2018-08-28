---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Renew Subscription / Update Event Filters
  description: "Renews the existent subscription if the request body is empty. If
    event filters are specified, calling this method modifies the event filters for
    the existing subscription. The client application can extend or narrow the events
    for which it receives notifications in the frame of one subscription.\nUsage Plan
    Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n404\nCMN-102\nResource for parameter [subscriptionId] is not found"
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/subscription/{subscriptionId}:
    put:
      summary: Renew Subscription / Update Event Filters
      description: "Renews the existent subscription if the request body is empty.
        If event filters are specified, calling this method modifies the event filters
        for the existing subscription. The client application can extend or narrow
        the events for which it receives notifications in the frame of one subscription.\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n404\nCMN-102\nResource for parameter [subscriptionId] is
        not found"
      operationId: updateSubscription
      x-api-path-slug: restapiv1-0subscriptionsubscriptionid-put
      parameters:
      - in: query
        name: aggregated
        description: If True then aggregated presence status is returned in a notification
          payload
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscriptionId
        description: Internal identifier of a subscription
      responses:
        200:
          description: OK
      tags:
      - Renew
      - Subscription
      - ""
      - ""
      - ""
      - Event
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