---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 0
info:
  title: AWS OpsWorks API Describe Commands
  version: 1.0.0
  description: Describes the results of specified commands.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeCommands:
    get:
      summary: Describe Commands
      description: Describes the results of specified commands.
      operationId: describeCommands
      x-api-path-slug: actiondescribecommands-get
      parameters:
      - in: query
        name: CommandIds
        description: An array of command IDs
        type: string
      - in: query
        name: DeploymentId
        description: The deployment ID
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Commands
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