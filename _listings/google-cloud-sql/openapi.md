swagger: "2.0"
x-collection-name: Google Cloud SQL
x-complete: 1
info:
  title: Cloud SQL Administration
  description: creates-and-configures-cloud-sql-instances-which-provide-fullymanaged-mysql-databases-
  contact:
    name: Google
    url: https://google.com
  version: v1beta4
host: www.googleapis.com
basePath: /sql/v1beta4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{project}/instances/{instance}/export:
    post:
      summary: Add Projects Project Instances Instance Export
      description: Exports data from a Cloud SQL instance to a Google Cloud Storage
        bucket as a MySQL dump file.
      operationId: sql.instances.export
      x-api-path-slug: projectsprojectinstancesinstanceexport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance to be exported
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Export