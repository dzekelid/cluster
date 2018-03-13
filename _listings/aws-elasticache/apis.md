---
name: AWS ElastiCache
description: Amazon ElastiCache is a web service that makes it easy to deploy, operate,
  and scale an in-memory data store or cache in the cloud. The service improves the
  performance of web applications by allowing you to retrieve information from fast,
  managed, in-memory data stores, instead of relying entirely on slower disk-based
  databases. Amazon ElastiCache automatically detects and replaces failed nodes, reducing
  the overhead associated with self-managed infrastructures and provides a resilient
  system that mitigates the risk of overloaded databases, which slow website and application
  load times. Through integration with Amazon CloudWatch, Amazon ElastiCache provides
  enhanced visibility into key performance metrics associated with your Redis or Memcached
  nodes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Stack Network
- Performance
- Cache
- Availability
- Amazon Web Services
created: "2018-03-13"
modified: "2018-03-13"
url: https://raw.githubusercontent.com/streamdata-gallery/cluster/master/_listings/aws-elasticache/apis.yaml
specificationVersion: "0.14"
apis:
- name: Amazon ElastiCache API
  description: Amazon ElastiCache is a web service that makes it easy to deploy, operate,
    and scale an in-memory data store or cache in the cloud
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: ""
  baseURL: :///
  tags: Cluster
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/cluster/master/_listings/aws-elasticache/action-modifycachecluster-get.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/AmazonElastiCache/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/elasticache/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/elasticache/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/elasticache/pricing/
- type: x-resources
  url: https://aws.amazon.com/elasticache/developer-resources/
- type: x-testimonials
  url: https://aws.amazon.com/elasticache/testimonials/
- type: x-website
  url: https://aws.amazon.com/elasticache/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---