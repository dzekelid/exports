---
swagger: "2.0"
x-collection-name: OpenDataSoft
x-complete: 0
info:
  title: OpenDataSoft Get Source Datasets Dataset Exports Json
  description: Export dataset in JSON format
  version: 2.1.0
host: public.opendatasoft.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{source}/datasets/{dataset_id}/exports/csv:
    get:
      summary: Get Source Datasets Dataset Exports Csv
      description: Export dataset in CSV format
      operationId: exportRecordsCSV
      x-api-path-slug: sourcedatasetsdataset-idexportscsv-get
      parameters:
      - in: query
        name: delimiter
        description: Provide a different delimiter (default ,)
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Datasets
      - Dataset
      - Id
      - Exports
      - Csv
  /{source}/datasets/{dataset_id}/exports/geojson:
    get:
      summary: Get Source Datasets Dataset Exports Geojson
      description: Export dataset in GEOJSON format
      operationId: exportRecordsGEOJSON
      x-api-path-slug: sourcedatasetsdataset-idexportsgeojson-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Datasets
      - Dataset
      - Id
      - Exports
      - Geojson
  /{source}/datasets/{dataset_id}/exports/ical:
    get:
      summary: Get Source Datasets Dataset Exports Ical
      description: Export dataset in ICAL format
      operationId: exportRecordsICAL
      x-api-path-slug: sourcedatasetsdataset-idexportsical-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Datasets
      - Dataset
      - Id
      - Exports
      - Ical
  /{source}/datasets/{dataset_id}/exports/json:
    get:
      summary: Get Source Datasets Dataset Exports Json
      description: Export dataset in JSON format
      operationId: exportRecordsJSON
      x-api-path-slug: sourcedatasetsdataset-idexportsjson-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Datasets
      - Dataset
      - Id
      - Exports
      - Json
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