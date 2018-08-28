---
swagger: "2.0"
x-collection-name: Botify
x-complete: 0
info:
  title: Botify Get Analyses Username Project Slug Analysis Slug Urls Export
  description: Get analyses username project slug analysis slug urls export.
  version: 1.0.0
host: api.botify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/export:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Urls Export
      description: Get analyses username project slug analysis slug urls export.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugUrlsExport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsexport-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Export
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls Export
      description: Parameters analyses username project slug analysis slug urls export.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrlsExport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsexport-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Export
    post:
      summary: Post Analyses Username Project Slug Analysis Slug Urls Export
      description: Creates a new UrlExport object and starts a task that will export
        the results into a csv. Returns the model id that manages the task
      operationId: postAnalysesUsernameProjectSlugAnalysisSlugUrlsExport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsexport-post
      parameters:
      - in: query
        name: area
        description: Analysis context
      - in: body
        name: UrlsQuery
        description: Urls query
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Export
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/export/{url_export_id}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Urls Export Url Export
      description: Checks the status of an CSVUrlExportJob object. Returns json object
        with the status.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugUrlsExportUrlExport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsexporturl-export-id-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Export
      - Url
      - Export
      - Id
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls Export
        Url Export
      description: Parameters analyses username project slug analysis slug urls export
        url export.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrlsExportUrlExport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsexporturl-export-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Export
      - Url
      - Export
      - Id
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