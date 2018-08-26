---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Get Person
  description: |-
    Returns a user or multiple users by their ID(s). Batch request is supported.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Light
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/glip/persons/{personId}:
    get:
      summary: Get Person
      description: |-
        Returns a user or multiple users by their ID(s). Batch request is supported.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Light
      operationId: loadGlipPerson
      x-api-path-slug: restapiv1-0glippersonspersonid-get
      parameters:
      - in: path
        name: personId
        description: Internal identifier of a user to be returned, the maximum number
          of IDs is 30
      responses:
        200:
          description: OK
      tags:
      - Person
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