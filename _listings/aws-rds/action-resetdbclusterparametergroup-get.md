---
swagger: "2.0"
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ResetDBClusterParameterGroup&k=1:
    get:
      summary: Reset D B Cluster Parameter Group
      description: Modifies the parameters of a DB cluster parameter group to the
        default value
      operationId: resetdbclusterparametergroup
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to reset
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: A list of parameter names in the DB cluster parameter group to
          reset to the default values
        type: string
      - in: query
        name: ResetAllParameters
        description: A value that is set to true to reset all parameters in the DB
          cluster parameter group       to their default values, and false otherwise
        type: string
      responses:
        200:
          description: OK
      tags:
      - cluster parameter groups
definitions: []
x-collection-name: AWS RDS
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