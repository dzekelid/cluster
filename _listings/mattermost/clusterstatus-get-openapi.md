---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get cluster status
  description: |-
    Get a set of information for each node in the cluster, useful for checking the status and health of each node.
    ##### Permissions
    Must have `manage_system` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cluster/status:
    get:
      summary: Get cluster status
      description: |-
        Get a set of information for each node in the cluster, useful for checking the status and health of each node.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: get-a-set-of-information-for-each-node-in-the-cluster-useful-for-checking-the-status-and-health-of-e
      x-api-path-slug: clusterstatus-get
      responses:
        200:
          description: OK
      tags:
      - Cluster
      - Status
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