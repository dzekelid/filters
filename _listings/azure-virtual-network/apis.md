---
name: Azure Virtual Network
x-slug: azure-virtual-network
description: Azure Virtual Network lets you create private networks in the cloud with
  full control over IP addresses, DNS servers, security rules, and traffic flows.
  Securely connect a virtual network to on-premises networks by using a VPN tunnel,
  or connect privately by using the ExpressRoute service.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-network-topology.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Filters
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/azure-virtual-network/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Virtual Network API Route Filters Delete
  x-api-slug: azure-virtual-network-api
  description: Deletes the specified route filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-network-topology.png
  humanURL: https://azure.microsoft.com/en-us/services/virtual-network/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/routeFilters/{routeFilterName}
  tags: Route Filters
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/azure-virtual-network/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkroutefiltersroutefiltername-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/azure-virtual-network/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkroutefiltersroutefiltername-delete-openapi.md
- name: Azure Virtual Network API Route Filters Get
  x-api-slug: azure-virtual-network-api
  description: Gets the specified route filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-network-topology.png
  humanURL: https://azure.microsoft.com/en-us/services/virtual-network/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/routeFilters/{routeFilterName}
  tags: Route Filters
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/azure-virtual-network/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkroutefiltersroutefiltername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/azure-virtual-network/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkroutefiltersroutefiltername-get-openapi.md
- name: Azure Virtual Network API Route Filters Create Or Update
  x-api-slug: azure-virtual-network-api
  description: Creates or updates a route filter in a specified resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-network-topology.png
  humanURL: https://azure.microsoft.com/en-us/services/virtual-network/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/routeFilters/{routeFilterName}
  tags: Route Filters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/azure-virtual-network/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkroutefiltersroutefiltername-put-openapi.md
- name: Azure Virtual Network API Route Filters Update
  x-api-slug: azure-virtual-network-api
  description: Updates a route filter in a specified resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-network-topology.png
  humanURL: https://azure.microsoft.com/en-us/services/virtual-network/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/routeFilters/{routeFilterName}
  tags: Route Filters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/azure-virtual-network/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkroutefiltersroutefiltername-patch-openapi.md
- name: Azure Virtual Network API Route Filters List By Resource Group
  x-api-slug: azure-virtual-network-api
  description: Gets all route filters in a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-network-topology.png
  humanURL: https://azure.microsoft.com/en-us/services/virtual-network/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/routeFilters
  tags: Route Filters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/azure-virtual-network/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkroutefilters-get-openapi.md
- name: Azure Virtual Network API Route Filters List
  x-api-slug: azure-virtual-network-api
  description: Gets all route filters in a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-network-topology.png
  humanURL: https://azure.microsoft.com/en-us/services/virtual-network/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Network/routeFilters
  tags: Route Filters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/azure-virtual-network/subscriptionssubscriptionidprovidersmicrosoft-networkroutefilters-get-openapi.md
- name: Azure Virtual Network API
  x-api-slug: azure-virtual-network-api
  description: Azure Virtual Network lets you create private networks in the cloud
    with full control over IP addresses, DNS servers, security rules, and traffic
    flows. Securely connect a virtual network to on-premises networks by using a VPN
    tunnel, or connect privately by using the ExpressRoute service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-network-topology.png
  humanURL: https://azure.microsoft.com/en-us/services/virtual-network/
  baseURL: ://management.azure.com//
  tags: Filters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/azure-virtual-network/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/virtual-network/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/virtual-network/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/virtual-network/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---