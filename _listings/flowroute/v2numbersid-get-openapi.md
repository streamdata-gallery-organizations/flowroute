---
swagger: "2.0"
x-collection-name: Flowroute
x-complete: 0
info:
  title: FlowRoute API Phone Number Details
  description: Lists all of the information associated with any of the phone numbers
    in your account, including billing method, primary voice route, and failover voice
    route.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2.1/messages:
    post:
      summary: Send a Message
      description: Sends an SMS or MMS from a Flowroute long code or toll-free phone
        number to another valid phone number.
      operationId: sends-an-sms-or-mms-from-a-flowroute-long-code-or-tollfree-phone-number-to-another-valid-phone-numbe
      x-api-path-slug: v2-1messages-post
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Send
      - Message
    get:
      summary: Look Up a Set of Messages
      description: Retrieves a list of Message Detail Records (MDRs) within a specified
        date range. Date and time is based on Coordinated Universal Time (UTC).
      operationId: retrieves-a-list-of-message-detail-records-mdrs-within-a-specified-date-range-date-and-time-is-based
      x-api-path-slug: v2-1messages-get
      parameters:
      - in: query
        name: end_date
        description: The ending date and time, in UTC, on which to perform an MDR
          search
      - in: query
        name: limit
        description: The number of MDRs to retrieve at one time
      - in: query
        name: offset
        description: The number of MDRs to skip when performing a query
      - in: query
        name: start_date
        description: The beginning date and time, in UTC, on which to perform an MDR
          search
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Look
      - Up
      - Set
      - Of
      - Messages
  /v2.1/messages/{id}:
    get:
      summary: Look Up a Message Detail Record
      description: Searches for a specific message record ID and returns a Message
        Detail Record (in MDR2 format).
      operationId: searches-for-a-specific-message-record-id-and-returns-a-message-detail-record-in-mdr2-format
      x-api-path-slug: v2-1messagesid-get
      parameters:
      - in: path
        name: id
        description: The unique message detail record identifier (MDR ID) of any message
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Look
      - Up
      - Message
      - Detail
      - Record
  /v2/numbers:
    get:
      summary: Account Phone Numbers
      description: Returns a list of all phone numbers currently on your Flowroute
        account. The response includes details such as the phone number's rate center,
        state, number type, and whether CNAM Lookup is enabled for that number.
      operationId: returns-a-list-of-all-phone-numbers-currently-on-your-flowroute-account-the-response-includes-detail
      x-api-path-slug: v2numbers-get
      parameters:
      - in: query
        name: contains
        description: Retrieves phone numbers containing the specified value
      - in: query
        name: ends_with
        description: Retrieves phone numbers that end with the specified value
      - in: query
        name: limit
        description: Limits the number of items to retrieve
      - in: query
        name: offset
        description: Offsets the list of phone numbers by your specified value
      - in: query
        name: starts_with
        description: Retrieves phone numbers that start with the specified value
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Account
      - Phone
      - Numbers
  /v2/numbers/{id}:
    get:
      summary: Phone Number Details
      description: Lists all of the information associated with any of the phone numbers
        in your account, including billing method, primary voice route, and failover
        voice route.
      operationId: lists-all-of-the-information-associated-with-any-of-the-phone-numbers-in-your-account-including-bill
      x-api-path-slug: v2numbersid-get
      parameters:
      - in: path
        name: id
        description: Phone number to search for which must be a number that you own
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Phone
      - Number
      - Details
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