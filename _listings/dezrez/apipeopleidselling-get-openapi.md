---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get Selling Roles for a Person
  version: 1.0.0
  description: Get selling roles for a person.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/event/recordenquiry:
    post:
      summary: Records an event on the role representing a neg being in contact with
        a person
      description: Records an event on the role representing a neg being in contact
        with a person.
      operationId: Event_RecordEnquiryByrecordEnquiryDataContract
      x-api-path-slug: apieventrecordenquiry-post
      parameters:
      - in: body
        name: recordEnquiryDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Event
      - "On"
      - Role
      - Representing
      - Neg
      - Being
      - In
      - Contact
      - Person
  /api/identity/Get:
    get:
      summary: Gets all of the identities for the logged in person
      description: Gets all of the identities for the logged in person.
      operationId: Identity_GetLoggedInPersonIdentities
      x-api-path-slug: apiidentityget-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Of
      - Identitiesthe
      - Logged
      - In
      - Person
  /api/identity/Add:
    post:
      summary: Adds a new identity (E.g. Facebook Identity, Twitter identity etc.)
        to a person
      description: Adds a new identity (e.g. facebook identity, twitter identity etc.)
        to a person.
      operationId: Identity_AddIdentityToPersonBypersonIdByidentity
      x-api-path-slug: apiidentityadd-post
      parameters:
      - in: body
        name: identity
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: personId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Identity
      - (E
      - G
      - ""
      - Facebook
      - Identity
      - ""
      - Twitter
      - Identity
      - Etc
      - )
      - To
      - Person
  /api/identity/Remove:
    put:
      summary: Removes an identity (E.g. Facebook Identity, Twitter identity etc.)
        from a person
      description: Removes an identity (e.g. facebook identity, twitter identity etc.)
        from a person.
      operationId: Identity_RemoveIdentityFromPersonBypersonIdByidentityId
      x-api-path-slug: apiidentityremove-put
      parameters:
      - in: query
        name: identityId
      - in: query
        name: personId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Identity
      - (E
      - G
      - ""
      - Facebook
      - Identity
      - ""
      - Twitter
      - Identity
      - Etc
      - )
      - From
      - Person
  /api/negotiator/me:
    get:
      summary: Get a person by its Id
      description: Get a person by its id.
      operationId: Negotiator_GetLoggedInNegotiatorDetails
      x-api-path-slug: apinegotiatorme-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Person
      - By
      - Its
      - Id
  /api/people/{id}:
    get:
      summary: Get a person by its Id
      description: Get a person by its id.
      operationId: People_GetByid
      x-api-path-slug: apipeopleid-get
      parameters:
      - in: path
        name: id
        description: The id of the person to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Person
      - By
      - Its
      - Id
  /api/people/{id}/searching:
    get:
      summary: Get Searching Roles for a Person
      description: Get searching roles for a person.
      operationId: People_SearchingRolesByid
      x-api-path-slug: apipeopleidsearching-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Searching
      - Rolesa
      - Person
  /api/people/{id}/selling:
    get:
      summary: Get Selling Roles for a Person
      description: Get selling roles for a person.
      operationId: People_SellingRolesByid
      x-api-path-slug: apipeopleidselling-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Selling
      - Rolesa
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