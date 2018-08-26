---
swagger: "2.0"
x-collection-name: MySpace Developers
x-complete: 0
info:
  title: My Space Get Activities Personid Selector Appid
  description: Retrieves activities created by an application.
  version: 1.0.0
host: api.myspace.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1.0/activities/{personId}/@self:
    post:
      summary: Post Activities Personid Self
      description: Creates an activity for the user.
      operationId: 1.0.activities.personId._self.post
      x-api-path-slug: 1-0activitiespersonidself-post
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: header
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: personId
        description: The persons identifier
      responses:
        200:
          description: OK
      tags:
      - Activities
      - People
      - Self
  /1.0/activities/{personId}/{selector}:
    get:
      summary: Get Activities Personid Selector
      description: Retrieves all activities for the user or for the friends of the
        viewer.
      operationId: 1.0.activities.personId.selector.get
      x-api-path-slug: 1-0activitiespersonidselector-get
      parameters:
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: format
        description: Determines the format of the response
      - in: path
        name: personId
        description: The persons identifier
      - in: path
        name: selector
        description: Indicates which set of individuals to query for activities
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      - in: query
        name: updatedSince
        description: Indicates the date before which no activities should be returned
      responses:
        200:
          description: OK
      tags:
      - Activities
      - People
      - Selector
  /1.0/activities/{personId}/{selector}/{appId}:
    get:
      summary: Get Activities Personid Selector Appid
      description: Retrieves activities created by an application.
      operationId: 1.0.activities.personId.selector.appId.get
      x-api-path-slug: 1-0activitiespersonidselectorappid-get
      parameters:
      - in: path
        name: appId
        description: The applications ID associated with the OAuth ConsumerKey/ConsumerSecret
          pair
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: format
        description: Determines the format of the response
      - in: path
        name: personId
        description: The persons identifier
      - in: path
        name: selector
        description: Indicates which set of individuals to query for activities
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      - in: query
        name: updatedSince
        description: Indicates the date before which no activities should be returned
      responses:
        200:
          description: OK
      tags:
      - Activities
      - People
      - Selector
      - AppId
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