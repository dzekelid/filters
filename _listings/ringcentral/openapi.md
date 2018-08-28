swagger: "2.0"
x-collection-name: RingCentral
x-complete: 1
info:
  title: RingCentral Connect Platform API Explorer
  description: this-is-an-interactive-api-explorer-for-the-ringcentral-connect-platform--to-use-this-service-you-will-need-to-have-a-developer-account---links--a-hrefhttpsnetstorage-ringcentral-comdpwapiexplorerrcplatform-basic-ymlv20180514092722-target-blankringcentral-api-specaspannbspnbspopenapi-fka-swagger-formatnbspnbspnbspnbspspana-hrefhttpsgithub-comoaiopenapispecification-target-blanklearn-more-about-openapia
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
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/call-log:
    get:
      summary: Get Call Log Records by Filter
      description: "Returns call log records filtered by parameters specified.\nApp
        Permission\nReadCallLog\nUser Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter
        [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
        [transport] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-129\nAccess
        token corrupted\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n401\nOAU-213\nToken
        not found\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
        needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call
        this API endpoint, user needs to have [ReadCallLog] permission for requested
        resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found\n\n\n429\nCMN-301\nRequest
        rate exceeded"
      operationId: loadExtensionCallLog
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidcalllog-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: query
        name: dateFrom
        description: The start datetime for resulting records in ISO 8601 format including
          timezone, for example 2016-03-10T18:07:52
      - in: query
        name: dateTo
        description: The end datetime for resulting records in ISO 8601 format including
          timezone, for example 2016-03-10T18:07:52
      - in: query
        name: direction
        description: The direction for the resulting records
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: query
        name: extensionNumber
        description: Extension number of a user
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: phoneNumber
        description: Phone number of a caller/callee
      - in: query
        name: sessionId
      - in: query
        name: showBlocked
        description: If True then calls from/to blocked numbers are returned
      - in: query
        name: transport
        description: Call transport type
      - in: query
        name: type
        description: Call type of a record
      - in: query
        name: view
        description: The default value is Simple for both account and extension call
          log
      - in: query
        name: withRecording
        description: True should be specified to return recorded calls only
      responses:
        200:
          description: OK
      tags:
      - Call
      - Log
      - Records
      - By
      - Filter
  /restapi/v1.0/account/{accountId}/call-log:
    get:
      summary: Get Call Log Records by Filter
      description: "Returns call log records filtered by parameters specified.\nApp
        Permission\nReadCallLog\nUser Permission\nFullCompanyCallLog\nUsage Plan Group\nHeavy\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter
        [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
        [dateFrom] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order
        to call this API endpoint, user needs to have [ReadCompanyCallLog] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
        is not found"
      operationId: loadAccountCallLog
      x-api-path-slug: restapiv1-0accountaccountidcalllog-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: query
        name: dateFrom
        description: The start datetime for resulting records in ISO 8601 format including
          timezone, for example 2016-03-10T18:07:52
      - in: query
        name: dateTo
        description: The end datetime for resulting records in ISO 8601 format including
          timezone, for example 2016-03-10T18:07:52
      - in: query
        name: direction
        description: The direction for the result records
      - in: query
        name: extensionNumber
        description: Extension number of a user
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: phoneNumber
        description: Phone number of a caller/call recipient
      - in: query
        name: sessionId
      - in: query
        name: type
        description: Call type of a record
      - in: query
        name: view
        description: The default value is Simple for both account and extension call
          log
      - in: query
        name: withRecording
        description: True if only recorded calls have to be returned
      responses:
        200:
          description: OK
      tags:
      - Call
      - Log
      - Records
      - By
      - Filter