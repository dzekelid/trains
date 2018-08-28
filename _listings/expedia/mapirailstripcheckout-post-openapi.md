---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 0
info:
  title: Expedia Rails Checkout With JSON Request Body
  description: Mobile API Rails Checkout
  version: 0.0.1
host: apim.expedia.com
basePath: x/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /m/api/rails/trip/checkout:
    post:
      summary: Rails Checkout With JSON Request Body
      description: Mobile API Rails Checkout
      operationId: rails-cko
      x-api-path-slug: mapirailstripcheckout-post
      parameters:
      - in: body
        name: body
        description: JSON body with all the fields required for a Rails checkout
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Trains
      - Rails
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