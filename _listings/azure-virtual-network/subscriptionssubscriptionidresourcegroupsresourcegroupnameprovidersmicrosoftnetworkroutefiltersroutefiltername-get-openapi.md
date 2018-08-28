---
swagger: "2.0"
x-collection-name: Azure Virtual Network
x-complete: 0
info:
  title: Azure Virtual Network API Route Filters Get
  description: Gets the specified route filter.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/routeFilters/{routeFilterName}:
    delete:
      summary: Route Filters Delete
      description: Deletes the specified route filter.
      operationId: RouteFilters_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworkroutefiltersroutefiltername-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: routeFilterName
        description: The name of the route filter
      responses:
        200:
          description: OK
      tags:
      - Route Filters
    get:
      summary: Route Filters Get
      description: Gets the specified route filter.
      operationId: RouteFilters_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworkroutefiltersroutefiltername-get
      parameters:
      - in: query
        name: $expand
        description: Expands referenced express route bgp peering resources
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: routeFilterName
        description: The name of the route filter
      responses:
        200:
          description: OK
      tags:
      - Route Filters
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