---
name: Flowroute
x-slug: flowroute
description: Flowroute is the leading provider of cloud-based communications and is
  based in Seattle, Washington.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
x-kinRank: "7"
x-alexaRank: "235018"
tags: Flowroute
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/apis.md
specificationVersion: "0.14"
apis:
- name: Flowroute APIs - Send a Message
  x-api-slug: v2-1messages-post
  description: Sends an SMS or MMS from a Flowroute long code or toll-free phone number
    to another valid phone number.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2-1messages-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2-1messages-post-openapi.md
- name: Flowroute APIs - Look Up a Set of Messages
  x-api-slug: v2-1messages-get
  description: Retrieves a list of Message Detail Records (MDRs) within a specified
    date range. Date and time is based on Coordinated Universal Time (UTC).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2-1messages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2-1messages-get-openapi.md
- name: Flowroute APIs - Look Up a Message Detail Record
  x-api-slug: v2-1messagesid-get
  description: Searches for a specific message record ID and returns a Message Detail
    Record (in MDR2 format).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2-1messagesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2-1messagesid-get-openapi.md
- name: Flowroute APIs - Account Phone Numbers
  x-api-slug: v2numbers-get
  description: Returns a list of all phone numbers currently on your Flowroute account.
    The response includes details such as the phone number's rate center, state, number
    type, and whether CNAM Lookup is enabled for that number.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbers-get-openapi.md
- name: Flowroute APIs - Phone Number Details
  x-api-slug: v2numbersid-get
  description: Lists all of the information associated with any of the phone numbers
    in your account, including billing method, primary voice route, and failover voice
    route.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersid-get-openapi.md
- name: Flowroute APIs - Purchase a Phone Number
  x-api-slug: v2numbersid-post
  description: Lets you purchase a phone number from available Flowroute inventory.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersid-post-openapi.md
- name: Flowroute APIs - Search for Purchasable Phone Numbers
  x-api-slug: v2numbersavailable-get
  description: This endpoint lets you search for phone numbers by state or rate center,
    or by your specified search value.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersavailable-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersavailable-get-openapi.md
- name: Flowroute APIs - List Available Area Codes
  x-api-slug: v2numbersavailableareacodes-get
  description: Returns a list of all Numbering Plan Area (NPA) codes containing purchasable
    phone numbers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersavailableareacodes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersavailableareacodes-get-openapi.md
- name: Flowroute APIs - List Available Exchange Codes
  x-api-slug: v2numbersavailableexchanges-get
  description: Returns a list of all Central Office (exchange) codes containing purchasable
    phone numbers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersavailableexchanges-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersavailableexchanges-get-openapi.md
- name: Flowroute APIs - Update Primary Voice Route for a Phone Number
  x-api-slug: v2numbersnumber-idrelationshipsprimary-route-patch
  description: Use this endpoint to update the primary voice route for a phone number.
    You must create the route first by following "Create an Inbound Route". You can
    then assign the created route by specifying its value in a PATCH request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersnumber-idrelationshipsprimary-route-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersnumber-idrelationshipsprimary-route-patch-openapi.md
- name: Flowroute APIs - Update Failover Voice Route for a Phone Number
  x-api-slug: v2numbersnumber-idrelationshipsfailover-route-patch
  description: Use this endpoint to update the failover voice route for a phone number.
    You must create the route first by following "Create an Inbound Route". You can
    then assign the created route by specifying its value in a PATCH request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersnumber-idrelationshipsfailover-route-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2numbersnumber-idrelationshipsfailover-route-patch-openapi.md
- name: Flowroute APIs - Create an Inbound Route
  x-api-slug: v2routes-post
  description: Creates a new inbound route which can then be associated with phone
    numbers. Please see "List Inbound Routes" to review the route values that you
    can associate with your Flowroute phone numbers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2routes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2routes-post-openapi.md
- name: Flowroute APIs - List Inbound Routes
  x-api-slug: v2routes-get
  description: Returns a list of your inbound routes. From the list, you can then
    select routes to use as the primary and failover routes for a phone number, which
    you can do via "Update Primary Voice Route for a Phone Number" and "Update Failover
    Voice Route for a Phone Number".
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28795-developer-flowroute-com.jpg
  humanURL: http://developer.flowroute.com
  baseURL: https:////
  tags: Telecommunications, ISP, Technology, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2routes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flowroute/master/_listings/flowroute/v2routes-get-openapi.md
x-common:
- type: x-github
  url: https://github.com/flowroute
- type: x-openapi
  url: https://raw.githubusercontent.com/flowroute/flowroute-sdk-v3-dot-net/master/swagger_specs/Flowroute_API_01172018.json
- type: x-api-gallery
  url: http://evrythng.api.gallery.streamdata.io
- type: x-crunchbase
  url: https://crunchbase.com/organization/flowroute
- type: x-email
  url: legal@flowroute.com
- type: x-twitter
  url: https://twitter.com/flowroute
- type: x-website
  url: http://developer.flowroute.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---