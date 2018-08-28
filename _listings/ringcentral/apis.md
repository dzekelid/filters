---
name: RingCentral
x-slug: ringcentral
description: 'RingCentral, Inc. (NYSE: RNG) is a global provider of cloud enterprise
  unified communications and collaboration solutions. More flexible and cost-effective
  than legacy on-premise systems, RingCentral empowers today&rsquo;s mobile and distributed
  workforces to be connected anywhere and on any device through voice, video, team
  messaging, collaboration, SMS, conferencing, online meetings, contact center, and
  fax. RingCentral provides an open platform that integrates with today&rsquo;s leading
  business apps while giving customers the flexibility to customize their own workflows.'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
x-kinRank: "7"
x-alexaRank: "7180"
tags: Filters
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/apis.md
specificationVersion: "0.14"
apis:
- name: RingCentral Connect Platform API Explorer - Renew Subscription / Update Event
    Filters
  x-api-slug: restapiv1-0subscriptionsubscriptionid-put
  description: "Renews the existent subscription if the request body is empty. If
    event filters are specified, calling this method modifies the event filters for
    the existing subscription. The client application can extend or narrow the events
    for which it receives notifications in the frame of one subscription.\nUsage Plan
    Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n404\nCMN-102\nResource for parameter [subscriptionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Log Records by Filter
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcalllog-get
  description: "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser
    Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter [sessionId]
    is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
    [transport] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-129\nAccess
    token corrupted\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n401\nOAU-213\nToken
    not found\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs
    to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this API
    endpoint, user needs to have [ReadCallLog] permission for requested resource.\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found\n\n\n429\nCMN-301\nRequest rate exceeded"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllog-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Log Records by Filter
  x-api-slug: restapiv1-0accountaccountidcalllog-get
  description: "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser
    Permission\nFullCompanyCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter
    [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
    [dateFrom] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this
    API endpoint, user needs to have [ReadCompanyCallLog] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidcalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidcalllog-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Log Records by Filter
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcalllog-get
  description: "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser
    Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter [sessionId]
    is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
    [transport] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-129\nAccess
    token corrupted\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n401\nOAU-213\nToken
    not found\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs
    to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this API
    endpoint, user needs to have [ReadCallLog] permission for requested resource.\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found\n\n\n429\nCMN-301\nRequest rate exceeded"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllog-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Log Records by Filter
  x-api-slug: restapiv1-0accountaccountidcalllog-get
  description: "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser
    Permission\nFullCompanyCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter
    [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
    [dateFrom] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this
    API endpoint, user needs to have [ReadCompanyCallLog] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidcalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidcalllog-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Log Records by Filter
  x-api-slug: restapiv1-0accountaccountidcalllog-get
  description: "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser
    Permission\nFullCompanyCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter
    [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
    [dateFrom] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this
    API endpoint, user needs to have [ReadCompanyCallLog] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidcalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidcalllog-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Log Records by Filter
  x-api-slug: restapiv1-0accountaccountidcalllog-get
  description: "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser
    Permission\nFullCompanyCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter
    [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
    [dateFrom] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this
    API endpoint, user needs to have [ReadCompanyCallLog] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidcalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidcalllog-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Log Records by Filter
  x-api-slug: restapiv1-0accountaccountidcalllog-get
  description: "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser
    Permission\nFullCompanyCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter
    [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
    [dateFrom] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this
    API endpoint, user needs to have [ReadCompanyCallLog] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidcalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidcalllog-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Log Records by Filter
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcalllog-get
  description: "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser
    Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter [sessionId]
    is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
    [transport] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-129\nAccess
    token corrupted\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n401\nOAU-213\nToken
    not found\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs
    to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this API
    endpoint, user needs to have [ReadCallLog] permission for requested resource.\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found\n\n\n429\nCMN-301\nRequest rate exceeded"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllog-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Log Records by Filter
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcalllog-get
  description: "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser
    Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter [sessionId]
    is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
    [transport] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-129\nAccess
    token corrupted\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n401\nOAU-213\nToken
    not found\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs
    to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this API
    endpoint, user needs to have [ReadCallLog] permission for requested resource.\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found\n\n\n429\nCMN-301\nRequest rate exceeded"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllog-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Log Records by Filter
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcalllog-get
  description: "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser
    Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter [sessionId]
    is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
    [transport] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-129\nAccess
    token corrupted\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n401\nOAU-213\nToken
    not found\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs
    to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this API
    endpoint, user needs to have [ReadCallLog] permission for requested resource.\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found\n\n\n429\nCMN-301\nRequest rate exceeded"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllog-get-openapi.md
x-common:
- type: x-blog
  url: https://medium.com/ringcentral-developers
- type: x-blog-rss
  url: https://medium.com/feed/ringcentral-developers
- type: x-github
  url: https://github.com/ringcentral
- type: x-openapi
  url: https://netstorage.ringcentral.com/dpw/api-explorer/swagger-ring_basic.yml?v=20180816
- type: x-website
  url: http://www.ringcentral.com
- type: x-api-gallery
  url: http://reverb.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ringcentral.stack.network
- type: x-code
  url: https://developer.ringcentral.com/library/sdks.html
- type: x-crunchbase
  url: https://crunchbase.com/organization/ringcentral
- type: x-developer
  url: https://developer.ringcentral.com/
- type: x-documentation
  url: https://developer.ringcentral.com/api-explorer/latest/index.html?_ga=2.259782990.551967760.1534465156-1236351744.1533920460
- type: x-support
  url: https://developer.ringcentral.com/support.html
- type: x-twitter
  url: https://twitter.com/RingCentral
- type: x-website
  url: https://developer.ringcentral.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---