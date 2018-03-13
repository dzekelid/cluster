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
  /?Action=ModifyDBCluster&k=1:
    get:
      summary: Modify D B Cluster
      description: Modify a setting for an Amazon Aurora DB cluster
      operationId: modifydbcluster
      parameters:
      - in: query
        name: ApplyImmediately
        description: A value that specifies whether the modifications in this request
          and      any pending modifications are asynchronously applied      as soon
          as possible, regardless of the      PreferredMaintenanceWindow setting for
          the DB cluster
        type: string
      - in: query
        name: BackupRetentionPeriod
        description: The number of days for which automated backups are retained
        type: string
      - in: query
        name: DBClusterIdentifier
        description: The DB cluster identifier for the cluster being modified
        type: string
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to use for the DB
          cluster
        type: string
      - in: query
        name: MasterUserPassword
        description: The new password for the master database user
        type: string
      - in: query
        name: NewDBClusterIdentifier
        description: The new DB cluster identifier for the DB cluster when renaming
          a DB cluster
        type: string
      - in: query
        name: OptionGroupName
        description: A value that indicates that the DB cluster should be associated
          with the specified option group
        type: string
      - in: query
        name: Port
        description: The port number on which the DB cluster accepts connections
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created            if
          automated backups are enabled,            using the BackupRetentionPeriod
          parameter
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range during which system maintenance can occur,
          in Universal Coordinated Time (UTC)
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A lst of VPC security groups that the DB cluster will belong
          to
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