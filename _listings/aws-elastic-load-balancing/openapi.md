swagger: "2.0"
x-collection-name: AWS Elastic Load Balancing
x-complete: 1
info:
  title: AWS Elastic Load Balancing API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SetSubnets:
    get:
      summary: Set Subnets
      description: Enables the Availability Zone for the specified subnets for the
        specified load balancer.
      operationId: setSubnets
      x-api-path-slug: actionsetsubnets-get
      parameters:
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      - in: query
        name: Subnets.member.N
        description: The IDs of the subnets
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnets