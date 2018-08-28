---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Ticket Eventid Export
  version: 1.0.0
  description: Get ticket eventid export.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/ticket/{eventId}/export:
    get:
      summary: Get Ticket Eventid Export
      description: Get ticket eventid export.
      operationId: getApiV1TicketEventExport
      x-api-path-slug: apiv1ticketeventidexport-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      - in: query
        name: from
      - in: query
        name: to
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Eventid
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