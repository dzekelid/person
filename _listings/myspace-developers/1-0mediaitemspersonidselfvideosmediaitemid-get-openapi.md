---
swagger: "2.0"
x-collection-name: MySpace Developers
x-complete: 0
info:
  title: My Space Get Mediaitems Personid Self Videos Mediaitemid
  description: Retrieves a video.
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
  /1.0/albums/{personId}/@self:
    post:
      summary: Post Albums Personid Self
      description: Adding an Album.
      operationId: 1.0.albums.personId._self.post
      x-api-path-slug: 1-0albumspersonidself-post
      parameters:
      - in: header
        name: Content-Type
        description: Specifies Content Type
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: personId
        description: The persons identifier
      responses:
        200:
          description: OK
      tags:
      - Albums
      - People
      - Self
    get:
      summary: Get Albums Personid Self
      description: Retrieves the current user's albums.
      operationId: 1.0.albums.personId._self.get
      x-api-path-slug: 1-0albumspersonidself-get
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
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - Albums
      - People
      - Self
  /1.0/albums/{personId}/@self/{albumId}:
    put:
      summary: Put Albums Personid Self Albums
      description: Update an Album.
      operationId: 1.0.albums.personId._self.albumId.put
      x-api-path-slug: 1-0albumspersonidselfalbumid-put
      parameters:
      - in: path
        name: albumId
        description: Indicates which single album should be returned
      - in: header
        name: Content-Type
        description: Specifies Content Type
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: personId
        description: The persons identifier
      responses:
        200:
          description: OK
      tags:
      - Albums
      - People
      - Self
      - AlbumId
    get:
      summary: Get Albums Personid Self Albums
      description: Retrieves an album.
      operationId: 1.0.albums.personId._self.albumId.get
      x-api-path-slug: 1-0albumspersonidselfalbumid-get
      parameters:
      - in: path
        name: albumId
        description: Indicates which single album should be returned
      - in: path
        name: personId
        description: The persons identifier
      responses:
        200:
          description: OK
      tags:
      - Albums
      - People
      - Self
      - AlbumId
  /1.0/appdata/{personId}/{selector}/{appId}:
    delete:
      summary: Delete Appdata Personid Selector Appid
      description: Deletes a specified user's application data.
      operationId: 1.0.appdata.personId.selector.appId.delete
      x-api-path-slug: 1-0appdatapersonidselectorappid-delete
      parameters:
      - in: path
        name: appId
        description: The applications ID associated with the OAuth ConsumerKey/ConsumerSecret
          pair
      - in: query
        name: fields
        description: The fields correspond to keys in the application data
      - in: query
        name: format
        description: Determines the format of the response
      - in: path
        name: personId
        description: The persons identifier
      - in: path
        name: selector
        description: Indicates which set of individuals to query for activities
      responses:
        200:
          description: OK
      tags:
      - Appdata
      - People
      - Selector
      - AppId
    post:
      summary: Post Appdata Personid Selector Appid
      description: Adds or updates a specified user's application data.
      operationId: 1.0.appdata.personId.selector.appId.post
      x-api-path-slug: 1-0appdatapersonidselectorappid-post
      parameters:
      - in: path
        name: appId
        description: The applications ID associated with the OAuth ConsumerKey/ConsumerSecret
          pair
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: header
        name: Content-Type
        description: Specifies Content Type
      - in: query
        name: fields
        description: The fields correspond to keys in the application data
      - in: query
        name: format
        description: Determines the format of the response
      - in: path
        name: personId
        description: The persons identifier
      - in: path
        name: selector
        description: Indicates which set of individuals to query for activities
      responses:
        200:
          description: OK
      tags:
      - Appdata
      - People
      - Selector
      - AppId
    get:
      summary: Get Appdata Personid Selector Appid
      description: Retrieves all application data for a specified user.
      operationId: 1.0.appdata.personId.selector.appId.get
      x-api-path-slug: 1-0appdatapersonidselectorappid-get
      parameters:
      - in: path
        name: appId
        description: The applications ID associated with the OAuth ConsumerKey/ConsumerSecret
          pair
      - in: query
        name: fields
        description: The fields correspond to keys in the application data
      - in: query
        name: format
        description: Determines the format of the response
      - in: path
        name: personId
        description: The persons identifier
      - in: path
        name: selector
        description: Indicates which set of individuals to query for activities
      responses:
        200:
          description: OK
      tags:
      - Appdata
      - People
      - Selector
      - AppId
  /1.0/groups/{personId}:
    get:
      summary: Get Groups Personid
      description: Retrieves the current user's groups.
      operationId: 1.0.groups.personId.get
      x-api-path-slug: 1-0groupspersonid-get
      parameters:
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: 'The following field names are supported: id and title'
      - in: query
        name: format
        description: Determines the format of the response
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - Groups
      - People
  /1.0/mediaitemcomments/{personId}/@self/{albumId}/{mediaItemId}:
    get:
      summary: Get Mediaitemcomments Personid Self Albums Mediaitemid
      description: Retrieves item comments from a specified album.
      operationId: 1.0.mediaitemcomments.personId._self.albumId.mediaItemId.get
      x-api-path-slug: 1-0mediaitemcommentspersonidselfalbumidmediaitemid-get
      parameters:
      - in: path
        name: albumId
        description: Indicates which single album from the group identified by {selector}
          should be returned
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
        name: mediaItemId
        description: Indicates which single media item from the album identified by
          {albumId} should be returned
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - Mediaitemcomments
      - People
      - Self
      - AlbumId
      - MediaItemId
  /1.0/mediaItems/{personId}/@self/@videos:
    post:
      summary: Post Mediaitems Personid Self Videos
      description: Adds videos from a specified album.
      operationId: 1.0.mediaItems.personId._self._videos.post
      x-api-path-slug: 1-0mediaitemspersonidselfvideos-post
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: header
        name: Content-Type
        description: Specifies Content Type
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
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - MediaItems
      - People
      - Self
      - '@videos'
    get:
      summary: Get Mediaitems Personid Self Videos
      description: Retrieves all the videos.
      operationId: 1.0.mediaItems.personId._self._videos.get
      x-api-path-slug: 1-0mediaitemspersonidselfvideos-get
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
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - MediaItems
      - People
      - Self
      - '@videos'
  /1.0/mediaItems/{personId}/@self/@videos/{mediaItemId}:
    put:
      summary: Put Mediaitems Personid Self Videos Mediaitemid
      description: Updates an video.
      operationId: 1.0.mediaItems.personId._self._videos.mediaItemId.put
      x-api-path-slug: 1-0mediaitemspersonidselfvideosmediaitemid-put
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: header
        name: Content-Type
        description: Specifies Content Type
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
        name: mediaItemId
        description: Indicates which single media item should be returned
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - MediaItems
      - People
      - Self
      - '@videos'
      - MediaItemId
    get:
      summary: Get Mediaitems Personid Self Videos Mediaitemid
      description: Retrieves a video.
      operationId: 1.0.mediaItems.personId._self._videos.mediaItemId.get
      x-api-path-slug: 1-0mediaitemspersonidselfvideosmediaitemid-get
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
        name: mediaItemId
        description: Indicates which single media item should be returned
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - MediaItems
      - People
      - Self
      - '@videos'
      - MediaItemId
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