---
swagger: "2.0"
x-collection-name: Azure Virtual Network
x-complete: 1
info:
  title: NetworkManagementClient
  description: the-microsoft-azure-network-management-api-provides-a-restful-set-of-web-services-that-interact-with-microsoft-azure-networks-service-to-manage-your-network-resources-the-api-has-entities-that-capture-the-relationship-between-an-end-user-and-the-microsoft-azure-networks-service
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
    put:
      summary: Route Filters Create Or Update
      description: Creates or updates a route filter in a specified resource group.
      operationId: RouteFilters_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworkroutefiltersroutefiltername-put
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworkroutefiltersroutefiltername-patch
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
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/routeFilters:
    get:
      summary: Route Filters List By Resource Group
      description: Gets all route filters in a resource group.
      operationId: RouteFilters_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworkroutefilters-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Route Filters
  /subscriptions/{subscriptionId}/providers/Microsoft.Network/routeFilters:
    get:
      summary: Route Filters List
      description: Gets all route filters in a subscription.
      operationId: RouteFilters_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftnetworkroutefilters-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Route Filters
---