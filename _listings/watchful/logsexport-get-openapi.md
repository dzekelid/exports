---
swagger: "2.0"
x-collection-name: Watchful
x-complete: 0
info:
  title: Watchful Get A CSV Or PDF File Contain The List Of Logs
  description: Returns a file contain the list of logs
  version: 1.0.0
host: watchful.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /logs/export:
    get:
      summary: Get A CSV Or PDF File Contain The List Of Logs
      description: Returns a file contain the list of logs
      operationId: getExportLogs
      x-api-path-slug: logsexport-get
      parameters:
      - in: query
        name: enddate
        description: Logs before this date, format YYYY-MM-DD HH:MM:SS
      - in: query
        name: filter_type
        description: Type of the log
      - in: query
        name: format
        description: Format of exported file (PDF or CSV)
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: search
        description: Do a LIKE search, you can also use %
      - in: query
        name: site
        description: Site id of the log
      - in: query
        name: startdate
        description: Logs after this date, format YYYY-MM-DD HH:MM:SS
      - in: query
        name: startid
        description: Start of the return (default 0)
      responses:
        200:
          description: OK
      tags:
      - Logs
      - Export
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