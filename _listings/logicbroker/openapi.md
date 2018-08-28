swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Shipments/Export:
    get:
      summary: Export to CSV/XLSX
      description: "The 'fields' parameter accepts a comma delimited list of JSON
        paths, for example: 'Identifier.logicbrokerKey, BillToAddress.FirstName'.
        It is also possible to rename these fields using syntax like 'DocumentDate
        as Date' or 'DocumentDate Date'.\r\n            You must specify a value for
        either the 'LogicbrokerKeys' parameter or the 'filter' parameter."
      operationId: Shipment_GetDocumentExportToken
      x-api-path-slug: apiv1shipmentsexport-get
      parameters:
      - in: query
        name: delimiter
        description: The column delimiter to use for CSV export
      - in: query
        name: fields
        description: The fields to export
      - in: query
        name: fileType
        description: Valid options are csv, xlsx, xml, json and legacy
      - in: query
        name: filter.advanced
        description: Advanced query options
      - in: query
        name: filter.from
        description: Beginning of time search window
      - in: query
        name: filter.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: filter.page
        description: Page number
      - in: query
        name: filter.pageSize
        description: Page size
      - in: query
        name: filter.partnerPO
        description: The partners purchase order number
      - in: query
        name: filter.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: filter.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: filter.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: filter.status
        description: The status of the document
      - in: query
        name: filter.to
        description: End of time search window
      - in: query
        name: LogicbrokerKeys
        description: The logicbroker keys
      responses:
        200:
          description: OK
      tags:
      - Export
      - To
      - CSV
      - XLSX
  /api/v1/Returns/Export:
    get:
      summary: Export to CSV/XLSX
      description: "The 'fields' parameter accepts a comma delimited list of JSON
        paths, for example: 'Identifier.LogicbrokerKey, BillToAddress.FirstName'.
        It is also possible to rename these fields using syntax like 'DocumentDate
        as Date' or 'DocumentDate Date'.\r\n            You must specify a value for
        either the 'LogicbrokerKeys' parameter or the 'filter' parameter."
      operationId: Return_GetDocumentExportToken
      x-api-path-slug: apiv1returnsexport-get
      parameters:
      - in: query
        name: delimiter
        description: The column delimiter to use for CSV export
      - in: query
        name: fields
        description: The fields to export
      - in: query
        name: fileType
        description: Valid options are csv, xlsx, xml, and json
      - in: query
        name: filter.advanced
        description: Advanced query options
      - in: query
        name: filter.from
        description: Beginning of time search window
      - in: query
        name: filter.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: filter.page
        description: Page number
      - in: query
        name: filter.pageSize
        description: Page size
      - in: query
        name: filter.partnerPO
        description: The partners purchase order number
      - in: query
        name: filter.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: filter.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: filter.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: filter.status
        description: The status of the document
      - in: query
        name: filter.to
        description: End of time search window
      - in: query
        name: LogicbrokerKeys
        description: The logicbroker keys
      responses:
        200:
          description: OK
      tags:
      - Export
      - To
      - CSV
      - XLSX
  /api/v1/Orders/Export:
    get:
      summary: Export to CSV/XLSX
      description: "The 'fields' parameter accepts a comma delimited list of JSON
        paths, for example: 'Identifier.logicbrokerKey, BillToAddress.FirstName'.
        It is also possible to rename these fields using syntax like 'DocumentDate
        as Date' or 'DocumentDate Date'.\r\n            You must specify a value for
        either the 'LogicbrokerKeys' parameter or the 'filter' parameter."
      operationId: Order_GetDocumentExportToken
      x-api-path-slug: apiv1ordersexport-get
      parameters:
      - in: query
        name: Delimiter
        description: The column delimiter to use for CSV export
      - in: query
        name: Fields
        description: The fields to export
      - in: query
        name: FileType
        description: Valid options are csv, xlsx, xml, json and legacy
      - in: query
        name: Filter.advanced
        description: Advanced query options
      - in: query
        name: Filter.from
        description: Beginning of time search window
      - in: query
        name: Filter.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: Filter.page
        description: Page number
      - in: query
        name: Filter.pageSize
        description: Page size
      - in: query
        name: Filter.partnerPO
        description: The partners purchase order number
      - in: query
        name: Filter.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: Filter.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: Filter.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: Filter.status
        description: The status of the document
      - in: query
        name: Filter.to
        description: End of time search window
      - in: query
        name: LogicbrokerKeys
        description: The logicbroker keys
      responses:
        200:
          description: OK
      tags:
      - Export
      - To
      - CSV
      - XLSX
  /api/v1/Invoices/Export:
    get:
      summary: Export to CSV/XLSX
      description: "The 'fields' parameter accepts a comma delimited list of JSON
        paths, for example: 'Identifier.LogicbrokerKey, BillToAddress.FirstName'.
        It is also possible to rename these fields using syntax like 'DocumentDate
        as Date' or 'DocumentDate Date'.\r\n            You must specify a value for
        either the 'LogicbrokerKeys' parameter or the 'filter' parameter."
      operationId: Invoice_GetDocumentExportToken
      x-api-path-slug: apiv1invoicesexport-get
      parameters:
      - in: query
        name: delimiter
        description: The column delimiter to use for CSV export
      - in: query
        name: fields
        description: The fields to export
      - in: query
        name: fileType
        description: Valid options are csv, xlsx, xml, json and legacy
      - in: query
        name: filter.advanced
        description: Advanced query options
      - in: query
        name: filter.from
        description: Beginning of time search window
      - in: query
        name: filter.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: filter.page
        description: Page number
      - in: query
        name: filter.pageSize
        description: Page size
      - in: query
        name: filter.partnerPO
        description: The partners purchase order number
      - in: query
        name: filter.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: filter.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: filter.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: filter.status
        description: The status of the document
      - in: query
        name: filter.to
        description: End of time search window
      - in: query
        name: LogicbrokerKeys
        description: The logicbroker keys
      responses:
        200:
          description: OK
      tags:
      - Export
      - To
      - CSV
      - XLSX
  /api/v1/Acknowledgements/Export:
    get:
      summary: Export to CSV/XLSX
      description: "The 'fields' parameter accepts a comma delimited list of JSON
        paths, for example: 'Identifier.LogicbrokerKey, BillToAddress.FirstName'.
        It is also possible to rename these fields using syntax like 'DocumentDate
        as Date' or 'DocumentDate Date'.\r\n            You must specify a value for
        either the 'LogicbrokerKeys' parameter or the 'filter' parameter."
      operationId: Acknowledgement_GetDocumentExportToken
      x-api-path-slug: apiv1acknowledgementsexport-get
      parameters:
      - in: query
        name: delimiter
        description: The column delimiter to use for CSV export
      - in: query
        name: fields
        description: The fields to export
      - in: query
        name: fileType
        description: Valid options are csv, xlsx, xml, json and legacy
      - in: query
        name: filter.advanced
        description: Advanced query options
      - in: query
        name: filter.from
        description: Beginning of time search window
      - in: query
        name: filter.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: filter.page
        description: Page number
      - in: query
        name: filter.pageSize
        description: Page size
      - in: query
        name: filter.partnerPO
        description: The partners purchase order number
      - in: query
        name: filter.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: filter.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: filter.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: filter.status
        description: The status of the document
      - in: query
        name: filter.to
        description: End of time search window
      - in: query
        name: LogicbrokerKeys
        description: The logicbroker keys
      responses:
        200:
          description: OK
      tags:
      - Export
      - To
      - CSV
      - XLSX