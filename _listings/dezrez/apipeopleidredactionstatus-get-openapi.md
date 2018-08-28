---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Redaction Status for a Person by PersonId
  version: 1.0.0
  description: Redaction status for a person by personid.
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
  /api/people/{id}/letting:
    get:
      summary: Get Letting Roles for a Person
      description: Get letting roles for a person.
      operationId: People_LettingRolesByid
      x-api-path-slug: apipeopleidletting-get
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
      - Letting
      - Rolesa
      - Person
  /api/people/{id}/addcontactitem:
    post:
      summary: Add a ContactItem to a Person
      description: Add a contactitem to a person.
      operationId: People_AddContactItemByidBycontactItemSaveCommandDataContract
      x-api-path-slug: apipeopleidaddcontactitem-post
      parameters:
      - in: body
        name: contactItemSaveCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - ContactItem
      - To
      - Person
  /api/people/{id}/removecontactitem/{contactItemid}:
    put:
      summary: Remove a ContactItem from a Person
      description: Remove a contactitem from a person.
      operationId: People_RemoveContactItemByidBycontactItemid
      x-api-path-slug: apipeopleidremovecontactitemcontactitemid-put
      parameters:
      - in: path
        name: contactItemid
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - ContactItem
      - From
      - Person
  /api/people/unsubscribe/{id}:
    get:
      summary: Get All contact items for a person, but obscure the details
      description: Get all contact items for a person, but obscure the details.
      operationId: People_ObscuredContactItemsByid
      x-api-path-slug: apipeopleunsubscribeid-get
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
      - Contact
      - Itemsa
      - Person
      - ""
      - But
      - Obscure
      - Details
    post:
      summary: Unsubscribe/Subscribe All contact items for a person
      description: Unsubscribe/subscribe all contact items for a person.
      operationId: People_UnsubscibedContactItemsByidByitems
      x-api-path-slug: apipeopleunsubscribeid-post
      parameters:
      - in: path
        name: id
      - in: body
        name: items
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Unsubscribe
      - Subscribe
      - ""
      - Contact
      - Itemsa
      - Person
  /api/people/{id}/addaddress:
    put:
      summary: Add an Address to a Person
      description: Add an address to a person.
      operationId: People_AddAddressByidByaddress
      x-api-path-slug: apipeopleidaddaddress-put
      parameters:
      - in: body
        name: address
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Ress
      - To
      - Person
  /api/people/{id}/removeaddress/{addressId}:
    put:
      summary: Remove an Address from a Person
      description: Remove an address from a person.
      operationId: People_RemoveAddressByidByaddressId
      x-api-path-slug: apipeopleidremoveaddressaddressid-put
      parameters:
      - in: path
        name: addressId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Ress
      - From
      - Person
  /api/people/{id}/savenote:
    post:
      summary: Add a Note to a Person
      description: Add a note to a person.
      operationId: People_SaveNoteByidBynote
      x-api-path-slug: apipeopleidsavenote-post
      parameters:
      - in: path
        name: id
      - in: query
        name: note
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Note
      - To
      - Person
  /api/people/setpaymentdetails:
    put:
      summary: Set the payment details for a person
      description: Set the payment details for a person.
      operationId: People_SetPaymentDetailsBydataContract
      x-api-path-slug: apipeoplesetpaymentdetails-put
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Payment
      - Detailsa
      - Person
  /api/people/setprimarypaymentdetails:
    put:
      summary: Set the primary payment details for a person
      description: Set the primary payment details for a person.
      operationId: People_SetPrimaryPaymentDetailsByidByaccountIdBytenantRoleId
      x-api-path-slug: apipeoplesetprimarypaymentdetails-put
      parameters:
      - in: query
        name: accountId
        description: The bank account id
      - in: query
        name: id
        description: The person id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantRoleId
        description: Optional tenant role id to set account as primary
      responses:
        200:
          description: OK
      tags:
      - Set
      - Primary
      - Payment
      - Detailsa
      - Person
  /api/people/removepaymentdetails:
    put:
      summary: Set the payment details for a person
      description: Set the payment details for a person.
      operationId: People_RemovePaymentDetailsByidByaccountId
      x-api-path-slug: apipeopleremovepaymentdetails-put
      parameters:
      - in: query
        name: accountId
        description: The bank account id
      - in: query
        name: id
        description: The person id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Payment
      - Detailsa
      - Person
  /api/people/{id}/accounts:
    get:
      summary: Get the bank details for a person
      description: Get the bank details for a person.
      operationId: People_GetPersonsAccountsByid
      x-api-path-slug: apipeopleidaccounts-get
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
      - Bank
      - Detailsa
      - Person
  /api/people/findbyidentity:
    get:
      summary: Gets the person by an identity reference
      description: Gets the person by an identity reference.
      operationId: People_GetPersonByIdentityByissuerBynameidentifier
      x-api-path-slug: apipeoplefindbyidentity-get
      parameters:
      - in: query
        name: issuer
        description: The issuer of the identity
      - in: query
        name: nameidentifier
        description: The nameidentifier of the identity
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Person
      - By
      - Identity
      - Reference
  /api/people/{id}/roles:
    get:
      summary: Get basic role infomation for a Person by PersonId
      description: Get basic role infomation for a person by personid.
      operationId: People_BasicRolesByidBypageSizeBypageNumber
      x-api-path-slug: apipeopleidroles-get
      parameters:
      - in: path
        name: id
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Basic
      - Role
      - Infomationa
      - Person
      - By
      - PersonId
  /api/people/{id}/redactionstatus:
    get:
      summary: Redaction Status for a Person by PersonId
      description: Redaction status for a person by personid.
      operationId: People_RedactionStatusByid
      x-api-path-slug: apipeopleidredactionstatus-get
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
      - Redaction
      - Statusa
      - Person
      - By
      - PersonId
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