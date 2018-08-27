swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
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