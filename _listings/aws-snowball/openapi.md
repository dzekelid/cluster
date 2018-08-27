swagger: "2.0"
x-collection-name: AWS Snowball
x-complete: 1
info:
  title: AWS Snowball API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelCluster:
    get:
      summary: Cancel Cluster
      description: Cancels a cluster job.
      operationId: cancelCluster
      x-api-path-slug: actioncancelcluster-get
      parameters:
      - in: query
        name: ClusterId
        description: The 39-character ID for the cluster that you want to cancel,
          for example        CID123e4567-e89b-12d3-a456-426655440000
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=CreateCluster:
    get:
      summary: Create Cluster
      description: Creates an empty cluster.
      operationId: createCluster
      x-api-path-slug: actioncreatecluster-get
      parameters:
      - in: query
        name: AddressId
        description: The ID for the address that you want the cluster shipped to
        type: string
      - in: query
        name: Description
        description: An optional description of this specific cluster, for example
          Environmental Data        Cluster-01
        type: string
      - in: query
        name: JobType
        description: The type of job for this cluster
        type: string
      - in: query
        name: KmsKeyARN
        description: The KmsKeyARN value that you want to associate with this cluster
        type: string
      - in: query
        name: Notification
        description: The Amazon Simple Notification Service (Amazon SNS) notification
          settings for this      cluster
        type: string
      - in: query
        name: Resources
        description: The resources associated with the cluster job
        type: string
      - in: query
        name: RoleARN
        description: The RoleARN that you want to associate with this cluster
        type: string
      - in: query
        name: ShippingOption
        description: The shipping speed for each node in this cluster
        type: string
      - in: query
        name: SnowballType
        description: The type of AWS Snowball appliance to use for this cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeCluster:
    get:
      summary: Describe Cluster
      description: |-
        Returns information about a specific cluster including shipping information, cluster
              status, and other important metadata.
      operationId: describeCluster
      x-api-path-slug: actiondescribecluster-get
      parameters:
      - in: query
        name: ClusterId
        description: The automatically generated ID for a cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ListClusterJobs:
    get:
      summary: List Cluster Jobs
      description: Returns an array of JobListEntry objects of the specified length.
      operationId: listClusterJobs
      x-api-path-slug: actionlistclusterjobs-get
      parameters:
      - in: query
        name: ClusterId
        description: The 39-character ID for the cluster that you want to list, for
          example        CID123e4567-e89b-12d3-a456-426655440000
        type: string
      - in: query
        name: MaxResults
        description: The number of JobListEntry objects to return
        type: string
      - in: query
        name: NextToken
        description: HTTP requests are stateless
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Jobs
  /?Action=ListClusters:
    get:
      summary: List Clusters
      description: Returns an array of ClusterListEntry objects of the specified length.
      operationId: listClusters
      x-api-path-slug: actionlistclusters-get
      parameters:
      - in: query
        name: MaxResults
        description: The number of ClusterListEntry objects to return
        type: string
      - in: query
        name: NextToken
        description: HTTP requests are stateless
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=UpdateCluster:
    get:
      summary: Update Cluster
      description: |-
        While a cluster's ClusterState value is in the AwaitingQuorum
              state, you can update some of the information associated with a cluster.
      operationId: updateCluster
      x-api-path-slug: actionupdatecluster-get
      parameters:
      - in: query
        name: AddressId
        description: The ID of the updated Address object
        type: string
      - in: query
        name: ClusterId
        description: The cluster ID of the cluster that you want to update, for example        CID123e4567-e89b-12d3-a456-426655440000
        type: string
      - in: query
        name: Description
        description: The updated description of this cluster
        type: string
      - in: query
        name: Notification
        description: The new or updated Notification object
        type: string
      - in: query
        name: Resources
        description: The updated arrays of JobResource objects that can include updated        S3Resource
          objects or LambdaResource objects
        type: string
      - in: query
        name: RoleARN
        description: The new role Amazon Resource Name (ARN) that you want to associate
          with this cluster
        type: string
      - in: query
        name: ShippingOption
        description: The updated shipping option value of this clusters ShippingDetails      object
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters