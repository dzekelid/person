---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API Show contributions of a certain type
    by a person
  description: Given a resource (dataset, report, etc.) and a role (editor, etc),
    and an identifier for a person, show the resources to which the person has contributed
    in that role.
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /person/{name}:
    get:
      summary: Redirect to a person based on a name
      description: Given a name (case sensitive, concatenated by dashes), redirect
        if there is a single match.  The first and last names can be in either order.
      operationId: given-a-name-case-sensitive-concatenated-by-dashes-redirect-if-there-is-a-single-match--the-first-an
      x-api-path-slug: personname-get
      parameters:
      - in: path
        name: name
        description: name description
      responses:
        200:
          description: OK
      tags:
      - Redirect
      - To
      - Person
      - Based
      - "On"
      - Name
  /person/{orcid}:
    get:
      summary: Redirect to a person based on an ORCID.
      description: Given an ORCID, if there is a match, redirect to the persons URI.
      operationId: given-an-orcid-if-there-is-a-match-redirect-to-the-persons-uri
      x-api-path-slug: personorcid-get
      parameters:
      - in: path
        name: orcid
        description: orcid description
      responses:
        200:
          description: OK
      tags:
      - Redirect
      - To
      - Person
      - Based
      - "On"
      - ORCID
  /person/{person_identifier}:
    get:
      summary: Get a representation of a person.
      description: Get JSON which represents the structure of a person.
      operationId: get-json-which-represents-the-structure-of-a-person
      x-api-path-slug: personperson-identifier-get
      parameters:
      - in: path
        name: person_identifier
        description: person_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Person
  /person/{person_identifier}/contributions/{role_type_identifier}/{resource}:
    get:
      summary: Show contributions of a certain type by a person
      description: Given a resource (dataset, report, etc.) and a role (editor, etc),
        and an identifier for a person, show the resources to which the person has
        contributed in that role.
      operationId: given-a-resource-dataset-report-etc-and-a-role-editor-etc-and-an-identifier-for-a-person-show-the-re
      x-api-path-slug: personperson-identifiercontributionsrole-type-identifierresource-get
      parameters:
      - in: path
        name: person_identifier
        description: person_identifier description
      - in: path
        name: resource
        description: resource description
      - in: path
        name: role_type_identifier
        description: role_type_identifier description
      responses:
        200:
          description: OK
      tags:
      - Show
      - Contributions
      - Certain
      - Type
      - By
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