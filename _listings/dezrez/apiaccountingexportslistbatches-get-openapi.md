---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get list of batch exports
  version: 1.0.0
  description: Get list of batch exports.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounting/exports/list/batches:
    get:
      summary: Get list of batch exports
      description: Get list of batch exports.
      operationId: AccountingExport_GetBatchPaymentsBybankAccountIdByincludeProcessed
      x-api-path-slug: apiaccountingexportslistbatches-get
      parameters:
      - in: query
        name: bankAccountId
      - in: query
        name: includeProcessed
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Batch
      - Exports
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