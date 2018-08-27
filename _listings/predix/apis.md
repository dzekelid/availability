---
name: Predix
x-slug: predix
description: Predix (IoT PaaS) helps you develop apps that connect people with industrial
  machines through analytics and data for better business outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
x-kinRank: "7"
x-alexaRank: "264121"
tags: Availability
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/availability/master/_listings/predix/apis.md
specificationVersion: "0.14"
apis:
- name: Data Services - Get all available aggregations
  x-api-slug: v1aggregations-get
  description: |-
    Return all supported aggregations.Response JSON (Status 200){
      "results": [
        {
          "name": "max",
          "type": "Maximum",
          "description": "Returns the maximum value data point for the time range"
        },
        {
          "name": "trendmode",
          "type": "Trend Mode",
          "description": "Returns the maximum and minimum value data point for the time range"
        },
        {
          "name": "count",
          "type": "Count",
          "description": "Returns the number of data points"
        },
        {
          "name": "scale",
          "type": "Scale",
          "description": "Scales each data point by a factor"
        },
        {
          "name": "interpolate",
          "type": "Interpolate",
          "description": "Does linear interpolation for the chosen window"
        },
        {
          "name": "sum",
          "type": "Sum",
          "description": "Adds the data points together"
        },
        {
          "name": "diff",
          "type": "Difference",
          "description": "Returns the difference between successive data points"
        },
        {
          "name": "gaps",
          "type": "Gaps",
          "description": "Marks gaps in data according to sampling rate with a null data point"
        },
        {
          "name": "sampler",
          "type": "Sampler",
          "description": "Returns the sampling rate of change for the data points"
        },
        {
          "name": "div",
          "type": "Divide",
          "description": "Divides each data point by a divisor"
        },
        {
          "name": "min",
          "type": "Minimum",
          "description": "Returns the minimum value data point for the time range"
        },
        {
          "name": "avg",
          "type": "Average",
          "description": "Returns the average of the data point set"
        },
        {
          "name": "least_squares",
          "type": "Least Squares",
          "description": "Returns a best fit line through the data points using the least squares algorithm"
        },
        {
          "name": "percentile",
          "type": "Percentile",
          "description": "Returns the percentile of the data range"
        },
        {
          "name": "dev",
          "type": "Standard Deviation",
          "description": "Returns the standard deviation of the time series"
        },
        {
          "name": "rate",
          "type": "Rate",
          "description": "Returns the rate of change for the data points"
        }
      ]
    }
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https://time-series-service-doc.grc-apps.svc.ice.ge.com//
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/availability/master/_listings/predix/v1aggregations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/availability/master/_listings/predix/v1aggregations-get-openapi.md
- name: Data Services - Get all available aggregations
  x-api-slug: v1aggregations-get
  description: |-
    Return all supported aggregations.Response JSON (Status 200){
      "results": [
        {
          "name": "max",
          "type": "Maximum",
          "description": "Returns the maximum value data point for the time range"
        },
        {
          "name": "trendmode",
          "type": "Trend Mode",
          "description": "Returns the maximum and minimum value data point for the time range"
        },
        {
          "name": "count",
          "type": "Count",
          "description": "Returns the number of data points"
        },
        {
          "name": "scale",
          "type": "Scale",
          "description": "Scales each data point by a factor"
        },
        {
          "name": "interpolate",
          "type": "Interpolate",
          "description": "Does linear interpolation for the chosen window"
        },
        {
          "name": "sum",
          "type": "Sum",
          "description": "Adds the data points together"
        },
        {
          "name": "diff",
          "type": "Difference",
          "description": "Returns the difference between successive data points"
        },
        {
          "name": "gaps",
          "type": "Gaps",
          "description": "Marks gaps in data according to sampling rate with a null data point"
        },
        {
          "name": "sampler",
          "type": "Sampler",
          "description": "Returns the sampling rate of change for the data points"
        },
        {
          "name": "div",
          "type": "Divide",
          "description": "Divides each data point by a divisor"
        },
        {
          "name": "min",
          "type": "Minimum",
          "description": "Returns the minimum value data point for the time range"
        },
        {
          "name": "avg",
          "type": "Average",
          "description": "Returns the average of the data point set"
        },
        {
          "name": "least_squares",
          "type": "Least Squares",
          "description": "Returns a best fit line through the data points using the least squares algorithm"
        },
        {
          "name": "percentile",
          "type": "Percentile",
          "description": "Returns the percentile of the data range"
        },
        {
          "name": "dev",
          "type": "Standard Deviation",
          "description": "Returns the standard deviation of the time series"
        },
        {
          "name": "rate",
          "type": "Rate",
          "description": "Returns the rate of change for the data points"
        }
      ]
    }
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https://time-series-service-doc.grc-apps.svc.ice.ge.com//
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/availability/master/_listings/predix/v1aggregations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/availability/master/_listings/predix/v1aggregations-get-openapi.md
- name: Data Services - Get all available aggregations
  x-api-slug: v1aggregations-get
  description: |-
    Return all supported aggregations.Response JSON (Status 200){
      "results": [
        {
          "name": "max",
          "type": "Maximum",
          "description": "Returns the maximum value data point for the time range"
        },
        {
          "name": "trendmode",
          "type": "Trend Mode",
          "description": "Returns the maximum and minimum value data point for the time range"
        },
        {
          "name": "count",
          "type": "Count",
          "description": "Returns the number of data points"
        },
        {
          "name": "scale",
          "type": "Scale",
          "description": "Scales each data point by a factor"
        },
        {
          "name": "interpolate",
          "type": "Interpolate",
          "description": "Does linear interpolation for the chosen window"
        },
        {
          "name": "sum",
          "type": "Sum",
          "description": "Adds the data points together"
        },
        {
          "name": "diff",
          "type": "Difference",
          "description": "Returns the difference between successive data points"
        },
        {
          "name": "gaps",
          "type": "Gaps",
          "description": "Marks gaps in data according to sampling rate with a null data point"
        },
        {
          "name": "sampler",
          "type": "Sampler",
          "description": "Returns the sampling rate of change for the data points"
        },
        {
          "name": "div",
          "type": "Divide",
          "description": "Divides each data point by a divisor"
        },
        {
          "name": "min",
          "type": "Minimum",
          "description": "Returns the minimum value data point for the time range"
        },
        {
          "name": "avg",
          "type": "Average",
          "description": "Returns the average of the data point set"
        },
        {
          "name": "least_squares",
          "type": "Least Squares",
          "description": "Returns a best fit line through the data points using the least squares algorithm"
        },
        {
          "name": "percentile",
          "type": "Percentile",
          "description": "Returns the percentile of the data range"
        },
        {
          "name": "dev",
          "type": "Standard Deviation",
          "description": "Returns the standard deviation of the time series"
        },
        {
          "name": "rate",
          "type": "Rate",
          "description": "Returns the rate of change for the data points"
        }
      ]
    }
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https://time-series-service-doc.grc-apps.svc.ice.ge.com//
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/availability/master/_listings/predix/v1aggregations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/availability/master/_listings/predix/v1aggregations-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://predicthq.api.gallery.streamdata.io
- type: x-api-stack
  url: http://predix.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/predix
- type: x-documentation
  url: https://docs.predix.io/en-US/platform
- type: x-twitter
  url: https://twitter.com/Predix
- type: x-website
  url: https://www.predix.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---