---
swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 0
info:
  title: SalesLoft Update a person stage
  description: Updates a person stage.
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/people.json:
    post:
      summary: Create a person
      description: |-
        Creates a person. Either email_address or phone/last_name must be provided as a unique lookup
        on the team.
      operationId: v2.people.json.post
      x-api-path-slug: v2people-json-post
      parameters:
      - in: formData
        name: account_id
        description: ID of the Account to link this person to
      - in: formData
        name: autotag_date
        description: Whether the date should be added to this person as a tag
      - in: formData
        name: city
        description: City
      - in: formData
        name: country
        description: Country
      - in: formData
        name: custom_fields
        description: Custom fields are defined by the users team
      - in: formData
        name: do_not_contact
        description: Whether this person can not be contacted
      - in: formData
        name: email_address
        description: Email address
      - in: formData
        name: first_name
        description: First name
      - in: formData
        name: home_phone
        description: Home phone without formatting
      - in: formData
        name: import_id
        description: ID of the Import this person is a part of
      - in: formData
        name: last_name
        description: Last name
      - in: formData
        name: linkedin_url
        description: Linkedin URL
      - in: formData
        name: locale
        description: Time locale of the person
      - in: formData
        name: mobile_phone
        description: Mobile phone without formatting
      - in: formData
        name: owner_id
        description: ID of the User that owns this person
      - in: formData
        name: personal_email_address
        description: Personal email address
      - in: formData
        name: personal_website
        description: The website of this person
      - in: formData
        name: person_company_industry
        description: Company industry
      - in: formData
        name: person_company_name
        description: Company name
      - in: formData
        name: person_company_website
        description: Company website
      - in: formData
        name: person_stage_id
        description: ID of the PersonStage of this person
      - in: formData
        name: phone
        description: Phone without formatting
      - in: formData
        name: phone_extension
        description: Phone extension without formatting
      - in: formData
        name: secondary_email_address
        description: Alternate email address
      - in: formData
        name: state
        description: State
      - in: formData
        name: tags
        description: All tags applied to this person
      - in: formData
        name: title
        description: Job title
      - in: formData
        name: twitter_handle
        description: The twitter handle of this person
      - in: formData
        name: work_city
        description: Work location - city
      - in: formData
        name: work_country
        description: Work location - country
      - in: formData
        name: work_state
        description: Work location - state
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Person
  /v2/people/{id}.json:
    delete:
      summary: Delete a person
      description: |-
        Deletes a person. This operation is not reversible without contacting support.
        This operation can be called multiple times successfully.
      operationId: v2.people.id.json.delete
      x-api-path-slug: v2peopleid-json-delete
      parameters:
      - in: path
        name: id
        description: Person id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Person
    get:
      summary: Fetch a person
      description: Fetches a person, by ID only.
      operationId: v2.people.id.json.get
      x-api-path-slug: v2peopleid-json-get
      parameters:
      - in: path
        name: id
        description: Person ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Person
    put:
      summary: Update a person
      description: Updates a person.
      operationId: v2.people.id.json.put
      x-api-path-slug: v2peopleid-json-put
      parameters:
      - in: formData
        name: account_id
        description: ID of the Account to link this person to
      - in: formData
        name: city
        description: City
      - in: formData
        name: country
        description: Country
      - in: formData
        name: custom_fields
        description: Custom fields are defined by the users team
      - in: formData
        name: do_not_contact
        description: Whether this person can not be contacted
      - in: formData
        name: email_address
        description: Email address
      - in: formData
        name: first_name
        description: First name
      - in: formData
        name: home_phone
        description: Home phone without formatting
      - in: path
        name: id
        description: Person id
      - in: formData
        name: import_id
        description: ID of the Import this person is a part of
      - in: formData
        name: last_name
        description: Last name
      - in: formData
        name: linkedin_url
        description: Linkedin URL
      - in: formData
        name: locale
        description: Time locale of the person
      - in: formData
        name: mobile_phone
        description: Mobile phone without formatting
      - in: formData
        name: owner_id
        description: ID of the User that owns this person
      - in: formData
        name: personal_email_address
        description: Personal email address
      - in: formData
        name: personal_website
        description: The website of this person
      - in: formData
        name: person_company_industry
        description: Company industry
      - in: formData
        name: person_company_name
        description: Company name
      - in: formData
        name: person_company_website
        description: Company website
      - in: formData
        name: person_stage_id
        description: ID of the PersonStage of this person
      - in: formData
        name: phone
        description: Phone without formatting
      - in: formData
        name: phone_extension
        description: Phone extension without formatting
      - in: formData
        name: secondary_email_address
        description: Alternate email address
      - in: formData
        name: state
        description: State
      - in: formData
        name: tags
        description: All tags applied to this person
      - in: formData
        name: title
        description: Job title
      - in: formData
        name: twitter_handle
        description: The twitter handle of this person
      - in: formData
        name: work_city
        description: Work location - city
      - in: formData
        name: work_country
        description: Work location - country
      - in: formData
        name: work_state
        description: Work location - state
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Person
  /v2/person_stages.json:
    get:
      summary: List person stages
      description: |-
        Fetches multiple person stage records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.person_stages.json.get
      x-api-path-slug: v2person-stages-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of person stages to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Person
      - Stages
    post:
      summary: Create a person stage
      description: Creates a person stage.
      operationId: v2.person_stages.json.post
      x-api-path-slug: v2person-stages-json-post
      parameters:
      - in: formData
        name: name
        description: The name of the new stage
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Person
      - Stage
  /v2/person_stages/{id}.json:
    delete:
      summary: Delete an person stage
      description: |-
        Deletes a person stage. This operation is not reversible without contacting support.
        This operation can be called multiple times successfully.
      operationId: v2.person_stages.id.json.delete
      x-api-path-slug: v2person-stagesid-json-delete
      parameters:
      - in: path
        name: id
        description: Stage ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Person
      - Stage
    get:
      summary: Fetch a person stage
      description: Fetches a person stage, by ID only.
      operationId: v2.person_stages.id.json.get
      x-api-path-slug: v2person-stagesid-json-get
      parameters:
      - in: path
        name: id
        description: Stage ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Person
      - Stage
    put:
      summary: Update a person stage
      description: Updates a person stage.
      operationId: v2.person_stages.id.json.put
      x-api-path-slug: v2person-stagesid-json-put
      parameters:
      - in: path
        name: id
        description: Stage ID
      - in: formData
        name: name
        description: The name of the stage
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Person
      - Stage
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