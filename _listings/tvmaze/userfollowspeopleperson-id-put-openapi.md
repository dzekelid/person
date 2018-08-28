---
swagger: "2.0"
x-collection-name: TVmaze
x-complete: 0
info:
  title: TVmaze user Put User Follows People Person
  description: Put user follows people person.
  version: "1.0"
host: api.tvmaze.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/follows/people/{person_id}:
    delete:
      summary: Delete User Follows People Person
      description: Delete user follows people person.
      operationId: deleteUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - People
      - Person
    get:
      summary: Get User Follows People Person
      description: Get user follows people person.
      operationId: getUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - People
      - Person
    parameters:
      summary: Parameters User Follows People Person
      description: Parameters user follows people person.
      operationId: parametersUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Follows
      - People
      - Person
    put:
      summary: Put User Follows People Person
      description: Put user follows people person.
      operationId: putUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-put
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - People
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