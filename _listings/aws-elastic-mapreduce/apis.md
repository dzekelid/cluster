---
name: AWS Elastic MapReduce
description: Amazon EMR provides a managed Hadoop framework that makes it easy, fast,
  and cost-effective to process vast amounts of data across dynamically scalable Amazon
  EC2 instances. You can also run other popular distributed frameworks such as Apache
  Spark, HBase, Presto, and Flink in Amazon EMR, and interact with data in other AWS
  data stores such as Amazon S3 and Amazon DynamoDB.nAmazon EMR securely and reliably
  handles a broad set of big data use cases, including log analysis, web indexing,
  data transformations (ETL), machine learning, financial analysis, scientific simulation,
  and bioinformatics.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonEMR.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Stack Network
- MapReduce
- Database
- Data
- Amazon Web Services
created: "2018-03-13"
modified: "2018-03-13"
url: https://raw.githubusercontent.com/streamdata-gallery/cluster/master/_listings/aws-elastic-mapreduce/apis.yaml
specificationVersion: "0.14"
apis:
- name: AWS Elastic MapReduce API
  description: Amazon EMR provides a managed Hadoop framework that makes it easy,
    fast, and cost-effective to process vast amounts of data across dynamically scalable
    Amazon EC2 instances
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonEMR.png
  humanURL: ""
  baseURL: :///
  tags: Cluster
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/cluster/master/_listings/aws-elastic-mapreduce/action-describecluster-get.md
x-common:
- type: x-article
  url: http://aws.amazon.com/articles/Elastic-MapReduce
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/ElasticMapReduce/latest/DeveloperGuide/emr-cli-reference.html
- type: x-faq
  url: https://aws.amazon.com/emr/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/emr/getting-started/
- type: x-partners
  url: https://aws.amazon.com/emr/partners/
- type: x-pricing
  url: https://aws.amazon.com/emr/pricing/
- type: x-documentation
  url: http://docs.aws.amazon.com/ElasticMapReduce/latest/API/
- type: x-website
  url: https://aws.amazon.com/emr/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---