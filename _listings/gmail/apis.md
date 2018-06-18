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
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/apis.md
specificationVersion: "0.14"
apis:
- name: Gmail Get Message Filters
  x-api-slug: gmail
  description: Lists the message filters of a Gmail user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/settings/filters
  tags: Filters
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/useridsettingsfilters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/useridsettingsfilters-get-openapi.md
- name: Gmail Create Message Filters
  x-api-slug: gmail
  description: Creates a filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/settings/filters
  tags: Filters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/useridsettingsfilters-post-openapi.md
- name: Gmail Delete Message Filter
  x-api-slug: gmail
  description: Deletes a filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/settings/filters/{id}
  tags: Filters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/useridsettingsfiltersid-delete-openapi.md
- name: Gmail Get Message Filter
  x-api-slug: gmail
  description: Gets a filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/settings/filters/{id}
  tags: Filters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/useridsettingsfiltersid-get-openapi.md
- name: Gmail
  x-api-slug: gmail
  description: The Gmail API is a RESTful API that can be used to access Gmail mailboxes
    and send mail. For most web applications (including mobile apps), the Gmail API
    is the best choice for authorized access to a users Gmail data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users
  tags: Filters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/gmail/openapi.md
x-common:
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