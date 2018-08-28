swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeExportTasks:
    get:
      summary: Describe Export Tasks
      description: Describes one or more of your export tasks.
      operationId: describeexporttasks
      x-api-path-slug: actiondescribeexporttasks-get
      parameters:
      - in: query
        name: AmazonProvidedIpv6CidrBlock
        description: Requests an Amazon-provided IPv6 CIDR block with a /56 prefix
          length for the VPC
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Export Takss
  /?Action=CancelExportTask:
    get:
      summary: Cancel Export Task
      description: Cancels an active export task.
      operationId: cancelexporttask
      x-api-path-slug: actioncancelexporttask-get
      parameters:
      - in: query
        name: Description
        description: A description for the conversion task or the resource being exported
        type: string
      - in: query
        name: ExportToS3
        description: The format and location for an instance export task
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: TargetEnvironment
        description: The target virtualization environment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Export Task
  /?Action=CreateInstanceExportTask:
    get:
      summary: Create Instance Export Task
      description: Exports a running or stopped instance to an S3 bucket.
      operationId: createinstanceexporttask
      x-api-path-slug: actioncreateinstanceexporttask-get
      parameters:
      - in: query
        name: ExportTaskId.N
        description: One or more export task IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Export Task