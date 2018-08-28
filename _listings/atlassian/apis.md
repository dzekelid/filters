---
name: Atlassian
x-slug: atlassian
description: Millions of users globally rely on Atlassian products every day for improving
  software development, project management, collaboration, and code quality.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
x-kinRank: "8"
x-alexaRank: "1656"
tags: Filters
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/apis.md
specificationVersion: "0.14"
apis:
- name: Jira Cloud REST API - Get filters
  x-api-slug: api2filter-get
  description: |-
    Returns all filters. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** None, however only the following filters are returned:

    *   Filters owned by the user.
    *   Filters shared with a group that the user is a member of.
    *   Filters shared with a private project that the user can browse.
    *   Filters shared with a public project, even if the user is anonymous.
    *   Filters shared with the public, even if the user is anonymous.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filter-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filter-get-openapi.md
- name: Jira Cloud REST API - Get favourite filters
  x-api-slug: api2filterfavourite-get
  description: Returns the favorite filters of the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL)).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterfavourite-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterfavourite-get-openapi.md
- name: Jira Cloud REST API - Get my filters
  x-api-slug: api2filtermy-get
  description: Returns the filters owned by the calling user. If `includeFavourites`
    is `true`, the user's favorite filters are also returned. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL)).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filtermy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filtermy-get-openapi.md
- name: Jira Cloud REST API - Create filter
  x-api-slug: api2filter-post
  description: Creates a new filter. The new filter is not shared and not selected
    as a favorite. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
    Permission to log in to Jira.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filter-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filter-post-openapi.md
- name: Jira Cloud REST API - Get filter
  x-api-slug: api2filterid-get
  description: Returns a filter. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** None, however the calling user must have permission view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-get-openapi.md
- name: Jira Cloud REST API - Update filter
  x-api-slug: api2filterid-put
  description: |-
    Updates an existing filter. Use this method to update a filter's name, description, JQL, or sharing. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira, however the following rules govern what a user can update:

    *   Private filters (i.e., not shared) can only be updated by the creator of the filter.
    *   Shared filters can only be updated by the creator of the filter or a Jira administrator.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-put-openapi.md
- name: Jira Cloud REST API - Delete filter
  x-api-slug: api2filterid-delete
  description: |-
    Delete a filter. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira, however the following rules govern what a user can delete:

    *   Private filters (i.e., not shared) can only be deleted by the creator of the filter.
    *   Shared filters can only be deleted by the creator of the filter or a Jira administrator.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-delete-openapi.md
- name: Jira Cloud REST API - Add filter as favorite
  x-api-slug: api2filteridfavourite-put
  description: Add a filter as a favorite for the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL))
    and permission to view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-put-openapi.md
- name: Jira Cloud REST API - Remove filter as favorite
  x-api-slug: api2filteridfavourite-delete
  description: Removes a filter as a favorite for the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL))
    and permission to view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-delete-openapi.md
- name: Jira Cloud REST API - Search for filters
  x-api-slug: api2filtersearch-get
  description: |-
    Search for filters. This method is similar to [Get filters](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-filter-get) except that you can refine the results to include filters that have specific attributes. For example, filters with a particular name. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** None, however only the following filters are returned (if no search parameters are set):

    *   Filters owned by the user.
    *   Filters shared with a group that the user is a member of.
    *   Filters shared with a private project that the user can browse.
    *   Filters shared with a public project, even if the user is anonymous.
    *   Filters shared with the public, even if the user is anonymous.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filtersearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filtersearch-get-openapi.md
- name: Jira Cloud REST API - Create filter
  x-api-slug: api2filter-post
  description: Creates a new filter. The new filter is not shared and not selected
    as a favorite. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
    Permission to log in to Jira.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filter-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filter-post-openapi.md
- name: Jira Cloud REST API - Get filter
  x-api-slug: api2filterid-get
  description: Returns a filter. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** None, however the calling user must have permission view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-get-openapi.md
- name: Jira Cloud REST API - Update filter
  x-api-slug: api2filterid-put
  description: |-
    Updates an existing filter. Use this method to update a filter's name, description, JQL, or sharing. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira, however the following rules govern what a user can update:

    *   Private filters (i.e., not shared) can only be updated by the creator of the filter.
    *   Shared filters can only be updated by the creator of the filter or a Jira administrator.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-put-openapi.md
- name: Jira Cloud REST API - Delete filter
  x-api-slug: api2filterid-delete
  description: |-
    Delete a filter. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira, however the following rules govern what a user can delete:

    *   Private filters (i.e., not shared) can only be deleted by the creator of the filter.
    *   Shared filters can only be deleted by the creator of the filter or a Jira administrator.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-delete-openapi.md
- name: Jira Cloud REST API - Add filter as favorite
  x-api-slug: api2filteridfavourite-put
  description: Add a filter as a favorite for the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL))
    and permission to view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-put-openapi.md
- name: Jira Cloud REST API - Remove filter as favorite
  x-api-slug: api2filteridfavourite-delete
  description: Removes a filter as a favorite for the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL))
    and permission to view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-delete-openapi.md
- name: Jira Cloud REST API - Get filters
  x-api-slug: api2filter-get
  description: |-
    Returns all filters. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** None, however only the following filters are returned:

    *   Filters owned by the user.
    *   Filters shared with a group that the user is a member of.
    *   Filters shared with a private project that the user can browse.
    *   Filters shared with a public project, even if the user is anonymous.
    *   Filters shared with the public, even if the user is anonymous.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filter-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filter-get-openapi.md
- name: Jira Cloud REST API - Search for filters
  x-api-slug: api2filtersearch-get
  description: |-
    Search for filters. This method is similar to [Get filters](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-filter-get) except that you can refine the results to include filters that have specific attributes. For example, filters with a particular name. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** None, however only the following filters are returned (if no search parameters are set):

    *   Filters owned by the user.
    *   Filters shared with a group that the user is a member of.
    *   Filters shared with a private project that the user can browse.
    *   Filters shared with a public project, even if the user is anonymous.
    *   Filters shared with the public, even if the user is anonymous.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filtersearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filtersearch-get-openapi.md
- name: Jira Cloud REST API - Get columns
  x-api-slug: api2filteridcolumns-get
  description: Returns the columns configured for a filter. The column configuration
    is used when the filter's results are viewed in _List View_ with the _Columns_
    set to _Filter_. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
    None, however the calling user must have permission to view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridcolumns-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridcolumns-get-openapi.md
- name: Jira Cloud REST API - Remove filter as favorite
  x-api-slug: api2filteridfavourite-delete
  description: Removes a filter as a favorite for the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL))
    and permission to view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-delete-openapi.md
- name: Jira Cloud REST API - Remove filter as favorite
  x-api-slug: api2filteridfavourite-delete
  description: Removes a filter as a favorite for the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL))
    and permission to view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-delete-openapi.md
- name: Jira Cloud REST API - Add filter as favorite
  x-api-slug: api2filteridfavourite-put
  description: Add a filter as a favorite for the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL))
    and permission to view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-put-openapi.md
- name: Jira Cloud REST API - Add filter as favorite
  x-api-slug: api2filteridfavourite-put
  description: Add a filter as a favorite for the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL))
    and permission to view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filteridfavourite-put-openapi.md
- name: Jira Cloud REST API - Delete filter
  x-api-slug: api2filterid-delete
  description: |-
    Delete a filter. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira, however the following rules govern what a user can delete:

    *   Private filters (i.e., not shared) can only be deleted by the creator of the filter.
    *   Shared filters can only be deleted by the creator of the filter or a Jira administrator.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-delete-openapi.md
- name: Jira Cloud REST API - Delete filter
  x-api-slug: api2filterid-delete
  description: |-
    Delete a filter. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira, however the following rules govern what a user can delete:

    *   Private filters (i.e., not shared) can only be deleted by the creator of the filter.
    *   Shared filters can only be deleted by the creator of the filter or a Jira administrator.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-delete-openapi.md
- name: Jira Cloud REST API - Update filter
  x-api-slug: api2filterid-put
  description: |-
    Updates an existing filter. Use this method to update a filter's name, description, JQL, or sharing. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira, however the following rules govern what a user can update:

    *   Private filters (i.e., not shared) can only be updated by the creator of the filter.
    *   Shared filters can only be updated by the creator of the filter or a Jira administrator.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-put-openapi.md
- name: Jira Cloud REST API - Update filter
  x-api-slug: api2filterid-put
  description: |-
    Updates an existing filter. Use this method to update a filter's name, description, JQL, or sharing. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira, however the following rules govern what a user can update:

    *   Private filters (i.e., not shared) can only be updated by the creator of the filter.
    *   Shared filters can only be updated by the creator of the filter or a Jira administrator.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-put-openapi.md
- name: Jira Cloud REST API - Get filter
  x-api-slug: api2filterid-get
  description: Returns a filter. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** None, however the calling user must have permission view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-get-openapi.md
- name: Jira Cloud REST API - Get filter
  x-api-slug: api2filterid-get
  description: Returns a filter. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** None, however the calling user must have permission view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filterid-get-openapi.md
- name: Jira Cloud REST API - Create filter
  x-api-slug: api2filter-post
  description: Creates a new filter. The new filter is not shared and not selected
    as a favorite. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
    Permission to log in to Jira.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filter-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filter-post-openapi.md
- name: Jira Cloud REST API - Create filter
  x-api-slug: api2filter-post
  description: Creates a new filter. The new filter is not shared and not selected
    as a favorite. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
    Permission to log in to Jira.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filter-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/atlassian/api2filter-post-openapi.md
x-common:
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/platform/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/confluence/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
- type: x-website
  url: http://atlassian.com/
- type: x-website
  url: http://www.atlassian.com
- type: x-api-gallery
  url: http://att.dev.program.api.gallery.streamdata.io
- type: x-api-stack
  url: http://atlassian.stack.network
- type: x-blog
  url: http://blogs.atlassian.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/atlassian
- type: x-crunchbase
  url: http://www.crunchbase.com/company/atlassian
- type: x-email
  url: copyright@atlassian.com
- type: x-email
  url: trademarks@atlassian.com
- type: x-email
  url: sales@atlassian.com
- type: x-email
  url: ar_enterprise@atlassian.com
- type: x-email
  url: privacy@atlassian.com
- type: x-email
  url: eudatarep@atlassian.com
- type: x-email
  url: experts@atlassian.com
- type: x-email
  url: remittance@atlassian.com
- type: x-email
  url: ap@atlassian.com
- type: x-email
  url: procurement@atlassian.com
- type: x-github
  url: https://github.com/atlassian
- type: x-privacy-policy
  url: https://www.atlassian.com/legal/privacy-policy?_ga=2.188884514.868776184.1519225620-845241124.1519225620
- type: x-twitter
  url: https://twitter.com/atlassian
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---