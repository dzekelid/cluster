---
swagger: "2.0"
x-collection-name: Google Container Engine
x-complete: 0
info:
  title: Google Container Engine API Update Cluster
  description: Updates the settings of a specific cluster.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: container.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}/zones/{zone}/clusters:
    get:
      summary: Get Clusters
      description: Lists all clusters owned by a project in either the specified zone
        or all zones.
      operationId: container.projects.zones.clusters.list
      x-api-path-slug: v1projectsprojectidzoneszoneclusters-get
      parameters:
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides, or - for all zones
      responses:
        200:
          description: OK
      tags:
      - Cluster
    post:
      summary: Create Cluster
      description: Creates a cluster, consisting of the specified number and type
        of Google Compute Engine instances. By default, the cluster is created in
        the project's [default network](/compute/docs/networks-and-firewalls#networks).
        One firewall is added for the cluster. After cluster creation, the cluster
        creates routes for each node to allow the containers on that node to communicate
        with all other instances in the cluster. Finally, an entry is added to the
        project's global metadata indicating which CIDR range is being used by the
        cluster.
      operationId: container.projects.zones.clusters.create
      x-api-path-slug: v1projectsprojectidzoneszoneclusters-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Cluster
  /v1/projects/{projectId}/zones/{zone}/clusters/{clusterId}:
    delete:
      summary: Delete Cluster
      description: Deletes the cluster, including the Kubernetes endpoint and all
        worker nodes. Firewalls and routes that were configured during cluster creation
        are also deleted. Other Google Compute Engine resources that might be in use
        by the cluster (e.g. load balancer resources) will not be deleted if they
        weren't present at the initial create time.
      operationId: container.projects.zones.clusters.delete
      x-api-path-slug: v1projectsprojectidzoneszoneclustersclusterid-delete
      parameters:
      - in: path
        name: clusterId
        description: The name of the cluster to delete
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Cluster
    get:
      summary: Get Cluster
      description: Gets the details of a specific cluster.
      operationId: container.projects.zones.clusters.get
      x-api-path-slug: v1projectsprojectidzoneszoneclustersclusterid-get
      parameters:
      - in: path
        name: clusterId
        description: The name of the cluster to retrieve
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Cluster
    put:
      summary: Update Cluster
      description: Updates the settings of a specific cluster.
      operationId: container.projects.zones.clusters.update
      x-api-path-slug: v1projectsprojectidzoneszoneclustersclusterid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: clusterId
        description: The name of the cluster to upgrade
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Cluster
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