---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 1
info:
  title: AWS EC2 Container Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateCluster:
    get:
      summary: Create Cluster
      description: Creates a new Amazon ECS cluster.
      operationId: createCluster
      x-api-path-slug: actioncreatecluster-get
      parameters:
      - in: query
        name: clusterName
        description: The name of your cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DeleteCluster:
    get:
      summary: Delete Cluster
      description: Deletes the specified cluster.
      operationId: deleteCluster
      x-api-path-slug: actiondeletecluster-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeClusters:
    get:
      summary: Describe Clusters
      description: Describes one or more of your clusters.
      operationId: describeClusters
      x-api-path-slug: actiondescribeclusters-get
      parameters:
      - in: query
        name: clusters
        description: A space-separated list of up to 100 cluster names or full cluster
          Amazon Resource Name (ARN)            entries
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ListClusters:
    get:
      summary: List Clusters
      description: Returns a list of existing clusters.
      operationId: listClusters
      x-api-path-slug: actionlistclusters-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of cluster results returned by ListClusters
          in            paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListClusters
          request where maxResults was used and the            results exceeded the
          value of that parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
---