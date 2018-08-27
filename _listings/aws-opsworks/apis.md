---
name: AWS OpsWorks
x-slug: aws-opsworks
description: AWS OpsWorks is a configuration management service that uses Chef, an
  automation platform that treats server configurations as code. OpsWorks uses Chef
  to automate how servers are configured, deployed, and managed across your Amazon
  Elastic Compute Cloud (Amazon EC2) instances or on-premises compute environments.
  OpsWorks has two offerings, AWS Opsworks for Chef Automate, and AWS OpsWorks Stacks.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Cluster
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/aws-opsworks/apis.md
specificationVersion: "0.14"
apis:
- name: AWS OpsWorks API - Deregister Ecs Cluster
  x-api-slug: actionderegisterecscluster-get
  description: Deregisters a specified Amazon ECS cluster from a stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: :///
  tags: Amazon Web Services, Orchestration, Stack Network, API Service Provider, API
    Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/aws-opsworks/actionderegisterecscluster-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/aws-opsworks/actionderegisterecscluster-get-openapi.md
- name: AWS OpsWorks API - Register Ecs Cluster
  x-api-slug: actionregisterecscluster-get
  description: Registers a specified Amazon ECS cluster with a stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: :///
  tags: Amazon Web Services, Orchestration, Stack Network, API Service Provider, API
    Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/aws-opsworks/actionregisterecscluster-get-openapi.md
- name: AWS OpsWorks API - Describe Ecs Clusters
  x-api-slug: actiondescribeecsclusters-get
  description: Describes Amazon ECS clusters that are registered with a stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: :///
  tags: Amazon Web Services, Orchestration, Stack Network, API Service Provider, API
    Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/aws-opsworks/actiondescribeecsclusters-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.marketplace.metering.service.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.opsworks.stack.network
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/userguide/cli-chap-welcome.html
- type: x-documentation
  url: http://docs.aws.amazon.com/opsworks/latest/APIReference/Welcome.html
- type: x-website
  url: https://aws.amazon.com/opsworks/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---