---
swagger: "2.0"
x-collection-name: OpenDataSoft
x-complete: 0
info:
  title: OpenDataSoft Get Source Exports Rss
  description: Export catalog (source) in RSS format
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
  /{source}/datasets/{dataset_id}/exports/ov2:
    get:
      summary: Get Source Datasets Dataset Exports Ov2
      description: Export dataset in OV2 format
      operationId: exportRecordsOV2
      x-api-path-slug: sourcedatasetsdataset-idexportsov2-get
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
      - Ov2
  /{source}/datasets/{dataset_id}/exports/shp:
    get:
      summary: Get Source Datasets Dataset Exports Shp
      description: Export dataset in Esri shapefile (shp) format
      operationId: exportRecordsSHP
      x-api-path-slug: sourcedatasetsdataset-idexportsshp-get
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
      - Shp
  /{source}/datasets/{dataset_id}/exports/xls:
    get:
      summary: Get Source Datasets Dataset Exports Xls
      description: Export dataset in XLS (Excel) format
      operationId: exportRecordsXLS
      x-api-path-slug: sourcedatasetsdataset-idexportsxls-get
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
      - Xls
  /{source}/exports/csv:
    get:
      summary: Get Source Exports Csv
      description: Export catalog (source) in CSV format
      operationId: exportDatasetsCSV
      x-api-path-slug: sourceexportscsv-get
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
      - Exports
      - Csv
  /{source}/exports/json:
    get:
      summary: Get Source Exports Json
      description: Export catalog (source) in JSON format
      operationId: exportDatasetsJson
      x-api-path-slug: sourceexportsjson-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Exports
      - Json
  /{source}/exports/rdf:
    get:
      summary: Get Source Exports Rdf
      description: Export catalog (source) in RDF/XML format
      operationId: exportDatasetsRDF
      x-api-path-slug: sourceexportsrdf-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Exports
      - Rdf
  /{source}/exports/rss:
    get:
      summary: Get Source Exports Rss
      description: Export catalog (source) in RSS format
      operationId: exportDatasetsRSS
      x-api-path-slug: sourceexportsrss-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Exports
      - Rss
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