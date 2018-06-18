---
swagger: "2.0"
x-collection-name: Azure Virtual Network
x-complete: 0
info:
  title: Azure Virtual Network API Route Filters Update
  description: Updates a route filter in a specified resource group.
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkroutefiltersroutefiltername-delete
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkroutefiltersroutefiltername-get
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
    put:
      summary: Route Filters Create Or Update
      description: Creates or updates a route filter in a specified resource group.
      operationId: RouteFilters_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkroutefiltersroutefiltername-put
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: routeFilterName
        description: The name of the route filter
      - in: body
        name: routeFilterParameters
        description: Parameters supplied to the create or update route filter operation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Route Filters
    patch:
      summary: Route Filters Update
      description: Updates a route filter in a specified resource group.
      operationId: RouteFilters_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkroutefiltersroutefiltername-patch
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: routeFilterName
        description: The name of the route filter
      - in: body
        name: routeFilterParameters
        description: Parameters supplied to the update route filter operation
        schema:
          $ref: '#/definitions/holder'
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