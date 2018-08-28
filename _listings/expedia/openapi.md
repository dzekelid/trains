swagger: "2.0"
x-collection-name: Expedia
x-complete: 1
info:
  title: Expedia
  description: expedia-mobile-api-documentation--brfont-colorblue-note-in-case-of-authorization-exception-just-a-hrefstaticmobileswaggeruiusersigninusersigninafont
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