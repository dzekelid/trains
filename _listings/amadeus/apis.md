---
name: Amadeus
x-slug: amadeus
description: Amadeus travel technology helps businesses connect to the global travel
  ecosystem, manage operations more effectively and serve travellers better than ever
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
x-kinRank: "8"
x-alexaRank: "4309"
tags: Trains
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/trains/master/_listings/amadeus/apis.md
specificationVersion: "0.14"
apis:
- name: Amadeus - Get Trains Extensive Search
  x-api-slug: trainsextensivesearch-get
  description: "This API allows you to search trains availability and prices for a
    single day or date range. It's based on our Rail Instant Search technology, providing
    you with immediate results from our rail search cache.\n\nThis API has content
    from SNCF (French trains).\n            \nThe content is also restricted to single-leg
    trips - where a single train takes you directly from the origin to the destination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trains/master/_listings/amadeus/trainsextensivesearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trains/master/_listings/amadeus/trainsextensivesearch-get-openapi.md
- name: Amadeus - Get Trains Schedule Search
  x-api-slug: trainsschedulesearch-get
  description: |-
    This API allows you to find all the possible destinations in the Rail Instant Search cache (used by Extensive Search above) from a given origin station on a given day. You can use this to help build network maps, journey planners or provide inspiration for rail travel.

    This API has continuous content from SNCF.
    All the options returned are single-leg trips - where a single train takes you directly from the origin to the destination. In general, only departure dates up to 90 days in the future are supported

    Currently agglomeration stations are not supported
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trains/master/_listings/amadeus/trainsschedulesearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trains/master/_listings/amadeus/trainsschedulesearch-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://amadeus.api.gallery.streamdata.io
- type: x-api-stack
  url: http://amadeus.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/amadeus
- type: x-documentation
  url: https://sandbox.amadeus.com/api-catalog
- type: x-github
  url: https://github.com/AmadeusITGroup
- type: x-privacy-policy
  url: http://www.amadeus.com/web/amadeus/en_1A-corporate/Amadeus-Home/Amadeus_IT_Group_SA-Legal-notices-2014/1319560218660-Page-AMAD_Detail_PopUp_Ppal?assetid=1319607040997&assettype=DataProtection_C
- type: x-sandbox
  url: https://sandbox.amadeus.com
- type: x-twitter
  url: https://twitter.com/amadeusinnov
- type: x-website
  url: https://amadeus.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---