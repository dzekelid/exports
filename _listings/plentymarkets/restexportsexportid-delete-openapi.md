---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Delete export
  description: Deletes an export. The ID of the export must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/exports:
    get:
      summary: List elastic exports
      description: Lists elastic exports.
      operationId: getRestExports
      x-api-path-slug: restexports-get
      parameters:
      - in: query
        name: formatKey
        description: The format of the export
      - in: query
        name: id
        description: The ID of the export
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: name
        description: The name of the export
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: type
        description: The type of the export
      responses:
        200:
          description: OK
      tags:
      - List
      - Elastic
      - Exports
    post:
      summary: Create an export
      description: Creates an export.
      operationId: postRestExports
      x-api-path-slug: restexports-post
      parameters:
      - in: body
        name: /rest/exports
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Export
  /rest/exports/{exportId}:
    delete:
      summary: Delete export
      description: Deletes an export. The ID of the export must be specified.
      operationId: deleteRestExportsExport
      x-api-path-slug: restexportsexportid-delete
      parameters:
      - in: path
        name: exportId
      responses:
        200:
          description: OK
      tags:
      - Export
    get:
      summary: Get export
      description: Gets detailed information about an export. The ID of the export
        must be specified.
      operationId: getRestExportsExport
      x-api-path-slug: restexportsexportid-get
      parameters:
      - in: path
        name: exportId
      responses:
        200:
          description: OK
      tags:
      - Export
    put:
      summary: Update an export
      description: Updates an export. The ID of the export must be specified.
      operationId: putRestExportsExport
      x-api-path-slug: restexportsexportid-put
      parameters:
      - in: body
        name: /rest/exports/{exportId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: exportId
      responses:
        200:
          description: OK
      tags:
      - Export
  /rest/orders/shipping/export_documents/{orderId}:
    get:
      summary: List export documents by order ID
      description: List export documents by order id.
      operationId: getRestOrdersShippingExportDocumentsOrder
      x-api-path-slug: restordersshippingexport-documentsorderid-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Export
      - Documents
      - By
      - Order
      - ID
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