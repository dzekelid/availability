swagger: "2.0"
x-collection-name: TelAPI
x-complete: 1
info:
  title: TelAPI
  description: telapi-is-a-rest-api--what-that-means-for-you-is-that-interacting-with-telapi-to-perform-all-of-your-telephony-needs-is-almost-as-simple-as-visiting-a-website--deeper-knowledge-regarding-rest-is-useful-when-developing-with-telapi-but-definitely-not-required--we-aim-to-provide-all-of-the-information-needed-for-working-with-our-rest-api-throughout-its-documentation-provided-here-so-even-if-you-are-new-to-rest-telapi-will-still-be-a-pleasure-to-use-
  termsOfService: http://www.telapi.com/legal/tos
  version: v2
host: api.telapi.com
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/hotel/v0/hotels/{hotelId}/rooms/available:
    get:
      summary: Request available rooms using a given criteria.
      description: Request available rooms using a given criteria..
      operationId: Rooms_GetAvailableRooms
      x-api-path-slug: apihotelv0hotelshotelidroomsavailable-get
      parameters:
      - in: query
        name: adults
        description: Specifies number of adults the returned rooms will have to be
          able to house
      - in: query
        name: amenities
        description: Return result only for rooms having all of the given amenities
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: from
        description: Rooms returned will not be assigned to a reservation or be under
          maintenance between this date            and the specified to date
      - in: path
        name: hotelId
        description: The hotel you are looking for available rooms
      - in: query
        name: includeOutOfService
        description: Should rooms that are set OutOfService in the defined time period
          be returned as available
      - in: query
        name: inlinecount
        description: Return total number of items for a given filter criteria
      - in: query
        name: locations
        description: Return result only for rooms having at least one of the specified
          locations
      - in: query
        name: roomTypes
        description: Return result only for rooms for the given room types
      - in: query
        name: skip
        description: Amount of items to skip
      - in: query
        name: to
        description: Rooms returned will not be assigned to a reservation or be under
          maintenance between the specified            from date and this date
      - in: query
        name: top
        description: Amount of items to select
      - in: query
        name: views
        description: Return result only for rooms having at least one of the specified
          views
      responses:
        200:
          description: OK
      tags:
      - Request
      - Available
      - Rooms
      - Using
      - Given
      - Criteria