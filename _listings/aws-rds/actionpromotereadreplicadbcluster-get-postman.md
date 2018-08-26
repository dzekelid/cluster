{
  "info": {
    "name": "Amazon RDS API Promote Read Replica D B Cluster",
    "_postman_id": "c8f5a9d2-6da5-4651-9ece-726c6949f2b5",
    "description": "Promotes a Read Replica DB cluster to a standalone DB cluster.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clusters",
      "item": [
        {
          "id": "e4382d9b-7543-4132-9c36-b45d77d708dd",
          "name": "addroletodbcluster",
          "request": {
            "url": "http://example.com/api/?Action=AddRoleToDBCluster?DBClusterIdentifier=DBClusterIdentifier&RoleArn=RoleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates an Identity and Access Management (IAM) role from an Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "574b5d58-16a3-488b-8da6-a341f73b33b7"
            }
          ]
        },
        {
          "id": "a92ea560-7300-42c0-8644-c3f9783a8c59",
          "name": "createdbcluster",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBCluster?AvailabilityZones.AvailabilityZone.N=AvailabilityZones.AvailabilityZone.N&BackupRetentionPeriod=BackupRetentionPeriod&CharacterSetName=CharacterSetName&DatabaseName=DatabaseName&DBClusterIdentifier=DBClusterIdentifier&DBClusterParameterGroupName=DBClusterParameterGroupName&DBSubnetGroupName=DBSubnetGroupName&Engine=Engine&EngineVersion=EngineVersion&KmsKeyId=KmsKeyId&MasterUsername=MasterUsername&MasterUserPassword=MasterUserPassword&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&ReplicationSourceIdentifier=ReplicationSourceIdentifier&StorageEncrypted=StorageEncrypted&Tags.Tag.N=Tags.Tag.N&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58b5403e-565e-4999-8246-d36605de359c"
            }
          ]
        },
        {
          "id": "43363a9a-c401-4e34-b30d-92fcb2b90457",
          "name": "deletedbcluster",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBCluster?DBClusterIdentifier=DBClusterIdentifier&FinalDBSnapshotIdentifier=FinalDBSnapshotIdentifier&SkipFinalSnapshot=SkipFinalSnapshot",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteDBCluster action deletes a previously provisioned DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1578065-e299-4a27-a321-30613c1c194e"
            }
          ]
        },
        {
          "id": "a75302f7-79b0-4396-9fe3-87aa74f2eee1",
          "name": "describedbclusters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusters?DBClusterIdentifier=DBClusterIdentifier&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about provisioned Aurora DB clusters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66ca3104-b6aa-4827-b5ac-709fb4ce07a3"
            }
          ]
        },
        {
          "id": "d6af8480-433c-45fa-84d1-a9ddd92e7294",
          "name": "failoverdbcluster",
          "request": {
            "url": "http://example.com/api/?Action=FailoverDBCluster?DBClusterIdentifier=DBClusterIdentifier&TargetDBInstanceIdentifier=TargetDBInstanceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Forces a failover for a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73628ca2-e4a4-48a0-8956-0308c5f068ce"
            }
          ]
        },
        {
          "id": "66ee2c78-a303-4e89-8524-c9af302a01e4",
          "name": "modifydbcluster",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBCluster?ApplyImmediately=ApplyImmediately&BackupRetentionPeriod=BackupRetentionPeriod&DBClusterIdentifier=DBClusterIdentifier&DBClusterParameterGroupName=DBClusterParameterGroupName&MasterUserPassword=MasterUserPassword&NewDBClusterIdentifier=NewDBClusterIdentifier&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modify a setting for an Amazon Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f66855c-eafb-45f7-98e8-5b47033c4c3c"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "8cd2ef4b-2d70-49d3-8fca-41e7bff78407",
          "name": "addsourceidentifiertosubscription",
          "request": {
            "url": "http://example.com/api/?Action=AddSourceIdentifierToSubscription?SourceIdentifier=SourceIdentifier&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a source identifier to an existing RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92febd8a-3837-4616-831c-1a296003c64c"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "03f50e4a-1efc-4f6b-99cd-0c451740b2a8",
          "name": "addtagstoresource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceName=ResourceName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds metadata tags to an Amazon RDS resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "faf58c01-3e1c-4074-a8f8-2aa2db7b896c"
            }
          ]
        },
        {
          "id": "dbcb707f-1432-4664-8a17-283b7b6c02e2",
          "name": "listtagsforresource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?Filters.Filter.N=Filters.Filter.N&ResourceName=ResourceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all tags on an Amazon RDS resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0b0fb06-e8c0-4f17-a2b0-7928c3d80c9e"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance Actions",
      "item": [
        {
          "id": "5226f551-1c94-40c7-90a7-f91d4cef535e",
          "name": "applypendingmaintenanceaction",
          "request": {
            "url": "http://example.com/api/?Action=ApplyPendingMaintenanceAction?ApplyAction=ApplyAction&OptInType=OptInType&ResourceIdentifier=ResourceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Applies a pending maintenance action to a resource (for example, to a DB instance)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82b1634a-9def-4ea3-bc8b-d1cf82beaf12"
            }
          ]
        },
        {
          "id": "15448a3b-d4e8-4607-a9af-73dfd0900950",
          "name": "describependingmaintenanceactions",
          "request": {
            "url": "http://example.com/api/?Action=DescribePendingMaintenanceActions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&ResourceIdentifier=ResourceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of resources (for example, DB instances) that have at least one pending maintenance action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be28a63d-cec2-4530-9ac2-9e1de0a9052a"
            }
          ]
        }
      ]
    },
    {
      "name": "Security Groups",
      "item": [
        {
          "id": "1ff8f503-9c9e-474b-9a22-387a71ce4d70",
          "name": "authorizedbsecuritygroupingress",
          "request": {
            "url": "http://example.com/api/?Action=AuthorizeDBSecurityGroupIngress?CIDRIP=CIDRIP&DBSecurityGroupName=DBSecurityGroupName&EC2SecurityGroupId=EC2SecurityGroupId&EC2SecurityGroupName=EC2SecurityGroupName&EC2SecurityGroupOwnerId=EC2SecurityGroupOwnerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables ingress to a DBSecurityGroup using one of two forms of authorization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "592648f7-6503-46ee-9d08-bf64fbbd3fca"
            }
          ]
        },
        {
          "id": "4fc8df68-f009-4573-a69b-a49231eced5b",
          "name": "createdbsecuritygroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSecurityGroup?DBSecurityGroupDescription=DBSecurityGroupDescription&DBSecurityGroupName=DBSecurityGroupName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d129e9fe-b415-4169-bd84-30b507e34c43"
            }
          ]
        },
        {
          "id": "372ec327-1216-46b1-afd3-d9a303b864cc",
          "name": "deletedbsecuritygroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSecurityGroup?DBSecurityGroupName=DBSecurityGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66790652-7a07-4c8e-8c7b-391dde92c592"
            }
          ]
        },
        {
          "id": "57295553-e584-4547-aa75-d49d8fb607dd",
          "name": "describedbsecuritygroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSecurityGroups?DBSecurityGroupName=DBSecurityGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBSecurityGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c50220d-de10-44b9-be55-8fbc217bcd25"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameter Groups",
      "item": [
        {
          "id": "8c7be99a-c555-4e03-ba85-36fad10408a8",
          "name": "copydbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBClusterParameterGroup?SourceDBClusterParameterGroupIdentifier=SourceDBClusterParameterGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBClusterParameterGroupDescription=TargetDBClusterParameterGroupDescription&TargetDBClusterParameterGroupIdentifier=TargetDBClusterParameterGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b36e8e67-6fb8-47fb-8dbf-5be1586fd3e2"
            }
          ]
        },
        {
          "id": "21b5438e-36d2-4655-acaf-aae552cbe448",
          "name": "createdbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName&DBParameterGroupFamily=DBParameterGroupFamily&Description=Description&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec8c8a17-6749-466f-b588-e61237e49b73"
            }
          ]
        },
        {
          "id": "9b189c46-99ea-4b24-8cb3-77615db7a934",
          "name": "deletedbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26f7d40c-8ec3-4245-8fd0-ac910442333d"
            }
          ]
        },
        {
          "id": "c090b578-e517-41a5-aa24-45e6120f5f4b",
          "name": "describedbclusterparametergroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterParameterGroups?DBClusterParameterGroupName=DBClusterParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBClusterParameterGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b920b75-47fc-4f1d-b9d7-c83db989f377"
            }
          ]
        },
        {
          "id": "2583b1a3-cf5d-4788-809b-d15b99d9c342",
          "name": "modifydbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName&Parameters.Parameter.N=Parameters.Parameter.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the parameters of a DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c6e9d4d-c8cc-4dec-b018-2d83ddfc0073"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Snapshots",
      "item": [
        {
          "id": "c7d407ae-979c-4754-8e16-fa8a331b9dda",
          "name": "copydbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBClusterSnapshot?SourceDBClusterSnapshotIdentifier=SourceDBClusterSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBClusterSnapshotIdentifier=TargetDBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a28967d-b829-4235-bbb9-5315eabac7f6"
            }
          ]
        },
        {
          "id": "2ba625e0-c776-4eb7-b428-63812f789c18",
          "name": "createdbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBClusterSnapshot?DBClusterIdentifier=DBClusterIdentifier&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "635c02b8-fca2-4ec7-a0cd-d8f44a75988d"
            }
          ]
        },
        {
          "id": "ca2bf73a-3b4d-41b5-9e5d-98d3907f7f4d",
          "name": "deletedbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBClusterSnapshot?DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5a13a43-5085-4a58-bb21-f6f98ab140dc"
            }
          ]
        },
        {
          "id": "460d7ee3-614e-452f-b11d-3f13a6f8f61f",
          "name": "describedbclustersnapshotattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterSnapshotAttributes?DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DB cluster snapshot attribute names and values for a manual DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aba3942d-c566-4fd4-8d59-50deb07a512a"
            }
          ]
        },
        {
          "id": "20838fcc-0b72-407f-9556-208f4e861fdd",
          "name": "describedbclustersnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterSnapshots?DBClusterIdentifier=DBClusterIdentifier&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&Filters.Filter.N=Filters.Filter.N&IncludePublic=IncludePublic&IncludeShared=IncludeShared&Marker=Marker&MaxRecords=MaxRecords&SnapshotType=SnapshotType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about DB cluster snapshots."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "376fb565-f819-4f51-9b35-039bb8120e42"
            }
          ]
        },
        {
          "id": "c3ada9b7-c44c-4000-8bfc-2df1b5d6facf",
          "name": "modifydbclustersnapshotattribute",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBClusterSnapshotAttribute?AttributeName=AttributeName&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&ValuesToAdd.AttributeValue.N=ValuesToAdd.AttributeValue.N&ValuesToRemove.AttributeValue.N=ValuesToRemove.AttributeValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an attribute and values to, or removes an attribute and values from, a manual DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbb03ea7-3c58-4f9b-a765-736bb680bfc3"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter Groups",
      "item": [
        {
          "id": "863ca5fe-811d-467c-a42e-032316b885bc",
          "name": "copydbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBParameterGroup?SourceDBParameterGroupIdentifier=SourceDBParameterGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBParameterGroupDescription=TargetDBParameterGroupDescription&TargetDBParameterGroupIdentifier=TargetDBParameterGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b57e0c7-1f1c-4ae0-b26d-5bbe5bd291b0"
            }
          ]
        },
        {
          "id": "8a977084-0443-4fd4-998c-2d7dc0da25ee",
          "name": "createdbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBParameterGroup?DBParameterGroupFamily=DBParameterGroupFamily&DBParameterGroupName=DBParameterGroupName&Description=Description&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ee77b4d-a0b5-4313-a418-007f600c5fc2"
            }
          ]
        },
        {
          "id": "c6076cb0-4d6c-44f6-909d-f97ce84139f3",
          "name": "deletedbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBParameterGroup?DBParameterGroupName=DBParameterGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified DBParameterGroup."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5db4cfd8-c4b1-4e87-890c-038dacb95e7a"
            }
          ]
        },
        {
          "id": "18a6406f-dbf7-4baf-84ab-92ac11a5a2c7",
          "name": "describedbparametergroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBParameterGroups?DBParameterGroupName=DBParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBParameterGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d86df79d-b162-46ca-aa2b-b1448c8e888a"
            }
          ]
        },
        {
          "id": "74d3d53e-9898-49ee-92b6-7d9b505b360d",
          "name": "modifydbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBParameterGroup?DBParameterGroupName=DBParameterGroupName&Parameters.Parameter.N=Parameters.Parameter.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the parameters of a DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89174969-3c3a-4e52-91ae-bb214e6a62a3"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "969e85ea-88c2-4416-8880-797a9a6cd70f",
          "name": "copydbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBSnapshot?CopyTags=CopyTags&KmsKeyId=KmsKeyId&PreSignedUrl=PreSignedUrl&SourceDBSnapshotIdentifier=SourceDBSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBSnapshotIdentifier=TargetDBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92d3b48d-6f36-4af8-8a8c-9b0bc0e0aea4"
            }
          ]
        },
        {
          "id": "37851598-ef9d-41b0-ba5a-5d5542b4153b",
          "name": "createdbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSnapshot?DBInstanceIdentifier=DBInstanceIdentifier&DBSnapshotIdentifier=DBSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a DBSnapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85a2ef12-580d-4fbe-be9f-a2e94d60393b"
            }
          ]
        },
        {
          "id": "465bca63-16a8-4f15-addc-e01af53b892a",
          "name": "deletedbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSnapshot?DBSnapshotIdentifier=DBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DBSnapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23f61a41-a68c-46bf-af68-c58f20231f51"
            }
          ]
        },
        {
          "id": "17d2d43b-8b70-4f23-b4dd-a0f02f1754b1",
          "name": "describedbsnapshotattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSnapshotAttributes?DBSnapshotIdentifier=DBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DB snapshot attribute names and values for a manual DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0190b56e-8963-45dd-87ff-552eb7ef3104"
            }
          ]
        },
        {
          "id": "8761075f-9fe3-43e5-b456-6609f09a940c",
          "name": "describedbsnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSnapshots?DBInstanceIdentifier=DBInstanceIdentifier&DBSnapshotIdentifier=DBSnapshotIdentifier&Filters.Filter.N=Filters.Filter.N&IncludePublic=IncludePublic&IncludeShared=IncludeShared&Marker=Marker&MaxRecords=MaxRecords&SnapshotType=SnapshotType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about DB snapshots."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c58e36e-189b-4991-a3b5-448ac9d323d6"
            }
          ]
        },
        {
          "id": "d0c01907-7ebf-407c-99d7-16c9b65bb5f1",
          "name": "modifydbsnapshotattribute",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBSnapshotAttribute?AttributeName=AttributeName&DBSnapshotIdentifier=DBSnapshotIdentifier&ValuesToAdd.AttributeValue.N=ValuesToAdd.AttributeValue.N&ValuesToRemove.AttributeValue.N=ValuesToRemove.AttributeValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an attribute and values to, or removes an attribute and values from, a manual DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5597a1a7-6546-49da-809d-f7ce82d5bc5b"
            }
          ]
        }
      ]
    },
    {
      "name": "Option Groups",
      "item": [
        {
          "id": "66ede356-f3a1-4fde-833c-cc94df0b3b3d",
          "name": "copyoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyOptionGroup?SourceOptionGroupIdentifier=SourceOptionGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetOptionGroupDescription=TargetOptionGroupDescription&TargetOptionGroupIdentifier=TargetOptionGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00e83f09-2b7b-4f19-9939-3f03df7bf7f6"
            }
          ]
        },
        {
          "id": "d9a978a8-1eb5-4b5e-b9ff-4145cc5bd1c9",
          "name": "createoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateOptionGroup?EngineName=EngineName&MajorEngineVersion=MajorEngineVersion&OptionGroupDescription=OptionGroupDescription&OptionGroupName=OptionGroupName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e37c5ee-77a4-4b2a-b430-441bf89c17d9"
            }
          ]
        },
        {
          "id": "6231c2b7-945c-4152-ac59-d29df2c3fec5",
          "name": "deleteoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteOptionGroup?OptionGroupName=OptionGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7a978a4-d1b2-410c-b93c-8097db48777b"
            }
          ]
        },
        {
          "id": "ac73dd08-1484-4e58-8617-3e9b60700668",
          "name": "describeoptiongroupoptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOptionGroupOptions?EngineName=EngineName&Filters.Filter.N=Filters.Filter.N&MajorEngineVersion=MajorEngineVersion&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes all available options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d58ad4dd-fa6e-4e35-92a5-2257b3f629e0"
            }
          ]
        },
        {
          "id": "eddf69ba-e0ef-4e42-9486-a524af388514",
          "name": "describeoptiongroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOptionGroups?EngineName=EngineName&Filters.Filter.N=Filters.Filter.N&MajorEngineVersion=MajorEngineVersion&Marker=Marker&MaxRecords=MaxRecords&OptionGroupName=OptionGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the available option groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c0a84cc-37b4-463f-9da8-e484700f9b40"
            }
          ]
        },
        {
          "id": "8d373dfd-e76f-4b11-a1de-7880f15c1b8f",
          "name": "modifyoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyOptionGroup?ApplyImmediately=ApplyImmediately&OptionGroupName=OptionGroupName&OptionsToInclude.OptionConfiguration.N=OptionsToInclude.OptionConfiguration.N&OptionsToRemove.member.N=OptionsToRemove.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies an existing option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2e14208-3ff6-4e6a-9522-e0001614197c"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "ec5a3265-59ba-4acc-a1f3-3dd0b050b397",
          "name": "createdbinstance",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBInstance?AllocatedStorage=AllocatedStorage&AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&AvailabilityZone=AvailabilityZone&BackupRetentionPeriod=BackupRetentionPeriod&CharacterSetName=CharacterSetName&CopyTagsToSnapshot=CopyTagsToSnapshot&DBClusterIdentifier=DBClusterIdentifier&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBName=DBName&DBParameterGroupName=DBParameterGroupName&DBSecurityGroups.DBSecurityGroupName.N=DBSecurityGroups.DBSecurityGroupName.N&DBSubnetGroupName=DBSubnetGroupName&Domain=Domain&DomainIAMRoleName=DomainIAMRoleName&Engine=Engine&EngineVersion=EngineVersion&Iops=Iops&KmsKeyId=KmsKeyId&LicenseModel=LicenseModel&MasterUsername=MasterUsername&MasterUserPassword=MasterUserPassword&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&MultiAZ=MultiAZ&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PromotionTier=PromotionTier&PubliclyAccessible=PubliclyAccessible&StorageEncrypted=StorageEncrypted&StorageType=StorageType&Tags.Tag.N=Tags.Tag.N&TdeCredentialArn=TdeCredentialArn&TdeCredentialPassword=TdeCredentialPassword&Timezone=Timezone&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ef26491-8178-41fb-91d4-7f0ad6276a8e"
            }
          ]
        },
        {
          "id": "98278341-9f75-41dd-aa6e-3290e09853ee",
          "name": "createdbinstancereadreplica",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBInstanceReadReplica?AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&AvailabilityZone=AvailabilityZone&CopyTagsToSnapshot=CopyTagsToSnapshot&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBSubnetGroupName=DBSubnetGroupName&Iops=Iops&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&OptionGroupName=OptionGroupName&Port=Port&PubliclyAccessible=PubliclyAccessible&SourceDBInstanceIdentifier=SourceDBInstanceIdentifier&StorageType=StorageType&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a DB instance for a DB instance running MySQL, MariaDB, or PostgreSQL that acts as a Read Replica of a source DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cde589f9-029c-48e9-8e6d-fa4a56155262"
            }
          ]
        },
        {
          "id": "42545bd4-19bf-440e-a195-a54ba9e55176",
          "name": "deletedbinstance",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBInstance?DBInstanceIdentifier=DBInstanceIdentifier&FinalDBSnapshotIdentifier=FinalDBSnapshotIdentifier&SkipFinalSnapshot=SkipFinalSnapshot",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteDBInstance action deletes a previously provisioned DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c3d23ab-f65f-4a43-83e0-64f776f2a559"
            }
          ]
        },
        {
          "id": "1bf803f7-338d-4c0a-9948-0e1db2bbb6fa",
          "name": "describedbinstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBInstances?DBInstanceIdentifier=DBInstanceIdentifier&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about provisioned RDS instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31fab824-ac45-4225-84f6-0601ec672197"
            }
          ]
        },
        {
          "id": "788fa4b1-4104-4fb3-844a-033eb14b3bbb",
          "name": "describeorderabledbinstanceoptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOrderableDBInstanceOptions?DBInstanceClass=DBInstanceClass&Engine=Engine&EngineVersion=EngineVersion&Filters.Filter.N=Filters.Filter.N&LicenseModel=LicenseModel&Marker=Marker&MaxRecords=MaxRecords&Vpc=Vpc",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of orderable DB instance options for the specified engine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bec3a491-003b-4f4d-91a9-f91f205bf2ca"
            }
          ]
        },
        {
          "id": "392e131f-6d51-4b6e-9ec9-5fc857e98029",
          "name": "describereserveddbinstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReservedDBInstances?DBInstanceClass=DBInstanceClass&Duration=Duration&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&MultiAZ=MultiAZ&OfferingType=OfferingType&ProductDescription=ProductDescription&ReservedDBInstanceId=ReservedDBInstanceId&ReservedDBInstancesOfferingId=ReservedDBInstancesOfferingId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about reserved DB instances for this account, or about a specified reserved DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b3b6cdd-5cb2-47b3-b181-73b4de8b9e7b"
            }
          ]
        },
        {
          "id": "a00d90ef-9b5e-4d19-823e-fa94e74a69a4",
          "name": "describereserveddbinstancesofferings",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReservedDBInstancesOfferings?DBInstanceClass=DBInstanceClass&Duration=Duration&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&MultiAZ=MultiAZ&OfferingType=OfferingType&ProductDescription=ProductDescription&ReservedDBInstancesOfferingId=ReservedDBInstancesOfferingId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists available reserved DB instance offerings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c9fba0f-379c-463b-996c-1f15ea5c6305"
            }
          ]
        },
        {
          "id": "9ea87f36-8494-4626-a109-7f6e3c3c37f8",
          "name": "modifydbinstance",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBInstance?AllocatedStorage=AllocatedStorage&AllowMajorVersionUpgrade=AllowMajorVersionUpgrade&ApplyImmediately=ApplyImmediately&AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&BackupRetentionPeriod=BackupRetentionPeriod&CACertificateIdentifier=CACertificateIdentifier&CopyTagsToSnapshot=CopyTagsToSnapshot&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBParameterGroupName=DBParameterGroupName&DBPortNumber=DBPortNumber&DBSecurityGroups.DBSecurityGroupName.N=DBSecurityGroups.DBSecurityGroupName.N&DBSubnetGroupName=DBSubnetGroupName&Domain=Domain&DomainIAMRoleName=DomainIAMRoleName&EngineVersion=EngineVersion&Iops=Iops&LicenseModel=LicenseModel&MasterUserPassword=MasterUserPassword&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&MultiAZ=MultiAZ&NewDBInstanceIdentifier=NewDBInstanceIdentifier&OptionGroupName=OptionGroupName&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PromotionTier=PromotionTier&PubliclyAccessible=PubliclyAccessible&StorageType=StorageType&TdeCredentialArn=TdeCredentialArn&TdeCredentialPassword=TdeCredentialPassword&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies settings for a DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e033b8bd-73c9-4fc9-b1c2-7fdc07e13a4c"
            }
          ]
        }
      ]
    },
    {
      "name": "Subnet Groups",
      "item": [
        {
          "id": "72807e30-e482-44cc-b9e1-247b095ffebf",
          "name": "createdbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSubnetGroup?DBSubnetGroupDescription=DBSubnetGroupDescription&DBSubnetGroupName=DBSubnetGroupName&SubnetIds.SubnetIdentifier.N=SubnetIds.SubnetIdentifier.N&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f240377-ea1e-4903-8fd3-67275c2c2ac9"
            }
          ]
        },
        {
          "id": "c1bcd848-0625-432c-9dee-3040539d3227",
          "name": "deletedbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSubnetGroup?DBSubnetGroupName=DBSubnetGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53bbef27-e1c5-4ef0-ae73-3bd4b5d7f171"
            }
          ]
        },
        {
          "id": "d8e38a92-6bb9-482b-b910-8a22fbc57042",
          "name": "describedbsubnetgroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSubnetGroups?DBSubnetGroupName=DBSubnetGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBSubnetGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13eef3de-ca74-4cbc-87dd-d4be713b539e"
            }
          ]
        },
        {
          "id": "f8d515b5-e1bb-47c2-bd77-f1946c6307e0",
          "name": "modifydbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBSubnetGroup?DBSubnetGroupDescription=DBSubnetGroupDescription&DBSubnetGroupName=DBSubnetGroupName&SubnetIds.SubnetIdentifier.N=SubnetIds.SubnetIdentifier.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies an existing DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a9a9eba-14b8-4404-b224-d99dac6027f8"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "2e3c6d45-8542-4711-9a65-5c387162c69f",
          "name": "createeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=CreateEventSubscription?Enabled=Enabled&EventCategories.EventCategory.N=EventCategories.EventCategory.N&SnsTopicArn=SnsTopicArn&SourceIds.SourceId.N=SourceIds.SourceId.N&SourceType=SourceType&SubscriptionName=SubscriptionName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a88997cf-17c3-401e-8519-5ad99106a1a7"
            }
          ]
        },
        {
          "id": "6e9f6088-d5af-477c-98f8-c17ab1431137",
          "name": "deleteeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEventSubscription?SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d63c546-381b-4a89-860e-e69885a37f22"
            }
          ]
        },
        {
          "id": "0e587451-a748-49ab-b0cc-ce4f41193ae3",
          "name": "describeeventsubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventSubscriptions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the subscription descriptions for a customer account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ad45855-3775-4360-a6f5-77f1ee17c49d"
            }
          ]
        },
        {
          "id": "8cf2cc78-60b8-4ca4-b060-a34b2569bee2",
          "name": "modifyeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=ModifyEventSubscription?Enabled=Enabled&EventCategories.EventCategory.N=EventCategories.EventCategory.N&SnsTopicArn=SnsTopicArn&SourceType=SourceType&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies an existing RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6633f111-211c-4b04-a7ea-bbc81b2afed8"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "e56ab512-2d5f-4317-a8e2-76fbfab12d24",
          "name": "describeaccountattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountAttributes?AccountQuotas.AccountQuota.N=AccountQuotas.AccountQuota.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the attributes for a customer account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c5792d6-bb9e-4b8f-8e2e-492493e36251"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "1eac2cfe-8407-4620-abe7-540ad3db58f6",
          "name": "describecertificates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCertificates?CertificateIdentifier=CertificateIdentifier&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the set of CA certificates provided by Amazon RDS for this AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec3253a5-19ef-40e7-ac56-85bc0a270239"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameters",
      "item": [
        {
          "id": "4b68c017-471e-41bb-90b8-8c653b5af46d",
          "name": "describedbclusterparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterParameters?DBClusterParameterGroupName=DBClusterParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&Source=Source",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the detailed parameter list for a particular DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84ad248e-6c58-412a-b391-24a185ef0513"
            }
          ]
        }
      ]
    },
    {
      "name": "Engines",
      "item": [
        {
          "id": "1ca8925c-034f-481d-a0ed-1bbbf5df0181",
          "name": "describedbengineversions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBEngineVersions?DBParameterGroupFamily=DBParameterGroupFamily&DefaultOnly=DefaultOnly&Engine=Engine&EngineVersion=EngineVersion&Filters.Filter.N=Filters.Filter.N&ListSupportedCharacterSets=ListSupportedCharacterSets&ListSupportedTimezones=ListSupportedTimezones&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available DB engines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fce1f4c6-e53c-4956-a58d-37fa125f34db"
            }
          ]
        }
      ]
    },
    {
      "name": "Blog Files",
      "item": [
        {
          "id": "4d2f694b-bdef-47d0-af1d-41482ebe5bff",
          "name": "describedblogfiles",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBLogFiles?DBInstanceIdentifier=DBInstanceIdentifier&FileLastWritten=FileLastWritten&FilenameContains=FilenameContains&FileSize=FileSize&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DB log files for the DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f378d9d2-a8f6-4895-b26b-cef69a22cbb2"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "896f92ae-171e-457f-aff5-18c9504817da",
          "name": "describedbparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBParameters?DBParameterGroupName=DBParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&Source=Source",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the detailed parameter list for a particular DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97015360-22e1-43fb-bc30-668abdf649e8"
            }
          ]
        }
      ]
    },
    {
      "name": "Default Cluster Parameters",
      "item": [
        {
          "id": "462b8724-c5da-4ce8-ad02-176a81e3423b",
          "name": "describeenginedefaultclusterparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEngineDefaultClusterParameters?DBParameterGroupFamily=DBParameterGroupFamily&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default engine and system parameter information for the cluster database engine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "333aaf03-3c8f-46d3-9a73-d79019bc9849"
            }
          ]
        }
      ]
    },
    {
      "name": "Default Parameters",
      "item": [
        {
          "id": "84bf5aac-8115-4310-a2c4-f85764e20e0d",
          "name": "describeenginedefaultparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEngineDefaultParameters?DBParameterGroupFamily=DBParameterGroupFamily&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default engine and system parameter information for the specified database engine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc4f0a94-d8af-4649-9882-580244f0faeb"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Categories",
      "item": [
        {
          "id": "47c86f4a-e930-4fb4-9b03-07aaee1aca96",
          "name": "describeeventcategories",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventCategories?Filters.Filter.N=Filters.Filter.N&SourceType=SourceType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Displays a list of categories for all event source types, or, if specified, for a specified source type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ff39862-0f89-4467-9c85-6d42e0d386c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "35d653b8-f52f-48fe-af51-95b0213e373f",
          "name": "describeevents",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEvents?Duration=Duration&EndTime=EndTime&EventCategories.EventCategory.N=EventCategories.EventCategory.N&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&SourceIdentifier=SourceIdentifier&SourceType=SourceType&StartTime=StartTime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns events related to DB instances, DB security groups, DB snapshots, and DB parameter groups for the past 14 days."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4ba29b2-2300-44e1-9e63-83212f0ff139"
            }
          ]
        }
      ]
    },
    {
      "name": "Source Regions",
      "item": [
        {
          "id": "b0554401-f5cb-4899-8721-165ca909c4e4",
          "name": "describesourceregions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSourceRegions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&RegionName=RegionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the source AWS regions where the current AWS region can create a Read Replica \n            or copy a DB snapshot from."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "600232e7-28e9-4dd3-8cc9-b220cb8e21c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Log Files",
      "item": [
        {
          "id": "46316822-03cd-4a01-ab97-c8c0474c94c3",
          "name": "downloaddblogfileportion",
          "request": {
            "url": "http://example.com/api/?Action=DownloadDBLogFilePortion?DBInstanceIdentifier=DBInstanceIdentifier&LogFileName=LogFileName&Marker=Marker&NumberOfLines=NumberOfLines",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Downloads all or a portion of the specified log file, up to 1 MB in size."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef8223ec-0cc0-4b32-b8b6-89aadac7908d"
            }
          ]
        }
      ]
    },
    {
      "name": "Replicas",
      "item": [
        {
          "id": "13d7aa72-7a6f-4c4c-bfad-f9bd2575f84a",
          "name": "promotereadreplica",
          "request": {
            "url": "http://example.com/api/?Action=PromoteReadReplica?BackupRetentionPeriod=BackupRetentionPeriod&DBInstanceIdentifier=DBInstanceIdentifier&PreferredBackupWindow=PreferredBackupWindow",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Promotes a Read Replica DB instance to a standalone DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0100eb72-cf5a-4575-b61e-d4fff7aefa57"
            }
          ]
        },
        {
          "id": "98fc0b70-814c-4433-8e4a-d0b66bae1dc3",
          "name": "promotereadreplicadbcluster",
          "request": {
            "url": "http://example.com/api/?Action=PromoteReadReplicaDBCluster?DBClusterIdentifier=DBClusterIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Promotes a Read Replica DB cluster to a standalone DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81cc7f91-2b2b-4209-ba0b-6fbe4ae2696d"
            }
          ]
        }
      ]
    }
  ]
}