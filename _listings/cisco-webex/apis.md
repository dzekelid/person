---
name: Cisco WebEx
x-slug: cisco-webex
description: Cisco Webex is the leading enterprise solution for video conferencing
  & web conferencing today. This secure software-based platform for video & audio
  conferencing, group messaging & webinars helps organizations be more productive.Participants
  can join ...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
x-kinRank: "7"
x-alexaRank: "632"
tags: Person
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/cisco-webex/apis.md
specificationVersion: "0.14"
apis:
- name: Webex Teams Admin API - Get Person Details1
  x-api-slug: people-person-get
  description: |-
    Shows details for a person, by ID.
    Specify the person ID in the personId parameter in the URI.

    https://developer.webex.com/endpoint-people-personId-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/cisco-webex/people-person-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/cisco-webex/people-person-get-openapi.md
- name: Webex Teams Admin API - Update a Person
  x-api-slug: people-person-put
  description: "Update details for a person, by ID.\r\n\r\nSpecify the person ID in
    the personId parameter in the URI. Only an admin can update a person details.\r\n\r\nhttps://developer.webex.com/endpoint-people-personId-put.html\r\n\r\nExample
    Request:\r\n``` json\r\n{\r\n  'emails\" : [ 'johnny.chang@foomail.com', 'jchang@barmail.com'
    ],\r\n  'displayName' : 'John Andersen',\r\n  'firstName' : 'John',\r\n  'lastName'
    : 'Andersen',\r\n  'avatar' : 'https://1efa7a94ed21783e352-c62266528714497a17239ececf39e9e2.ssl.cf1.rackcdn.com/V1~54c844c89e678e5a7b16a306bc2897b9~wx29yGtlTpilEFlYzqPKag==~1600',\r\n
    \ 'orgId' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',\r\n  'roles' :
    [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy',
    'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX'
    ],\r\n  'licenses' : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy',
    'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX'
    ]\r\n}\r\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/cisco-webex/people-person-put-openapi.md
- name: Webex Teams Admin API - Delete a Person
  x-api-slug: people-person-delete
  description: |-
    Remove a person from the system. Only an admin can remove a person.

    Specify the person ID in the personId parameter in the URI.

    https://developer.webex.com/endpoint-people-personId-delete.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/cisco-webex/people-person-delete-openapi.md
- name: Webex Teams Admin API - Get Person Details (me)
  x-api-slug: peopleme-get
  description: |-
    Show the profile for the authenticated user.

    https://developer.webex.com/endpoint-people-me-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/cisco-webex/peopleme-get-openapi.md
- name: Webex Teams Admin API - Create a Person (random)
  x-api-slug: people-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/cisco-webex/people-post-openapi.md
- name: Webex Teams API - Get person details (me)
  x-api-slug: peopleme-get
  description: |-
    Show the profile for the authenticated user.

    https://developer.webex.com/endpoint-people-me-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/cisco-webex/peopleme-get-openapi.md
- name: Webex Teams API - Get person details
  x-api-slug: people-person-get
  description: "Shows details for a person, by ID.\r\n\r\nSpecify the person ID in
    the personId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-people-personId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/cisco-webex/people-person-get-openapi.md
x-common:
- type: x-postman-collection
  url: https://app.getpostman.com/run-collection/1f5e101d8290a5303c90
- type: x-api-gallery
  url: http://cisco.unity.connection.messaging.interface.api.gallery.streamdata.io
- type: x-api-stack
  url: http://cisco.webex.stack.network
- type: x-blog
  url: http://blogs.webex.com/
- type: x-blog-rss
  url: http://blogs.webex.com/webex_interactions/index.rdf
- type: x-crunchbase
  url: https://crunchbase.com/organization/webex-communications
- type: x-crunchbase
  url: http://www.crunchbase.com/company/webex
- type: x-postman-collection
  url: https://app.getpostman.com/run-collection/0aa22af74405f82086d4
- type: x-twitter
  url: https://twitter.com/webex
- type: x-developer
  url: https://developer.webex.com/
- type: x-website
  url: https://webex.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---