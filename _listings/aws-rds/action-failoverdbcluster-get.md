---
swagger: "2.0"
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=FailoverDBCluster&k=1:
    get:
      summary: Failover D B Cluster
      description: Forces a failover for a DB cluster
      operationId: failoverdbcluster
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: A DB cluster identifier to force a failover for
        type: string
      - in: query
        name: TargetDBInstanceIdentifier
        description: The name of the instance to promote to the primary instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - clusters
definitions: []
x-collection-name: AWS RDS
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