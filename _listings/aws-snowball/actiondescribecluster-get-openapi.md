---
swagger: "2.0"
x-collection-name: AWS Snowball
x-complete: 0
info:
  title: AWS Snowball API Describe Cluster
  version: 1.0.0
  description: |-
    Returns information about a specific cluster including shipping information, cluster
          status, and other important metadata.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---