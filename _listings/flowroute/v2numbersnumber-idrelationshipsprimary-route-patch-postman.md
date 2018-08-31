{
  "info": {
    "name": "FlowRoute API Update Primary Voice Route for a Phone Number",
    "_postman_id": "a9de1e19-391b-4ff2-bcd7-802dd2330152",
    "description": "Use this endpoint to update the primary voice route for a phone number. You must create the route first by following \"Create an Inbound Route\". You can then assign the created route by specifying its value in a PATCH request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Messaging",
      "item": [
        {
          "id": "126eaf97-3ded-4a31-be76-8d688f42933d",
          "name": "retrieves-a-list-of-message-detail-records-mdrs-within-a-specified-date-range-date-and-time-is-based",
          "request": {
            "url": "{{default}}/v2.1/messages?end_date=%7B%7D&limit=%7B%7D&offset=%7B%7D&start_date=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of Message Detail Records (MDRs) within a specified date range. Date and time is based on Coordinated Universal Time (UTC)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc19a993-1a52-4c0f-a6b1-a07ef040ae07"
            }
          ]
        },
        {
          "id": "1461ee6c-9d9b-4329-be1e-ec357fbe63ee",
          "name": "sends-an-sms-or-mms-from-a-flowroute-long-code-or-tollfree-phone-number-to-another-valid-phone-numbe",
          "request": {
            "url": "{{default}}/v2.1/messages",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Sends an SMS or MMS from a Flowroute long code or toll-free phone number to another valid phone number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1426144c-3a9b-4200-8bc8-a9cae86cc9f4"
            }
          ]
        },
        {
          "id": "6ff5f178-cd77-4de1-951c-759ed8f89a44",
          "name": "searches-for-a-specific-message-record-id-and-returns-a-message-detail-record-in-mdr2-format",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v2.1/messages/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Searches for a specific message record ID and returns a Message Detail Record (in MDR2 format)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a8f6a45-044b-48b8-af7b-504c92b69ffd"
            }
          ]
        },
        {
          "id": "5ef113ec-8428-4ba8-83e4-f39e6ac4d9fc",
          "name": "returns-a-list-of-all-phone-numbers-currently-on-your-flowroute-account-the-response-includes-detail",
          "request": {
            "url": "{{default}}/v2/numbers?contains=%7B%7D&ends_with=%7B%7D&limit=%7B%7D&offset=%7B%7D&starts_with=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all phone numbers currently on your Flowroute account. The response includes details such as the phone number's rate center, state, number type, and whether CNAM Lookup is enabled for that number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "129f3f9a-ed24-476d-acb9-146bd5e0c2cf"
            }
          ]
        },
        {
          "id": "c0e23c87-b7b3-44bf-91a9-035c7b4cdce8",
          "name": "lists-all-of-the-information-associated-with-any-of-the-phone-numbers-in-your-account-including-bill",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v2/numbers/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the information associated with any of the phone numbers in your account, including billing method, primary voice route, and failover voice route."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8fc8316-6738-4f9f-a1e6-c48d2425775f"
            }
          ]
        },
        {
          "id": "26d6add5-8f98-414b-a08b-00479f570fde",
          "name": "lets-you-purchase-a-phone-number-from-available-flowroute-inventory",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v2/numbers/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lets you purchase a phone number from available Flowroute inventory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54fc6ffb-47e8-4613-b983-b0e615f207fe"
            }
          ]
        },
        {
          "id": "c9684776-0cce-4afb-bb54-f2d465b2b38c",
          "name": "this-endpoint-lets-you-search-for-phone-numbers-by-state-or-rate-center-or-by-your-specified-search-",
          "request": {
            "url": "{{default}}/v2/numbers/available?contains=%7B%7D&ends_with=%7B%7D&limit=%7B%7D&offset=%7B%7D&rate_center=%7B%7D&starts_with=%7B%7D&state=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint lets you search for phone numbers by state or rate center, or by your specified search value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d417cd25-c805-4598-b797-dceb9f58cc87"
            }
          ]
        },
        {
          "id": "c04f3189-7905-42e2-9b47-e84b0caa412a",
          "name": "returns-a-list-of-all-numbering-plan-area-npa-codes-containing-purchasable-phone-numbers",
          "request": {
            "url": "{{default}}/v2/numbers/available/areacodes?limit=%7B%7D&max_setup_cost=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all Numbering Plan Area (NPA) codes containing purchasable phone numbers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87bbf32c-ef28-4d63-961e-ad895ae31a8f"
            }
          ]
        },
        {
          "id": "1f84a027-8bf5-48e0-8d96-809abcac36a1",
          "name": "returns-a-list-of-all-central-office-exchange-codes-containing-purchasable-phone-numbers",
          "request": {
            "url": "{{default}}/v2/numbers/available/exchanges?areacode=%7B%7D&limit=%7B%7D&max_setup_cost=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all Central Office (exchange) codes containing purchasable phone numbers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d47767a-c48d-4f39-a1ef-5085cb5baeac"
            }
          ]
        },
        {
          "id": "3cdeb2b8-f310-4df9-a849-351cff70d264",
          "name": "use-this-endpoint-to-update-the-primary-voice-route-for-a-phone-number-you-must-create-the-route-fir",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v2/numbers/:number_id/relationships/primary_route"
              ],
              "variable": [
                {
                  "id": "number_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use this endpoint to update the primary voice route for a phone number. You must create the route first by following \"Create an Inbound Route\". You can then assign the created route by specifying its value in a PATCH request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "618c1071-ee4c-40ef-b8ca-90667e0e6cdd"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/"
    }
  ]
}