---
swagger: "2.0"
x-collection-name: Google Container Engine
x-complete: 0
info:
  title: Google Container Engine API Get Clusters
  description: Lists all clusters owned by a project in either the specified zone
    or all zones.
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