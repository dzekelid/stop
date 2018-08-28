---
name: Public Transport Victoria Timetable
x-slug: public-transport-victoria-timetable
description: The PTV Timetable API provides direct access to Public Transport Victoria&rsquo;s
  public transport timetable data. The API returns scheduled timetable, route and
  stop data for all metropolitan and regional train, tram and bus services in Victoria,
  including Night Network(Night Train and Night Tram data are included in metropolitan
  train and tram services data, respectively, whereas Night Bus is a separate route
  type). The API also returns real-time data for metropolitan train, tram and bus
  services (where this data is made available to PTV), as well as disruption information,
  stop facility information, and access to myki ticket outlet data.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/public-transport-victoria.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Stop
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/stop/master/_listings/public-transport-victoria-timetable/apis.md
specificationVersion: "0.14"
apis:
- name: Public Transport Victoria Timetable - Get V3 Departures Route Type Route Type
    Stop Stop
  x-api-slug: v3departuresroute-typeroute-typestopstop-id-get
  description: View departures for all routes from a stop.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/public-transport-victoria.png
  humanURL: https://www.ptv.vic.gov.au/about-ptv/data-and-reports/datasets/ptv-timetable-api/
  baseURL: https://timetableapi.ptv.vic.gov.au//
  tags: Transit, API Provider, Transportation, Profiles, General Data, Cities
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stop/master/_listings/public-transport-victoria-timetable/v3departuresroute-typeroute-typestopstop-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stop/master/_listings/public-transport-victoria-timetable/v3departuresroute-typeroute-typestopstop-id-get-openapi.md
- name: Public Transport Victoria Timetable - Get V3 Departures Route Type Route Type
    Stop Stop Route Route
  x-api-slug: v3departuresroute-typeroute-typestopstop-idrouteroute-id-get
  description: View departures for a specific route from a stop.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/public-transport-victoria.png
  humanURL: https://www.ptv.vic.gov.au/about-ptv/data-and-reports/datasets/ptv-timetable-api/
  baseURL: https://timetableapi.ptv.vic.gov.au//
  tags: Transit, API Provider, Transportation, Profiles, General Data, Cities
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stop/master/_listings/public-transport-victoria-timetable/v3departuresroute-typeroute-typestopstop-idrouteroute-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stop/master/_listings/public-transport-victoria-timetable/v3departuresroute-typeroute-typestopstop-idrouteroute-id-get-openapi.md
- name: Public Transport Victoria Timetable - Get V3 Stops Stop Route Type Route Type
  x-api-slug: v3stopsstop-idroute-typeroute-type-get
  description: View facilities at a specific stop (metro and v/line stations only).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/public-transport-victoria.png
  humanURL: https://www.ptv.vic.gov.au/about-ptv/data-and-reports/datasets/ptv-timetable-api/
  baseURL: https://timetableapi.ptv.vic.gov.au//
  tags: Transit, API Provider, Transportation, Profiles, General Data, Cities
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stop/master/_listings/public-transport-victoria-timetable/v3stopsstop-idroute-typeroute-type-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stop/master/_listings/public-transport-victoria-timetable/v3stopsstop-idroute-typeroute-type-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://product.hunt.api.gallery.streamdata.io
- type: x-api-stack
  url: http://public.transport.victoria.timetable.stack.network
- type: x-website
  url: https://www.ptv.vic.gov.au/about-ptv/data-and-reports/datasets/ptv-timetable-api/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---