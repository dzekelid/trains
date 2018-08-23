---
swagger: "2.0"
x-collection-name: Amadeus
x-complete: 1
info:
  title: Amadeus
  description: amadeus-api-is-a-toolkit-designed-for-travel-agencies-who-want-to-develop-their-own-travel-products-rather-than-using-offtheshelf-solutions--with-this-tool-you-can-build-your-very-own-customised-applications-that-link-in-a-stable-and-secure-dialogue-with-our-global-distribution-system-gds-
  contact:
    name: Amadeus Innovation and Research
    url: https://sandbox.amadeus.com
  version: 1.0.0
host: api.sandbox.amadeus.com
basePath: /v1.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /trains/extensive-search:
    get:
      summary: Get Trains Extensive Search
      description: "This API allows you to search trains availability and prices for
        a single day or date range. It's based on our Rail Instant Search technology,
        providing you with immediate results from our rail search cache.\n\nThis API
        has content from SNCF (French trains).\n            \nThe content is also
        restricted to single-leg trips - where a single train takes you directly from
        the origin to the destination."
      operationId: getTrainsExtensiveSearch
      x-api-path-slug: trainsextensivesearch-get
      parameters:
      - in: query
        name: departure_date
        description: The date or range of dates on which you would like to depart
          from the origin station to go to the destination
      - in: query
        name: destination
        description: Identifier of the rail station to which you would like to travel
      - in: query
        name: origin
        description: Identifier of the rail station from which you would like to depart
      responses:
        200:
          description: OK
      tags:
      - Trains
      - Extensive
      - Search
  /trains/schedule-search:
    get:
      summary: Get Trains Schedule Search
      description: |-
        This API allows you to find all the possible destinations in the Rail Instant Search cache (used by Extensive Search above) from a given origin station on a given day. You can use this to help build network maps, journey planners or provide inspiration for rail travel.

        This API has continuous content from SNCF.
        All the options returned are single-leg trips - where a single train takes you directly from the origin to the destination. In general, only departure dates up to 90 days in the future are supported

        Currently agglomeration stations are not supported
      operationId: getTrainsScheduleSearch
      x-api-path-slug: trainsschedulesearch-get
      parameters:
      - in: query
        name: departure_date
        description: The date on which you would like to depart from the origin station
          to go to the destination
      - in: query
        name: origin
        description: Identifier of the rail station where you would like to depart
          from
      responses:
        200:
          description: OK
      tags:
      - Trains
      - Schedule
      - Search
---