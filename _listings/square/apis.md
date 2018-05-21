---
name: Square
x-slug: square
description: Starting with a free credit card reader for the iPhone, iPad, and Android
  devices, Square Reader allows anyone to accept credit cards anywhere, anytime, for
  a low transaction rate of 2.75 percent per swipe, with no hidden fees. Square Register
  serves as a full point-of-sale system for businesses to accept payments, manage
  items, and share menu and location information. Square Wallet, available in the
  US, is the most seamless way to pay, enabling individuals to pay at their favorite
  local businesses, discover new ones nearby, explore menu listings, and store receipts.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
x-kinRank: "9"
x-alexaRank: ""
tags: Discounts
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/discounts/master/_listings/square/apis.md
specificationVersion: "0.14"
apis:
- name: Square Connect API Post Location Discounts
  x-api-slug: square-connect-api
  description: Post location discounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///{location_id}/discounts
  tags: Location,Discounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/discounts/master/_listings/square/location-iddiscounts-post-openapi.md
- name: Square Connect API Get Location Discounts
  x-api-slug: square-connect-api
  description: Lists all of a location's discounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///{location_id}/discounts
  tags: Location,Discounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/discounts/master/_listings/square/location-iddiscounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/discounts/master/_listings/square/location-iddiscounts-get-openapi.md
- name: Square Connect API Put Location Discounts Discount
  x-api-slug: square-connect-api
  description: Modifies the details of an existing discount.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///{location_id}/discounts/{discount_id}
  tags: Location,Discounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/discounts/master/_listings/square/location-iddiscountsdiscount-id-put-openapi.md
- name: Square Connect API Delete Location Discounts Discount
  x-api-slug: square-connect-api
  description: Delete location discounts discount.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///{location_id}/discounts/{discount_id}
  tags: Location,Discounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/discounts/master/_listings/square/location-iddiscountsdiscount-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/discounts/master/_listings/square/location-iddiscountsdiscount-id-delete-openapi.md
- name: Square Connect API
  x-api-slug: square-connect-api
  description: Starting with a free credit card reader for the iPhone, iPad, and Android
    devices, Square Reader allows anyone to accept credit cards anywhere, anytime,
    for a low transaction rate of 2.75 percent per swipe, with no hidden fees. Square
    Register serves as a full point-of-sale system for businesses to accept payments,
    manage items, and share menu and location information. Square Wallet, available
    in the US, is the most seamless way to pay, enabling individuals to pay at their
    favorite local businesses, discover new ones nearby, explore menu listings, and
    store receipts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1/
  tags: Discounts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/discounts/master/_listings/square/openapi.md
x-common:
- type: x-base
  url: https://connect.squareup.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/square
- type: x-developer
  url: https://connect.squareup.com/
- type: x-github
  url: https://github.com/square
- type: x-twitter
  url: https://twitter.com/Square
- type: x-website
  url: https://squareup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---