---
name: Azure Resource Health
description: Resource health helps you diagnose and get support when an Azure issue
  impacts your resources. It informs you about the current and past health of your
  resources and helps you mitigate issues. Resource health provides technical support
  when you need help with Azure service issues.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-health.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Stack Network
- Monitoring
- Microsoft
created: "2018-03-13"
modified: "2018-03-13"
url: https://raw.githubusercontent.com/streamdata-gallery/availability/master/_listings/azure-resource-health/apis.yaml
specificationVersion: "0.14"
apis:
- name: Azure Resource Health API
  description: Resource health helps you diagnose and get support when an Azure issue
    impacts your resources
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-health.png
  humanURL: ""
  baseURL: ://management.azure.com//
  tags: Availability
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/availability/master/_listings/azure-resource-health/resourceuri-providers-microsoft-resourcehealth-availabilitystatuses-get.md
- name: Azure Resource Health API Availability Statuses List By Subscription Id
  description: Lists the current availability status for all the resources in the
    subscription. Use the nextLink property in the response to get the next page of
    availability statuses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-health.png
  humanURL: https://docs.microsoft.com/en-us/azure/resource-health/
  baseURL: http:://management.azure.com//
  tags: Availability
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/availability/master/_listings/azure-resource-health/subscriptions-subscriptionid-providers-microsoft-resourcehealth-availabilitystatuses-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/availability/master/_listings/azure-resource-health/subscriptions-subscriptionid-providers-microsoft-resourcehealth-availabilitystatuses-get-postman.md
x-common:
- type: x-faq
  url: https://docs.microsoft.com/en-us/azure/resource-health/resource-health-faq
- type: x-website
  url: https://docs.microsoft.com/en-us/azure/resource-health/
- type: x-faq
  url: https://docs.microsoft.com/en-us/azure/resource-health/resource-health-faq
- type: x-website
  url: https://docs.microsoft.com/en-us/azure/resource-health/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---