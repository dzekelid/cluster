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
  /?Action=DeleteDBClusterSnapshot&k=1:
    get:
      summary: Delete D B Cluster Snapshot
      description: Deletes a DB cluster snapshot
      operationId: deletedbclustersnapshot
      parameters:
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier of the DB cluster snapshot to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - cluster snapshots
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