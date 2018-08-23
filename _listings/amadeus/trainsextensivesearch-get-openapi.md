---
swagger: "2.0"
x-collection-name: Amadeus
x-complete: 0
info:
  title: Amadeus Get Trains Extensive Search
  description: "This API allows you to search trains availability and prices for a
    single day or date range. It's based on our Rail Instant Search technology, providing
    you with immediate results from our rail search cache.\n\nThis API has content
    from SNCF (French trains).\n            \nThe content is also restricted to single-leg
    trips - where a single train takes you directly from the origin to the destination."
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