swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 1
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
  /?Action=AddRoleToDBCluster:
    get:
      summary: Add Role To D B Cluster
      description: Associates an Identity and Access Management (IAM) role from an
        Aurora DB cluster.
      operationId: addroletodbcluster
      x-api-path-slug: actionaddroletodbcluster-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The name of the DB cluster to associate the IAM role with
        type: string
      - in: query
        name: RoleArn
        description: The Amazon Resource Name (ARN) of the IAM role to associate with
          the Aurora DB cluster, for example            arn:aws:iam::123456789012:role/AuroraAccessRole
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=CopyDBClusterParameterGroup:
    get:
      summary: Copy D B Cluster Parameter Group
      description: Copies the specified DB cluster parameter group.
      operationId: copydbclusterparametergroup
      x-api-path-slug: actioncopydbclusterparametergroup-get
      parameters:
      - in: query
        name: SourceDBClusterParameterGroupIdentifier
        description: The identifier or Amazon Resource Name (ARN) for the source DB
          cluster parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetDBClusterParameterGroupDescription
        description: A description for the copied DB cluster parameter group
        type: string
      - in: query
        name: TargetDBClusterParameterGroupIdentifier
        description: The identifier for the copied DB cluster parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=CopyDBClusterSnapshot:
    get:
      summary: Copy D B Cluster Snapshot
      description: Creates a snapshot of a DB cluster.
      operationId: copydbclustersnapshot
      x-api-path-slug: actioncopydbclustersnapshot-get
      parameters:
      - in: query
        name: SourceDBClusterSnapshotIdentifier
        description: The identifier of the DB cluster snapshot to copy
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetDBClusterSnapshotIdentifier
        description: The identifier of the new DB cluster snapshot to create from
          the source DB cluster snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=CreateDBCluster:
    get:
      summary: Create D B Cluster
      description: Creates a new Amazon Aurora DB cluster.
      operationId: createdbcluster
      x-api-path-slug: actioncreatedbcluster-get
      parameters:
      - in: query
        name: AvailabilityZones.AvailabilityZone.N
        description: A list of EC2 Availability Zones that instances in the DB cluster
          can be created in
        type: string
      - in: query
        name: BackupRetentionPeriod
        description: The number of days for which automated backups are retained
        type: string
      - in: query
        name: CharacterSetName
        description: A value that indicates that the DB cluster should be associated
          with the specified CharacterSet
        type: string
      - in: query
        name: DatabaseName
        description: The name for your database of up to 8 alpha-numeric characters
        type: string
      - in: query
        name: DBClusterIdentifier
        description: The DB cluster identifier
        type: string
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to associate            with
          this DB cluster
        type: string
      - in: query
        name: DBSubnetGroupName
        description: A DB subnet group to associate with this DB cluster
        type: string
      - in: query
        name: Engine
        description: The name of the database engine to be used for this DB cluster
        type: string
      - in: query
        name: EngineVersion
        description: The version number of the database engine to use
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier for an encrypted DB cluster
        type: string
      - in: query
        name: MasterUsername
        description: The name of the master user for the DB cluster
        type: string
      - in: query
        name: MasterUserPassword
        description: The password for the master database user
        type: string
      - in: query
        name: OptionGroupName
        description: A value that indicates that the DB cluster should be associated
          with the specified option group
        type: string
      - in: query
        name: Port
        description: The port number on which the instances in the DB cluster accept
          connections
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created        if
          automated backups are enabled        using the BackupRetentionPeriod parameter
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range during which system maintenance can occur,
          in Universal Coordinated Time (UTC)
        type: string
      - in: query
        name: ReplicationSourceIdentifier
        description: The Amazon Resource Name (ARN) of the source DB cluster if this
          DB cluster is created as a Read Replica
        type: string
      - in: query
        name: StorageEncrypted
        description: Specifies whether the DB cluster is encrypted
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of EC2 VPC security groups to associate with this DB cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=CreateDBClusterParameterGroup:
    get:
      summary: Create D B Cluster Parameter Group
      description: Creates a new DB cluster parameter group.
      operationId: createdbclusterparametergroup
      x-api-path-slug: actioncreatedbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group
        type: string
      - in: query
        name: DBParameterGroupFamily
        description: The DB cluster parameter group family name
        type: string
      - in: query
        name: Description
        description: The description for the DB cluster parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=CreateDBClusterSnapshot:
    get:
      summary: Create D B Cluster Snapshot
      description: Creates a snapshot of a DB cluster.
      operationId: createdbclustersnapshot
      x-api-path-slug: actioncreatedbclustersnapshot-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The identifier of the DB cluster to create a snapshot for
        type: string
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier of the DB cluster snapshot
        type: string
      - in: query
        name: Tags.Tag.N
        description: The tags to be assigned to the DB cluster snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=DeleteDBCluster:
    get:
      summary: Delete D B Cluster
      description: The DeleteDBCluster action deletes a previously provisioned DB
        cluster.
      operationId: deletedbcluster
      x-api-path-slug: actiondeletedbcluster-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The DB cluster identifier for the DB cluster to be deleted
        type: string
      - in: query
        name: FinalDBSnapshotIdentifier
        description: The DB cluster snapshot identifier of the new DB cluster snapshot
          created when SkipFinalSnapshot      is set to false
        type: string
      - in: query
        name: SkipFinalSnapshot
        description: Determines whether a final DB cluster snapshot is created before
          the DB cluster is deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DeleteDBClusterParameterGroup:
    get:
      summary: Delete D B Cluster Parameter Group
      description: Deletes a specified DB cluster parameter group.
      operationId: deletedbclusterparametergroup
      x-api-path-slug: actiondeletedbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DeleteDBClusterSnapshot:
    get:
      summary: Delete D B Cluster Snapshot
      description: Deletes a DB cluster snapshot.
      operationId: deletedbclustersnapshot
      x-api-path-slug: actiondeletedbclustersnapshot-get
      parameters:
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier of the DB cluster snapshot to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=DescribeDBClusterParameterGroups:
    get:
      summary: Describe D B Cluster Parameter Groups
      description: Returns a list of DBClusterParameterGroup descriptions.
      operationId: describedbclusterparametergroups
      x-api-path-slug: actiondescribedbclusterparametergroups-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of a specific DB cluster parameter group to return details
          for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBClusterParameterGroups
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DescribeDBClusterParameters:
    get:
      summary: Describe D B Cluster Parameters
      description: Returns the detailed parameter list for a particular DB cluster
        parameter group.
      operationId: describedbclusterparameters
      x-api-path-slug: actiondescribedbclusterparameters-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of a specific DB cluster parameter group to return parameter
          details for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      DescribeDBClusterParameters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: Source
        description: A value that indicates to return only parameters for a specific
          source
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameters
  /?Action=DescribeDBClusters:
    get:
      summary: Describe D B Clusters
      description: Returns information about provisioned Aurora DB clusters.
      operationId: describedbclusters
      x-api-path-slug: actiondescribedbclusters-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The user-supplied DB cluster identifier
        type: string
      - in: query
        name: Filters.Filter.N
        description: A filter that specifies one or more DB clusters to describe
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribeDBClusters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeDBClusterSnapshotAttributes:
    get:
      summary: Describe D B Cluster Snapshot Attributes
      description: Returns a list of DB cluster snapshot attribute names and values
        for a manual DB cluster snapshot.
      operationId: describedbclustersnapshotattributes
      x-api-path-slug: actiondescribedbclustersnapshotattributes-get
      parameters:
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier for the DB cluster snapshot to describe the attributes
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=DescribeDBClusterSnapshots:
    get:
      summary: Describe D B Cluster Snapshots
      description: Returns information about DB cluster snapshots.
      operationId: describedbclustersnapshots
      x-api-path-slug: actiondescribedbclustersnapshots-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The ID of the DB cluster to retrieve the list of DB cluster snapshots
          for
        type: string
      - in: query
        name: DBClusterSnapshotIdentifier
        description: A specific DB cluster snapshot identifier to describe
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: IncludePublic
        description: Set this value to true to include manual DB cluster snapshots
          that are public and can be copied             or restored by any AWS account,
          otherwise set this value to false
        type: string
      - in: query
        name: IncludeShared
        description: Set this value to true to include shared manual DB cluster snapshots             from
          other AWS accounts that this AWS account has been given             permission
          to copy or restore, otherwise set this value to false
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribeDBClusterSnapshots
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: SnapshotType
        description: The type of DB cluster snapshots to be returned
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=DescribeEngineDefaultClusterParameters:
    get:
      summary: Describe Engine Default Cluster Parameters
      description: Returns the default engine and system parameter information for
        the cluster database engine.
      operationId: describeenginedefaultclusterparameters
      x-api-path-slug: actiondescribeenginedefaultclusterparameters-get
      parameters:
      - in: query
        name: DBParameterGroupFamily
        description: The name of the DB cluster parameter group family to return engine
          parameter information for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      DescribeEngineDefaultClusterParameters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Default Cluster Parameters
  /?Action=FailoverDBCluster:
    get:
      summary: Failover D B Cluster
      description: Forces a failover for a DB cluster.
      operationId: failoverdbcluster
      x-api-path-slug: actionfailoverdbcluster-get
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
      - Clusters
  /?Action=ModifyDBCluster:
    get:
      summary: Modify D B Cluster
      description: Modify a setting for an Amazon Aurora DB cluster.
      operationId: modifydbcluster
      x-api-path-slug: actionmodifydbcluster-get
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
      - Clusters
  /?Action=ModifyDBClusterParameterGroup:
    get:
      summary: Modify D B Cluster Parameter Group
      description: Modifies the parameters of a DB cluster parameter group.
      operationId: modifydbclusterparametergroup
      x-api-path-slug: actionmodifydbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to modify
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: A list of parameters in the DB cluster parameter group to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=ModifyDBClusterSnapshotAttribute:
    get:
      summary: Modify D B Cluster Snapshot Attribute
      description: Adds an attribute and values to, or removes an attribute and values
        from, a manual DB cluster snapshot.
      operationId: modifydbclustersnapshotattribute
      x-api-path-slug: actionmodifydbclustersnapshotattribute-get
      parameters:
      - in: query
        name: AttributeName
        description: The name of the DB cluster snapshot attribute to modify
        type: string
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier for the DB cluster snapshot to modify the attributes
          for
        type: string
      - in: query
        name: ValuesToAdd.AttributeValue.N
        description: A list of DB cluster snapshot attributes to add to the attribute
          specified by AttributeName
        type: string
      - in: query
        name: ValuesToRemove.AttributeValue.N
        description: A list of DB cluster snapshot attributes to remove from the attribute
          specified by AttributeName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=PromoteReadReplicaDBCluster:
    get:
      summary: Promote Read Replica D B Cluster
      description: Promotes a Read Replica DB cluster to a standalone DB cluster.
      operationId: promotereadreplicadbcluster
      x-api-path-slug: actionpromotereadreplicadbcluster-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The identifier of the DB cluster Read Replica to promote
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replicas
  /?Action=RemoveRoleFromDBCluster:
    get:
      summary: Remove Role From D B Cluster
      description: Disassociates an Identity and Access Management (IAM) role from
        an Aurora DB cluster.
      operationId: removerolefromdbcluster
      x-api-path-slug: actionremoverolefromdbcluster-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The name of the DB cluster to disassociate the IAM role rom
        type: string
      - in: query
        name: RoleArn
        description: The Amazon Resource Name (ARN) of the IAM role to disassociate
          from the Aurora DB cluster, for example        arn:aws:iam::123456789012:role/AuroraAccessRole
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ResetDBClusterParameterGroup:
    get:
      summary: Reset D B Cluster Parameter Group
      description: Modifies the parameters of a DB cluster parameter group to the
        default value.
      operationId: resetdbclusterparametergroup
      x-api-path-slug: actionresetdbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to reset
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: A list of parameter names in the DB cluster parameter group to
          reset to the default values
        type: string
      - in: query
        name: ResetAllParameters
        description: A value that is set to true to reset all parameters in the DB
          cluster parameter group       to their default values, and false otherwise
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=RestoreDBClusterFromS3:
    get:
      summary: Restore D B Cluster From S3
      description: Creates an Amazon Aurora DB cluster from data stored in an Amazon
        S3 bucket.
      operationId: restoredbclusterfroms3
      x-api-path-slug: actionrestoredbclusterfroms3-get
      parameters:
      - in: query
        name: AvailabilityZones.AvailabilityZone.N
        description: A list of EC2 Availability Zones that instances in the restored
          DB cluster can be created in
        type: string
      - in: query
        name: BackupRetentionPeriod
        description: The number of days for which automated backups of the restored
          DB cluster are retained
        type: string
      - in: query
        name: CharacterSetName
        description: A value that indicates that the restored DB cluster should be
          associated with the specified CharacterSet
        type: string
      - in: query
        name: DatabaseName
        description: The database name for the restored DB cluster
        type: string
      - in: query
        name: DBClusterIdentifier
        description: The name of the DB cluster to create from the source data in
          the S3 bucket
        type: string
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to associate            with
          the restored DB cluster
        type: string
      - in: query
        name: DBSubnetGroupName
        description: A DB subnet group to associate with the restored DB cluster
        type: string
      - in: query
        name: Engine
        description: The name of the database engine to be used for the restored DB
          cluster
        type: string
      - in: query
        name: EngineVersion
        description: The version number of the database engine to use
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier for an encrypted DB cluster
        type: string
      - in: query
        name: MasterUsername
        description: The name of the master user for the restored DB cluster
        type: string
      - in: query
        name: MasterUserPassword
        description: The password for the master database user
        type: string
      - in: query
        name: OptionGroupName
        description: A value that indicates that the restored DB cluster should be
          associated with the specified option group
        type: string
      - in: query
        name: Port
        description: The port number on which the instances in the restored DB cluster
          accept connections
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created            if
          automated backups are enabled            using the BackupRetentionPeriod
          parameter
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range during which system maintenance can occur,
          in Universal Coordinated Time (UTC)
        type: string
      - in: query
        name: S3BucketName
        description: The name of the Amazon S3 bucket that contains the data used
          to create the Amazon Aurora DB cluster
        type: string
      - in: query
        name: S3IngestionRoleArn
        description: The Amazon Resource Name (ARN) of the AWS Identity and Access
          Management (IAM) role that authorizes        Amazon RDS to access the Amazon
          S3 bucket on your behalf
        type: string
      - in: query
        name: S3Prefix
        description: The prefix for all of the file names that contain the data used
          to create the Amazon Aurora DB cluster
        type: string
      - in: query
        name: SourceEngine
        description: The identifier for the database engine that was backed up to
          create the files stored in the            Amazon S3 bucket
        type: string
      - in: query
        name: SourceEngineVersion
        description: The version of the database that the backup files were created
          from
        type: string
      - in: query
        name: StorageEncrypted
        description: Specifies whether the restored DB cluster is encrypted
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of EC2 VPC security groups to associate with the restored
          DB cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=RestoreDBClusterFromSnapshot:
    get:
      summary: Restore D B Cluster From Snapshot
      description: Creates a new DB cluster from a DB cluster snapshot.
      operationId: restoredbclusterfromsnapshot
      x-api-path-slug: actionrestoredbclusterfromsnapshot-get
      parameters:
      - in: query
        name: AvailabilityZones.AvailabilityZone.N
        description: Provides the list of EC2 Availability Zones that instances in
          the restored DB cluster can be created in
        type: string
      - in: query
        name: DatabaseName
        description: The database name for the restored DB cluster
        type: string
      - in: query
        name: DBClusterIdentifier
        description: The name of the DB cluster to create from the DB cluster snapshot
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The name of the DB subnet group to use for the new DB cluster
        type: string
      - in: query
        name: Engine
        description: The database engine to use for the new DB cluster
        type: string
      - in: query
        name: EngineVersion
        description: The version of the database engine to use for the new DB cluster
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier to use when restoring an encrypted DB
          cluster from a DB cluster snapshot
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group to use for the restored DB cluster
        type: string
      - in: query
        name: Port
        description: The port number on which the new DB cluster accepts connections
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The identifier for the DB cluster snapshot to restore from
        type: string
      - in: query
        name: Tags.Tag.N
        description: The tags to be assigned to the restored DB cluster
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of VPC security groups that the new DB cluster will belong
          to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=RestoreDBClusterToPointInTime:
    get:
      summary: Restore D B Cluster To Point In Time
      description: Restores a DB cluster to an arbitrary point in time.
      operationId: restoredbclustertopointintime
      x-api-path-slug: actionrestoredbclustertopointintime-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The name of the new DB cluster to be created
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The DB subnet group name to use for the new DB cluster
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier to use when restoring an encrypted DB
          cluster from an encrypted DB cluster
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group for the new DB cluster
        type: string
      - in: query
        name: Port
        description: The port number on which the new DB cluster accepts connections
        type: string
      - in: query
        name: RestoreToTime
        description: The date and time to restore the DB cluster to
        type: string
      - in: query
        name: SourceDBClusterIdentifier
        description: The identifier of the source DB cluster from which to restore
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: UseLatestRestorableTime
        description: A value that is set to true to restore the DB cluster to the
          latest       restorable backup time, and false otherwise
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A lst of VPC security groups that the new DB cluster belongs
          to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters