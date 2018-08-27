---
name: Google Cloud Dataproc
x-slug: google-cloud-dataproc
description: Use Google Cloud Dataproc, an Apache Hadoop, Apache Spark, Apache Pig,
  and Apache Hive service, to easily process big datasets at low cost. Control your
  costs by quickly creating managed clusters of any size and turning them off when
  youre done. Cloud Dataproc integrates across Google Cloud Platform products, giving
  you a powerful and complete data processing platform.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/dataproc.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Cluster
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/google-cloud-dataproc/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud Dataproc - Get Region Clusters
  x-api-slug: v1projectsprojectidregionsregionclusters-get
  description: Lists all regions/{region}/clusters in a project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/dataproc.png
  humanURL: https://cloud.google.com/dataproc/
  baseURL: ://dataproc.googleapis.com//
  tags: Google APIs, Data, Stack Network, API Service Provider, API Provider, Databases,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/google-cloud-dataproc/v1projectsprojectidregionsregionclusters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/google-cloud-dataproc/v1projectsprojectidregionsregionclusters-get-openapi.md
- name: Google Cloud Dataproc - Create Cluster
  x-api-slug: v1projectsprojectidregionsregionclusters-post
  description: Creates a cluster in a project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/dataproc.png
  humanURL: https://cloud.google.com/dataproc/
  baseURL: ://dataproc.googleapis.com//
  tags: Google APIs, Data, Stack Network, API Service Provider, API Provider, Databases,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/google-cloud-dataproc/v1projectsprojectidregionsregionclusters-post-openapi.md
- name: Google Cloud Dataproc - Delete Cluster
  x-api-slug: v1projectsprojectidregionsregionclustersclustername-delete
  description: Deletes a cluster in a project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/dataproc.png
  humanURL: https://cloud.google.com/dataproc/
  baseURL: ://dataproc.googleapis.com//
  tags: Google APIs, Data, Stack Network, API Service Provider, API Provider, Databases,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/google-cloud-dataproc/v1projectsprojectidregionsregionclustersclustername-delete-openapi.md
- name: Google Cloud Dataproc - Get Cluster
  x-api-slug: v1projectsprojectidregionsregionclustersclustername-get
  description: Gets the resource representation for a cluster in a project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/dataproc.png
  humanURL: https://cloud.google.com/dataproc/
  baseURL: ://dataproc.googleapis.com//
  tags: Google APIs, Data, Stack Network, API Service Provider, API Provider, Databases,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/google-cloud-dataproc/v1projectsprojectidregionsregionclustersclustername-get-openapi.md
- name: Google Cloud Dataproc - Update Cluster
  x-api-slug: v1projectsprojectidregionsregionclustersclustername-patch
  description: Updates a cluster in a project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/dataproc.png
  humanURL: https://cloud.google.com/dataproc/
  baseURL: ://dataproc.googleapis.com//
  tags: Google APIs, Data, Stack Network, API Service Provider, API Provider, Databases,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/google-cloud-dataproc/v1projectsprojectidregionsregionclustersclustername-patch-openapi.md
- name: Google Cloud Dataproc - Get Cluster Diagnostic
  x-api-slug: v1projectsprojectidregionsregionclustersclusternamediagnose-post
  description: Gets cluster diagnostic information. After the operation completes,
    the Operation.response field contains DiagnoseClusterOutputLocation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/dataproc.png
  humanURL: https://cloud.google.com/dataproc/
  baseURL: ://dataproc.googleapis.com//
  tags: Google APIs, Data, Stack Network, API Service Provider, API Provider, Databases,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cluster/master/_listings/google-cloud-dataproc/v1projectsprojectidregionsregionclustersclusternamediagnose-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.container.builder.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.cloud.dataproc.stack.network
- type: x-change-logs
  url: https://cloud.google.com/dataproc/docs/release-notes/service
- type: x-documentation
  url: https://cloud.google.com/dataproc/docs/
- type: x-faq
  url: https://cloud.google.com/dataproc/docs/resources/faq
- type: x-getting-started
  url: https://cloud.google.com/dataproc/docs/quickstarts
- type: x-guides
  url: https://cloud.google.com/dataproc/docs/how-to
- type: x-partners
  url: https://cloud.google.com/dataproc/docs/resources/partners
- type: x-pricing
  url: https://cloud.google.com/dataproc/docs/resources/pricing
- type: x-rate-limits
  url: https://cloud.google.com/dataproc/quotas
- type: x-sdk
  url: https://cloud.google.com/dataproc/docs/gcloud-installation
- type: x-service-level-agreements
  url: https://cloud.google.com/dataproc/docs/resources/sla
- type: x-support
  url: https://cloud.google.com/dataproc/docs/support/get-support
- type: x-website
  url: https://cloud.google.com/dataproc/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---