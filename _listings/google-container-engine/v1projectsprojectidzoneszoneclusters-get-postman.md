{
  "info": {
    "name": "Google Container Engine API Get Clusters",
    "_postman_id": "47ecb986-ae25-41ab-b862-08434812fb72",
    "description": "Lists all clusters owned by a project in either the specified zone or all zones.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cluster",
      "item": [
        {
          "id": "bd147e59-4ee5-4dff-ab39-d6296aed9a6e",
          "name": "container.projects.zones.clusters.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "container.googleapis.com",
              "path": [
                "v1/projects/:projectId/zones/:zone/clusters"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "zone",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all clusters owned by a project in either the specified zone or all zones."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e45a115b-bfc3-4c2c-88cd-19844bcd78cb"
            }
          ]
        }
      ]
    }
  ]
}