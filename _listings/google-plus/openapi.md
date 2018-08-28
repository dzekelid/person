swagger: "2.0"
x-collection-name: Google Plus
x-complete: 1
info:
  title: Google Plus
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities/{activityId}/people/{collection}:
    get:
      summary: Get People In Collection
      description: List all of the people in the specified collection for a particular
        activity.
      operationId: plusDomains.people.listByActivity
      x-api-path-slug: activitiesactivityidpeoplecollection-get
      parameters:
      - in: path
        name: activityId
        description: The ID of the activity to get the list of people for
      - in: path
        name: collection
        description: The collection of people to list
      - in: query
        name: maxResults
        description: The maximum number of people to include in the response, which
          is used for paging
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      responses:
        200:
          description: OK
      tags:
      - Person
  /people:
    get:
      summary: Get People
      description: Search all public profiles.
      operationId: plus.people.search
      x-api-path-slug: people-get
      parameters:
      - in: query
        name: language
        description: Specify the preferred language to search with
      - in: query
        name: maxResults
        description: The maximum number of people to include in the response, which
          is used for paging
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: query
        name: query
        description: Specify a query string for full text search of public text in
          all profiles
      responses:
        200:
          description: OK
      tags:
      - Person
  /people/{userId}:
    get:
      summary: Get Person Profile
      description: Get a person's profile.
      operationId: plusDomains.people.get
      x-api-path-slug: peopleuserid-get
      parameters:
      - in: path
        name: userId
        description: The ID of the person to get the profile for
      responses:
        200:
          description: OK
      tags:
      - Person
  /people/{userId}/people/{collection}:
    get:
      summary: Get People In Collection
      description: List all of the people in the specified collection.
      operationId: plusDomains.people.list
      x-api-path-slug: peopleuseridpeoplecollection-get
      parameters:
      - in: path
        name: collection
        description: The collection of people to list
      - in: query
        name: maxResults
        description: The maximum number of people to include in the response, which
          is used for paging
      - in: query
        name: orderBy
        description: The order to return people in
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: path
        name: userId
        description: Get the collection of people for the person identified
      responses:
        200:
          description: OK
      tags:
      - Person
  /circles/{circleId}/people:
    get:
      summary: Get People in Circle
      description: List all of the people who are members of a circle.
      operationId: plusDomains.people.listByCircle
      x-api-path-slug: circlescircleidpeople-get
      parameters:
      - in: path
        name: circleId
        description: The ID of the circle to get the members of
      - in: query
        name: maxResults
        description: The maximum number of people to include in the response, which
          is used for paging
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      responses:
        200:
          description: OK
      tags:
      - Person
    put:
      summary: Update People in Circle
      description: Add a person to a circle. Google+ limits certain circle operations,
        including the number of circle adds. Learn More.
      operationId: plusDomains.circles.addPeople
      x-api-path-slug: circlescircleidpeople-put
      parameters:
      - in: path
        name: circleId
        description: The ID of the circle to add the person to
      - in: query
        name: email
        description: Email of the people to add to the circle
      - in: query
        name: userId
        description: IDs of the people to add to the circle
      responses:
        200:
          description: OK
      tags:
      - Person