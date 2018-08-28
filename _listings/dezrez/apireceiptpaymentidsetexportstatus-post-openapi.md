---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Change status export status of payment
  version: 1.0.0
  description: Change status export status of payment.
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
  /api/accounting/exports/batchexport:
    post:
      summary: Get details for batch payment export
      description: Get details for batch payment export.
      operationId: AccountingExport_SetBatchPaymentExportBydataContract
      x-api-path-slug: apiaccountingexportsbatchexport-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detailsbatch
      - Payment
      - Export
  /api/accounting/exports/batch/{id}/removepayment:
    put:
      summary: Remove an individual payment from batch export
      description: Remove an individual payment from batch export.
      operationId: AccountingExport_RemoveFromBatchByidBypaymentId
      x-api-path-slug: apiaccountingexportsbatchidremovepayment-put
      parameters:
      - in: path
        name: id
      - in: query
        name: paymentId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Individual
      - Payment
      - From
      - Batch
      - Export
  /api/receipt/payment/{id}/setexportstatus:
    post:
      summary: Change status export status of payment
      description: Change status export status of payment.
      operationId: Receipt_SetPaymentExportStatusByidBystatusDataContract
      x-api-path-slug: apireceiptpaymentidsetexportstatus-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: statusDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Change
      - Status
      - Export
      - Status
      - Of
      - Payment
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