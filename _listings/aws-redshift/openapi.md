---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 1
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AuthorizeClusterSecurityGroupIngress:
    get:
      summary: Authorize Cluster Security Group Ingress
      description: Adds an inbound (ingress) rule to an Amazon Redshift security group.
      operationId: authorizeClusterSecurityGroupIngress
      x-api-path-slug: actionauthorizeclustersecuritygroupingress-get
      parameters:
      - in: query
        name: CIDRIP
        description: The IP range to be added the Amazon Redshift security group
        type: string
      - in: query
        name: ClusterSecurityGroupName
        description: The name of the security group to which the ingress rule is added
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The EC2 security group to be added the Amazon Redshift security
          group
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS account number of the owner of the security group specified
          by the                EC2SecurityGroupName parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=CopyClusterSnapshot:
    get:
      summary: Copy Cluster Snapshot
      description: Copies the specified automated cluster snapshot to a new manual
        cluster snapshot.
      operationId: copyClusterSnapshot
      x-api-path-slug: actioncopyclustersnapshot-get
      parameters:
      - in: query
        name: SourceSnapshotClusterIdentifier
        description: The identifier of the cluster the source snapshot was created
          from
        type: string
      - in: query
        name: SourceSnapshotIdentifier
        description: The identifier for the source snapshot
        type: string
      - in: query
        name: TargetSnapshotIdentifier
        description: The identifier given to the new manual snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateCluster:
    get:
      summary: Create Cluster
      description: Creates a new cluster.
      operationId: createCluster
      x-api-path-slug: actioncreatecluster-get
      parameters:
      - in: query
        name: AdditionalInfo
        description: Reserved
        type: string
      - in: query
        name: AllowVersionUpgrade
        description: If true, major version upgrades can be applied during the maintenance            window
          to the Amazon Redshift engine that is running on the cluster
        type: string
      - in: query
        name: AutomatedSnapshotRetentionPeriod
        description: The number of days that automated snapshots are retained
        type: string
      - in: query
        name: AvailabilityZone
        description: The EC2 Availability Zone (AZ) in which you want Amazon Redshift
          to provision the            cluster
        type: string
      - in: query
        name: ClusterIdentifier
        description: A unique identifier for the cluster
        type: string
      - in: query
        name: ClusterParameterGroupName
        description: The name of the parameter group to be associated with this cluster
        type: string
      - in: query
        name: ClusterSecurityGroups.ClusterSecurityGroupName.N
        description: A list of security groups to be associated with this cluster
        type: string
      - in: query
        name: ClusterSubnetGroupName
        description: The name of a cluster subnet group to be associated with this
          cluster
        type: string
      - in: query
        name: ClusterType
        description: The type of the cluster
        type: string
      - in: query
        name: ClusterVersion
        description: The version of the Amazon Redshift engine software that you want
          to deploy on the            cluster
        type: string
      - in: query
        name: DBName
        description: The name of the first database to be created when the cluster
          is created
        type: string
      - in: query
        name: ElasticIp
        description: The Elastic IP (EIP) address for the cluster
        type: string
      - in: query
        name: Encrypted
        description: If true, the data in the cluster is encrypted at rest
        type: string
      - in: query
        name: EnhancedVpcRouting
        description: An option that specifies whether to create the cluster with enhanced
          VPC routing            enabled
        type: string
      - in: query
        name: HsmClientCertificateIdentifier
        description: Specifies the name of the HSM client certificate the Amazon Redshift
          cluster uses to           retrieve the data encryption keys stored in an
          HSM
        type: string
      - in: query
        name: HsmConfigurationIdentifier
        description: Specifies the name of the HSM configuration that contains the
          information the            Amazon Redshift cluster can use to retrieve and
          store keys in an HSM
        type: string
      - in: query
        name: IamRoles.IamRoleArn.N
        description: A list of AWS Identity and Access Management (IAM) roles that
          can be used by the            cluster to access other AWS services
        type: string
      - in: query
        name: KmsKeyId
        description: The AWS Key Management Service (KMS) key ID of the encryption
          key that you want to            use to encrypt data in the cluster
        type: string
      - in: query
        name: MasterUsername
        description: The user name associated with the master user account for the
          cluster that is being            created
        type: string
      - in: query
        name: MasterUserPassword
        description: The password associated with the master user account for the
          cluster that is being            created
        type: string
      - in: query
        name: NodeType
        description: The node type to be provisioned for the cluster
        type: string
      - in: query
        name: NumberOfNodes
        description: The number of compute nodes in the cluster
        type: string
      - in: query
        name: Port
        description: The port number on which the cluster accepts incoming connections
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range (in UTC) during which automated cluster
          maintenance can            occur
        type: string
      - in: query
        name: PubliclyAccessible
        description: If true, the cluster can be accessed from a public network
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of Virtual Private Cloud (VPC) security groups to be associated
          with the            cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=CreateClusterParameterGroup:
    get:
      summary: Create Cluster Parameter Group
      description: Creates an Amazon Redshift parameter group.
      operationId: createClusterParameterGroup
      x-api-path-slug: actioncreateclusterparametergroup-get
      parameters:
      - in: query
        name: Description
        description: A description of the parameter group
        type: string
      - in: query
        name: ParameterGroupFamily
        description: The Amazon Redshift engine version to which the cluster parameter
          group applies
        type: string
      - in: query
        name: ParameterGroupName
        description: The name of the cluster parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=CreateClusterSecurityGroup:
    get:
      summary: Create Cluster Security Group
      description: Creates a new Amazon Redshift security group.
      operationId: createClusterSecurityGroup
      x-api-path-slug: actioncreateclustersecuritygroup-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name for the security group
        type: string
      - in: query
        name: Description
        description: A description for the security group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=CreateClusterSnapshot:
    get:
      summary: Create Cluster Snapshot
      description: Creates a manual snapshot of the specified cluster.
      operationId: createClusterSnapshot
      x-api-path-slug: actioncreateclustersnapshot-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The cluster identifier for which you want a snapshot
        type: string
      - in: query
        name: SnapshotIdentifier
        description: A unique identifier for the snapshot that you are requesting
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateClusterSubnetGroup:
    get:
      summary: Create Cluster Subnet Group
      description: Creates a new Amazon Redshift subnet group.
      operationId: createClusterSubnetGroup
      x-api-path-slug: actioncreateclustersubnetgroup-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name for the subnet group
        type: string
      - in: query
        name: Description
        description: A description for the subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: An array of VPC subnet IDs
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=DeleteCluster:
    get:
      summary: Delete Cluster
      description: Deletes a previously provisioned cluster.
      operationId: deleteCluster
      x-api-path-slug: actiondeletecluster-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster to be deleted
        type: string
      - in: query
        name: FinalClusterSnapshotIdentifier
        description: The identifier of the final snapshot that is to be created immediately
          before            deleting the cluster
        type: string
      - in: query
        name: SkipFinalClusterSnapshot
        description: Determines whether a final snapshot of the cluster is created
          before Amazon Redshift            deletes the cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DeleteClusterParameterGroup:
    get:
      summary: Delete Cluster Parameter Group
      description: Deletes a specified Amazon Redshift parameter group.
      operationId: deleteClusterParameterGroup
      x-api-path-slug: actiondeleteclusterparametergroup-get
      parameters:
      - in: query
        name: ParameterGroupName
        description: The name of the parameter group to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DeleteClusterSecurityGroup:
    get:
      summary: Delete Cluster Security Group
      description: Deletes an Amazon Redshift security group.
      operationId: deleteClusterSecurityGroup
      x-api-path-slug: actiondeleteclustersecuritygroup-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name of the cluster security group to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=DeleteClusterSnapshot:
    get:
      summary: Delete Cluster Snapshot
      description: Deletes the specified manual snapshot.
      operationId: deleteClusterSnapshot
      x-api-path-slug: actiondeleteclustersnapshot-get
      parameters:
      - in: query
        name: SnapshotClusterIdentifier
        description: The unique identifier of the cluster the snapshot was created
          from
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The unique identifier of the manual snapshot to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DeleteClusterSubnetGroup:
    get:
      summary: Delete Cluster Subnet Group
      description: Deletes the specified cluster subnet group.
      operationId: deleteClusterSubnetGroup
      x-api-path-slug: actiondeleteclustersubnetgroup-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the cluster subnet group name to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=DescribeClusterParameterGroups:
    get:
      summary: Describe Cluster Parameter Groups
      description: |-
        Returns a list of Amazon Redshift parameter groups, including parameter groups you
                    created and the default parameter group.
      operationId: describeClusterParameterGroups
      x-api-path-slug: actiondescribeclusterparametergroups-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ParameterGroupName
        description: The name of a specific parameter group for which to return details
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          parameter            groups that are associated with the specified key or
          keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster parameter            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DescribeClusterParameters:
    get:
      summary: Describe Cluster Parameters
      description: |-
        Returns a detailed list of parameters contained within the specified Amazon Redshift
                    parameter group.
      operationId: describeClusterParameters
      x-api-path-slug: actiondescribeclusterparameters-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ParameterGroupName
        description: The name of a cluster parameter group for which to return details
        type: string
      - in: query
        name: Source
        description: The parameter types to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameters
  /?Action=DescribeClusters:
    get:
      summary: Describe Clusters
      description: |-
        Returns properties of provisioned clusters including general cluster properties,
                    cluster database properties, maintenance and backup properties, and security and access
                    properties.
      operationId: describeClusters
      x-api-path-slug: actiondescribeclusters-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of a cluster whose properties you are requesting
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching clusters
          that are            associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          clusters that are            associated with the specified tag value or
          values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeClusterSecurityGroups:
    get:
      summary: Describe Cluster Security Groups
      description: Returns information about Amazon Redshift security groups.
      operationId: describeClusterSecurityGroups
      x-api-path-slug: actiondescribeclustersecuritygroups-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name of a cluster security group for which you are requesting
          details
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          security groups            that are associated with the specified key or
          keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster security            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=DescribeClusterSnapshots:
    get:
      summary: Describe Cluster Snapshots
      description: |-
        Returns one or more snapshot objects, which contain metadata about your cluster
                    snapshots.
      operationId: describeClusterSnapshots
      x-api-path-slug: actiondescribeclustersnapshots-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster for which information about snapshots
          is            requested
        type: string
      - in: query
        name: EndTime
        description: A time value that requests only snapshots created at or before
          the specified time
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: OwnerAccount
        description: The AWS customer account used to create or copy the snapshot
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The snapshot identifier of the snapshot about which to return            information
        type: string
      - in: query
        name: SnapshotType
        description: The type of snapshots for which you are requesting information
        type: string
      - in: query
        name: StartTime
        description: A value that requests only snapshots created at or after the
          specified time
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          snapshots that            are associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster snapshots            that are associated with the specified tag
          value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeClusterSubnetGroups:
    get:
      summary: Describe Cluster Subnet Groups
      description: |-
        Returns one or more cluster subnet group objects, which contain metadata about your
                    cluster subnet groups.
      operationId: describeClusterSubnetGroups
      x-api-path-slug: actiondescribeclustersubnetgroups-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the cluster subnet group for which information is
          requested
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          subnet groups            that are associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster subnet            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=DescribeClusterVersions:
    get:
      summary: Describe Cluster Versions
      description: Returns descriptions of the available Amazon Redshift cluster versions.
      operationId: describeClusterVersions
      x-api-path-slug: actiondescribeclusterversions-get
      parameters:
      - in: query
        name: ClusterParameterGroupFamily
        description: The name of a specific cluster parameter group family to return
          details            for
        type: string
      - in: query
        name: ClusterVersion
        description: The specific cluster version to return
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeDefaultClusterParameters:
    get:
      summary: Describe Default Cluster Parameters
      description: |-
        Returns a list of parameter settings for the specified parameter group
                    family.
      operationId: describeDefaultClusterParameters
      x-api-path-slug: actiondescribedefaultclusterparameters-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ParameterGroupFamily
        description: The name of the cluster parameter group family
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameters
  /?Action=DescribeOrderableClusterOptions:
    get:
      summary: Describe Orderable Cluster Options
      description: Returns a list of orderable cluster options.
      operationId: describeOrderableClusterOptions
      x-api-path-slug: actiondescribeorderableclusteroptions-get
      parameters:
      - in: query
        name: ClusterVersion
        description: The version filter value
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: NodeType
        description: The node type filter value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Options
  /?Action=ModifyCluster:
    get:
      summary: Modify Cluster
      description: Modifies the settings for a cluster.
      operationId: modifyCluster
      x-api-path-slug: actionmodifycluster-get
      parameters:
      - in: query
        name: AllowVersionUpgrade
        description: If true, major version upgrades will be applied automatically
          to the            cluster during the maintenance window
        type: string
      - in: query
        name: AutomatedSnapshotRetentionPeriod
        description: The number of days that automated snapshots are retained
        type: string
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the cluster to be modified
        type: string
      - in: query
        name: ClusterParameterGroupName
        description: The name of the cluster parameter group to apply to this cluster
        type: string
      - in: query
        name: ClusterSecurityGroups.ClusterSecurityGroupName.N
        description: A list of cluster security groups to be authorized on this cluster
        type: string
      - in: query
        name: ClusterType
        description: The new cluster type
        type: string
      - in: query
        name: ClusterVersion
        description: The new version number of the Amazon Redshift engine to upgrade
          to
        type: string
      - in: query
        name: ElasticIp
        description: The Elastic IP (EIP) address for the cluster
        type: string
      - in: query
        name: EnhancedVpcRouting
        description: An option that specifies whether to create the cluster with enhanced
          VPC routing            enabled
        type: string
      - in: query
        name: HsmClientCertificateIdentifier
        description: Specifies the name of the HSM client certificate the Amazon Redshift
          cluster uses to            retrieve the data encryption keys stored in an
          HSM
        type: string
      - in: query
        name: HsmConfigurationIdentifier
        description: Specifies the name of the HSM configuration that contains the
          information the            Amazon Redshift cluster can use to retrieve and
          store keys in an HSM
        type: string
      - in: query
        name: MasterUserPassword
        description: The new password for the cluster master user
        type: string
      - in: query
        name: NewClusterIdentifier
        description: The new identifier for the cluster
        type: string
      - in: query
        name: NodeType
        description: The new node type of the cluster
        type: string
      - in: query
        name: NumberOfNodes
        description: The new number of nodes of the cluster
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range (in UTC) during which system maintenance
          can occur, if            necessary
        type: string
      - in: query
        name: PubliclyAccessible
        description: If true, the cluster can be accessed from a public network
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of virtual private cloud (VPC) security groups to be associated
          with the            cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ModifyClusterIamRoles:
    get:
      summary: Modify Cluster Iam Roles
      description: |-
        Modifies the list of AWS Identity and Access Management (IAM) roles that can be
                    used by the cluster to access other AWS services.
      operationId: modifyClusterIamRoles
      x-api-path-slug: actionmodifyclusteriamroles-get
      parameters:
      - in: query
        name: AddIamRoles.IamRoleArn.N
        description: Zero or more IAM roles to associate with the cluster
        type: string
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the cluster for which you want to associate
          or            disassociate IAM roles
        type: string
      - in: query
        name: RemoveIamRoles.IamRoleArn.N
        description: Zero or more IAM roles in ARN format to disassociate from the
          cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster IAM Roles
  /?Action=ModifyClusterParameterGroup:
    get:
      summary: Modify Cluster Parameter Group
      description: Modifies the parameters of a parameter group.
      operationId: modifyClusterParameterGroup
      x-api-path-slug: actionmodifyclusterparametergroup-get
      parameters:
      - in: query
        name: ParameterGroupName
        description: The name of the parameter group to be modified
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: An array of parameters to be modified
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=ModifyClusterSubnetGroup:
    get:
      summary: Modify Cluster Subnet Group
      description: Modifies a cluster subnet group to include the specified list of
        VPC subnets.
      operationId: modifyClusterSubnetGroup
      x-api-path-slug: actionmodifyclustersubnetgroup-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the subnet group to be modified
        type: string
      - in: query
        name: Description
        description: A text description of the subnet group to be modified
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: An array of VPC subnet IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=RebootCluster:
    get:
      summary: Reboot Cluster
      description: Reboots a cluster.
      operationId: rebootCluster
      x-api-path-slug: actionrebootcluster-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The cluster identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ResetClusterParameterGroup:
    get:
      summary: Reset Cluster Parameter Group
      description: |-
        Sets one or more parameters of the specified parameter group to their default
                    values and sets the source values of the parameters to "engine-default".
      operationId: resetClusterParameterGroup
      x-api-path-slug: actionresetclusterparametergroup-get
      parameters:
      - in: query
        name: ParameterGroupName
        description: The name of the cluster parameter group to be reset
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: An array of names of parameters to be reset
        type: string
      - in: query
        name: ResetAllParameters
        description: If true, all parameters in the specified parameter group will
          be reset            to their default values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=RestoreFromClusterSnapshot:
    get:
      summary: Restore From Cluster Snapshot
      description: Creates a new cluster from a snapshot.
      operationId: restoreFromClusterSnapshot
      x-api-path-slug: actionrestorefromclustersnapshot-get
      parameters:
      - in: query
        name: AdditionalInfo
        description: Reserved
        type: string
      - in: query
        name: AllowVersionUpgrade
        description: If true, major version upgrades can be applied during the maintenance            window
          to the Amazon Redshift engine that is running on the cluster
        type: string
      - in: query
        name: AutomatedSnapshotRetentionPeriod
        description: The number of days that automated snapshots are retained
        type: string
      - in: query
        name: AvailabilityZone
        description: The Amazon EC2 Availability Zone in which to restore the cluster
        type: string
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster that will be created from restoring
          the            snapshot
        type: string
      - in: query
        name: ClusterParameterGroupName
        description: The name of the parameter group to be associated with this cluster
        type: string
      - in: query
        name: ClusterSecurityGroups.ClusterSecurityGroupName.N
        description: A list of security groups to be associated with this cluster
        type: string
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the subnet group where you want to cluster restored
        type: string
      - in: query
        name: ElasticIp
        description: The elastic IP (EIP) address for the cluster
        type: string
      - in: query
        name: EnhancedVpcRouting
        description: An option that specifies whether to create the cluster with enhanced
          VPC routing            enabled
        type: string
      - in: query
        name: HsmClientCertificateIdentifier
        description: Specifies the name of the HSM client certificate the Amazon Redshift
          cluster uses to            retrieve the data encryption keys stored in an
          HSM
        type: string
      - in: query
        name: HsmConfigurationIdentifier
        description: Specifies the name of the HSM configuration that contains the
          information the            Amazon Redshift cluster can use to retrieve and
          store keys in an HSM
        type: string
      - in: query
        name: IamRoles.IamRoleArn.N
        description: A list of AWS Identity and Access Management (IAM) roles that
          can be used by the            cluster to access other AWS services
        type: string
      - in: query
        name: KmsKeyId
        description: The AWS Key Management Service (KMS) key ID of the encryption
          key that you want to            use to encrypt data in the cluster that
          you restore from a shared snapshot
        type: string
      - in: query
        name: NodeType
        description: The node type that the restored cluster will be provisioned with
        type: string
      - in: query
        name: OwnerAccount
        description: The AWS customer account used to create or copy the snapshot
        type: string
      - in: query
        name: Port
        description: The port number on which the cluster accepts connections
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range (in UTC) during which automated cluster
          maintenance can            occur
        type: string
      - in: query
        name: PubliclyAccessible
        description: If true, the cluster can be accessed from a public network
        type: string
      - in: query
        name: SnapshotClusterIdentifier
        description: The name of the cluster the source snapshot was created from
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The name of the snapshot from which to create the new cluster
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of Virtual Private Cloud (VPC) security groups to be associated
          with the            cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=RestoreTableFromClusterSnapshot:
    get:
      summary: Restore Table From Cluster Snapshot
      description: Creates a new table from a table in an Amazon Redshift cluster
        snapshot.
      operationId: restoreTableFromClusterSnapshot
      x-api-path-slug: actionrestoretablefromclustersnapshot-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the Amazon Redshift cluster to restore the
          table to
        type: string
      - in: query
        name: NewTableName
        description: The name of the table to create as a result of the current request
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The identifier of the snapshot to restore the table from
        type: string
      - in: query
        name: SourceDatabaseName
        description: The name of the source database that contains the table to restore
          from
        type: string
      - in: query
        name: SourceSchemaName
        description: The name of the source schema that contains the table to restore
          from
        type: string
      - in: query
        name: SourceTableName
        description: The name of the source table to restore from
        type: string
      - in: query
        name: TargetDatabaseName
        description: The name of the database to restore the table to
        type: string
      - in: query
        name: TargetSchemaName
        description: The name of the schema to restore the table to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=RevokeClusterSecurityGroupIngress:
    get:
      summary: Revoke Cluster Security Group Ingress
      description: |-
        Revokes an ingress rule in an Amazon Redshift security group for a previously authorized
                    IP range or Amazon EC2 security group.
      operationId: revokeClusterSecurityGroupIngress
      x-api-path-slug: actionrevokeclustersecuritygroupingress-get
      parameters:
      - in: query
        name: CIDRIP
        description: The IP range for which to revoke access
        type: string
      - in: query
        name: ClusterSecurityGroupName
        description: The name of the security Group from which to revoke the ingress
          rule
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The name of the EC2 Security Group whose access is to be revoked
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS account number of the owner of the security group specified
          in the                EC2SecurityGroupName parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
---