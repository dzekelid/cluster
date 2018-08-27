swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeregisterEcsCluster:
    get:
      summary: Deregister Ecs Cluster
      description: Deregisters a specified Amazon ECS cluster from a stack.
      operationId: deregisterEcsCluster
      x-api-path-slug: actionderegisterecscluster-get
      parameters:
      - in: query
        name: EcsClusterArn
        description: The clusters ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Ecs
      - Cluster
  /?Action=RegisterEcsCluster:
    get:
      summary: Register Ecs Cluster
      description: Registers a specified Amazon ECS cluster with a stack.
      operationId: registerEcsCluster
      x-api-path-slug: actionregisterecscluster-get
      parameters:
      - in: query
        name: EcsClusterArn
        description: The clusters ARN
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Ecs
      - Cluster
  /?Action=DescribeEcsClusters:
    get:
      summary: Describe Ecs Clusters
      description: Describes Amazon ECS clusters that are registered with a stack.
      operationId: describeEcsClusters
      x-api-path-slug: actiondescribeecsclusters-get
      parameters:
      - in: query
        name: EcsClusterArns
        description: A list of ARNs, one for each cluster to be described
        type: string
      - in: query
        name: MaxResults
        description: To receive a paginated response, use this parameter to specify
          the maximum number      of results to be returned with a single call
        type: string
      - in: query
        name: NextToken
        description: If the previous paginated request did not return all of the remaining
          results,      the response objectsNextToken parameter value is set to a
          token
        type: string
      - in: query
        name: StackId
        description: A stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Ecs
      - Clusters