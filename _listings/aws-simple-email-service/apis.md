---
name: AWS Simple Email Service
x-slug: aws-simple-email-service
description: Amazon Simple Email Service (Amazon SES) is a cost-effective email service
  built on the reliable and scalable infrastructure that Amazon.com developed to serve
  its own customer base. With Amazon SES, you can send and receive email with no required
  minimum commitments &ndash; you pay as you go, and you only pay for what you use.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSES.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Filters
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/aws-simple-email-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Simple Email Service API Create Receipt Filter
  x-api-slug: aws-simple-email-service-api
  description: Creates a new IP address filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSES.png
  humanURL: https://aws.amazon.com/ses/
  baseURL: ://///?Action=CreateReceiptFilter
  tags: Receipt Filters
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/aws-simple-email-service/actioncreatereceiptfilter-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/aws-simple-email-service/actioncreatereceiptfilter-get-openapi.md
- name: AWS Simple Email Service API Delete Receipt Filter
  x-api-slug: aws-simple-email-service-api
  description: Deletes the specified IP address filter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSES.png
  humanURL: https://aws.amazon.com/ses/
  baseURL: ://///?Action=DeleteReceiptFilter
  tags: Receipt Filters
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/aws-simple-email-service/actiondeletereceiptfilter-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/aws-simple-email-service/actiondeletereceiptfilter-get-openapi.md
- name: AWS Simple Email Service API List Receipt Filters
  x-api-slug: aws-simple-email-service-api
  description: Lists the IP address filters associated with your AWS account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSES.png
  humanURL: https://aws.amazon.com/ses/
  baseURL: ://///?Action=ListReceiptFilters
  tags: 'Receipt Filters '
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/aws-simple-email-service/actionlistreceiptfilters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/aws-simple-email-service/actionlistreceiptfilters-get-openapi.md
- name: AWS Simple Email Service API
  x-api-slug: aws-simple-email-service-api
  description: Amazon Simple Email Service (Amazon SES) is a cost-effective email
    service built on the reliable and scalable infrastructure that Amazon.com developed
    to serve its own customer base. With Amazon SES, you can send and receive email
    with no required minimum commitments &ndash; you pay as you go, and you only pay
    for what you use.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSES.png
  humanURL: https://aws.amazon.com/ses/
  baseURL: :///
  tags: Filters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/aws-simple-email-service/openapi.md
x-common:
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/Amazon-SES
- type: x-documentation
  url: http://docs.aws.amazon.com/ses/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/ses/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=90
- type: x-getting-started
  url: https://aws.amazon.com/ses/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/ses/pricing/
- type: x-sdk
  url: http://aws.amazon.com/tools
- type: x-service-health
  url: http://status.aws.amazon.com/
- type: x-tools
  url: http://aws.amazon.com/developertools/Amazon-SES
- type: x-website
  url: https://aws.amazon.com/ses/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---