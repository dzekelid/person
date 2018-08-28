swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 1
info:
  title: Webex Teams API
  description: hey-there-thanks-for-checking-out-cisco-webex-for-developers--if-youve-used-cisco-webex-meetings-or-cisco-webex-teams-formerly-cisco-spark-you-know-how-easy-it-is-to-meet-and-collaborate-with-your-team-members-and-customers-the-webex-for-developers-program-opens-up-the-power-behind-the-webex-platform-to-anyone-seeking-to-extend-the-webex-experience-webex-meetings-is-a-powerful-conferencing-solution-that-lets-you-connect-with-anyone-anywhere-in-real-time--by-combining-video-audio-and-content-sharing-webex-meetings-creates-an-effective-conferencing-environment-leading-to-more-productive-meetings-and-increased-productivity--developer-information-for-webex-meetings-will-soon-be-available-on-this-site--in-the-meantime-to-get-started-with-developing-for-webex-meetings-please-see-the-getting-started-guides-over-on-cisco-devnet--keep-reading-for-information-about-webex-teams-webex-teams-makes-staying-in-sync-with-your-teammates-and-customers-easy-conversations-in-webex-teams-take-place-in-virtual-meeting-rooms--some-rooms-live-for-a-few-hours-while-others-become-permanent-fixtures-of-your-teams-workflow-with-titles-like-daily-standup-or-build-status--webex-teams-allows-conversations-to-flow-seamlessly-between-messages-video-calls-and-realtime-whiteboarding-sessions--no-other-solution-brings-together-so-many-facets-of-collaboration-into-a-single-unified-platform-httpsdeveloper-webex-comgettingstarted-html
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
      summary: Get person details
      description: "Shows details for a person, by ID.\r\n\r\nSpecify the person ID
        in the personId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-people-personId-get.html"
      operationId: PeopleByPersonGet
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
      - Details
    put:
      summary: Update a Person
      description: "Update details for a person, by ID.\r\n\r\nSpecify the person
        ID in the personId parameter in the URI. Only an admin can update a person
        details.\r\n\r\nhttps://developer.webex.com/endpoint-people-personId-put.html\r\n\r\nExample
        Request:\r\n``` json\r\n{\r\n  'emails\" : [ 'johnny.chang@foomail.com', 'jchang@barmail.com'
        ],\r\n  'displayName' : 'John Andersen',\r\n  'firstName' : 'John',\r\n  'lastName'
        : 'Andersen',\r\n  'avatar' : 'https://1efa7a94ed21783e352-c62266528714497a17239ececf39e9e2.ssl.cf1.rackcdn.com/V1~54c844c89e678e5a7b16a306bc2897b9~wx29yGtlTpilEFlYzqPKag==~1600',\r\n
        \ 'orgId' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',\r\n  'roles'
        : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy',
        'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX'
        ],\r\n  'licenses' : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy',
        'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX'
        ]\r\n}\r\n```"
      operationId: PeopleByPersonPut
      x-api-path-slug: people-person-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: _person
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Person
    delete:
      summary: Delete a Person
      description: |-
        Remove a person from the system. Only an admin can remove a person.

        Specify the person ID in the personId parameter in the URI.

        https://developer.webex.com/endpoint-people-personId-delete.html
      operationId: PeopleByPersonDelete
      x-api-path-slug: people-person-delete
      parameters:
      - in: path
        name: _person
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Person
  /people/me:
    get:
      summary: Get person details (me)
      description: |-
        Show the profile for the authenticated user.

        https://developer.webex.com/endpoint-people-me-get.html
      operationId: PeopleMeGet
      x-api-path-slug: peopleme-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Person
      - Details
      - (me)
  /people:
    post:
      summary: Create a Person (random)
      description: |-
        Create a new user account for a given organization. Only an admin can create a new user account.

        https://developer.webex.com/endpoint-people-post.html

        Example Request:
        ``` json
        {
          'emails' : [ 'johnny.chang@foomail.com', 'jchang@barmail.com' ],
          'displayName' : 'John Andersen',
          'firstName' : 'John',
          'lastName' : 'Andersen',
          'avatar' : 'https://1efa7a94ed21783e352-c62266528714497a17239ececf39e9e2.ssl.cf1.rackcdn.com/V1~54c844c89e678e5a7b16a306bc2897b9~wx29yGtlTpilEFlYzqPKag==~1600',
          'orgId' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
          'roles' : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy', 'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX' ],
          'licenses' : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy', 'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX' ]
        }

        Example Response:
        {
          'id' : 'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mNWIzNjE4Ny1jOGRkLTQ3MjctOGIyZi1mOWM0NDdmMjkwNDY',
          'emails' : [ 'johnny.chang@foomail.com', 'jchang@barmail.com' ],
          'displayName' : 'John Andersen',
          'firstName' : 'John',
          'lastName' : 'Andersen',
          'avatar' : 'https://1efa7a94ed21783e352-c62266528714497a17239ececf39e9e2.ssl.cf1.rackcdn.com/V1~54c844c89e678e5a7b16a306bc2897b9~wx29yGtlTpilEFlYzqPKag==~1600',
          'orgId' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
          'roles' : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy', 'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX' ],
          'licenses' : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy', 'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX' ],
          'created' : '2015-10-18T14:26:16+00:00',
          'timezone' : 'America/Denver'
        }
        ```
      operationId: PeoplePost
      x-api-path-slug: people-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Person
      - (random)