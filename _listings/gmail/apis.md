---
name: Gmail
x-slug: gmail
description: The Gmail API is a RESTful API that can be used to access Gmail mailboxes
  and send mail. For most web applications (including mobile apps), the Gmail API
  is the best choice for authorized access to a users Gmail data.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Filters
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/apis.md
specificationVersion: "0.14"
apis:
- name: Gmail - Get Message Filters
  x-api-slug: useridsettingsfilters-get
  description: Lists the message filters of a Gmail user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users
  tags: Google APIs, Stack Network, Stack, Productivity, API Provider, Emails, Profiles,
    Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/useridsettingsfilters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/useridsettingsfilters-get-openapi.md
- name: Gmail - Create Message Filters
  x-api-slug: useridsettingsfilters-post
  description: Creates a filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users
  tags: Google APIs, Stack Network, Stack, Productivity, API Provider, Emails, Profiles,
    Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/useridsettingsfilters-post-openapi.md
- name: Gmail - Delete Message Filter
  x-api-slug: useridsettingsfiltersid-delete
  description: Deletes a filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users
  tags: Google APIs, Stack Network, Stack, Productivity, API Provider, Emails, Profiles,
    Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/useridsettingsfiltersid-delete-openapi.md
- name: Gmail - Get Message Filter
  x-api-slug: useridsettingsfiltersid-get
  description: Gets a filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users
  tags: Google APIs, Stack Network, Stack, Productivity, API Provider, Emails, Profiles,
    Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/useridsettingsfiltersid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://globalchange.gov.api.gallery.streamdata.io
- type: x-api-stack
  url: http://gmail.stack.network
- type: x-auth-scopes
  url: https://developers.google.com/gmail/api/auth/scopes
- type: x-authentication
  url: https://developers.google.com/gmail/api/auth/about-auth
- type: x-developer
  url: https://developers.google.com/gmail/api/
- type: x-documentation
  url: https://developers.google.com/gmail/api/v1/reference/
- type: x-twitter
  url: https://twitter.com/gmail
- type: x-website
  url: https://www.google.com/gmail/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---