{
  "info": {
    "name": "Google Cloud Dataproc API Get Region Clusters",
    "_postman_id": "fd3628b5-9782-490b-9f94-14f9f660e33e",
    "description": "Lists all regions/{region}/clusters in a project.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cluster",
      "item": [
        {
          "id": "5a6fd48d-dc8d-402d-832d-98ad80e98b6e",
          "name": "dataproc.projects.regions.clusters.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "dataproc.googleapis.com",
              "path": [
                "v1/projects/:projectId/regions/:region/clusters"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "region",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all regions/{region}/clusters in a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf562531-8ae6-4e94-bfc4-fd4fa671c45d"
            }
          ]
        }
      ]
    }
  ]
}