swagger: "2.0"
x-collection-name: EhrScape
x-complete: 1
info:
  title: EhrScape Terminology APIs
  description: validates-and-resolves-terminology-codes
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /terminology-adapter/rest
paths:
  /view/{ehrId}/weight:
    get:
      summary: Gets recorded weights for a patient
      description: Gets recorded weights for a patient.
      operationId: get_weight
      x-api-path-slug: viewehridweight-get
      parameters:
      - in: path
        name: ehrId
        description: EHR ID
      - in: query
        name: from
        description: Limit by date from
      - in: query
        name: limit
        description: Maximum number of results to return (default = 10, max = 100)
      - in: query
        name: to
        description: Limit by date to
      responses:
        200:
          description: OK
      tags:
      - View
      - EhrId
      - Weight