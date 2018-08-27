swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateVolume:
    get:
      summary: Create Volume
      description: Creates an EBS volume that can be attached to an instance in the
        same Availability Zone.
      operationId: createvolume
      x-api-path-slug: actioncreatevolume-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the EBS snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volume
  /?Action=DescribeAvailabilityZones:
    get:
      summary: Describe Availability Zones
      description: Describes one or more of the Availability Zones that are available
        to you.
      operationId: describeavailabilityzones
      x-api-path-slug: actiondescribeavailabilityzones-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: RegionName.N
        description: The names of one or more regions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Availability Zones
  /?Action=DescribeScheduledInstanceAvailability:
    get:
      summary: Describe Scheduled Instance Availability
      description: Finds available schedules that meet the specified criteria.
      operationId: describescheduledinstanceavailability
      x-api-path-slug: actiondescribescheduledinstanceavailability-get
      responses:
        200:
          description: OK
      tags:
      - Server Instance Availability
  /?Action=ModifyReservedInstances:
    get:
      summary: Modify Reserved Instances
      description: Modifies the Availability Zone, instance count, instance type,
        or network platform (EC2-Classic or EC2-VPC) of your Standard Reserved Instances.
      operationId: modifyreservedinstances
      x-api-path-slug: actionmodifyreservedinstances-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceCount
        description: The number of Reserved Instances to purchase
        type: string
      - in: query
        name: LimitPrice
        description: Specified for Reserved Instance Marketplace offerings to limit
          the total order and ensure that the Reserved Instances are not purchased
          at unexpected prices
        type: string
      - in: query
        name: ReservedInstancesOfferingId
        description: The ID of the Reserved Instance offering to purchase
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instance