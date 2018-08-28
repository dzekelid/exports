swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /audit/export:
    get:
      summary: Export audit records
      description: "Exports audit records as a CSV file or ZIP file.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission."
      operationId: com.atlassian.confluence.plugins.restapi.resources.AuditResource.exportAuditRecords_get
      x-api-path-slug: auditexport-get
      parameters:
      - in: query
        name: endDate
        description: Filters the exported results to the records on or before the
          `endDate`
      - in: query
        name: format
        description: The format of the export file for the audit records
      - in: query
        name: searchString
        description: Filters the exported results to records that have string property
          values matching the `searchString`
      - in: query
        name: startDate
        description: Filters the exported results to the records on or after the `startDate`
      responses:
        200:
          description: OK
      tags:
      - Export
      - Audit
      - Records