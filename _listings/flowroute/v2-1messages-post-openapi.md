---
swagger: "2.0"
x-collection-name: Flowroute
x-complete: 0
info:
  title: FlowRoute API Send a Message
  description: Sends an SMS or MMS from a Flowroute long code or toll-free phone number
    to another valid phone number.
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