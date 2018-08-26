---
swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 0
info:
  title: Webex Teams Admin API Get Person Details1
  description: |-
    Shows details for a person, by ID.
    Specify the person ID in the personId parameter in the URI.

    https://developer.webex.com/endpoint-people-personId-get.html
  version: 1.0.0
host: api.ciscospark.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /people/{_person}:
    get:
      summary: Get Person Details1
      description: |-
        Shows details for a person, by ID.
        Specify the person ID in the personId parameter in the URI.

        https://developer.webex.com/endpoint-people-personId-get.html
      operationId: PeopleByPersonGet2
      x-api-path-slug: people-person-get
      parameters:
      - in: path
        name: _person
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Person
      - Details1
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