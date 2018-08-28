swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
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