swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 1
info:
  title: AWS CloudFormation API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListExports:
    get:
      summary: List Exports
      description: Lists all exported output values in the account and region in which
        you call this action.
      operationId: listExports
      x-api-path-slug: actionlistexports-get
      parameters:
      - in: query
        name: NextToken
        description: A string (provided by the ListExports response output) that        identifies
          the next page of exported output values that you asked to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Exports