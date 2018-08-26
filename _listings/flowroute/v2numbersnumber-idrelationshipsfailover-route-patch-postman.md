{
  "info": {
    "name": "FlowRoute API Update Failover Voice Route for a Phone Number",
    "_postman_id": "6ef151c9-3058-47fb-90ce-cd496bfae889",
    "description": "Use this endpoint to update the failover voice route for a phone number. You must create the route first by following \"Create an Inbound Route\". You can then assign the created route by specifying its value in a PATCH request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Messaging",
      "item": [
        {
          "id": "ab9ceb53-f542-4808-afcd-258dff97f590",
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
              "id": "fbaab25a-625c-4538-9446-5b365057f3fc"
            }
          ]
        },
        {
          "id": "0edf76af-18d9-480d-84d0-af3210b8b16c",
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
              "id": "ecd1cab9-b148-453b-b16b-ad028b7c0a61"
            }
          ]
        },
        {
          "id": "58574a36-cbdf-46fa-a2a1-c033770d7d91",
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
              "id": "254c99a6-f035-416d-98ec-9114b1ceb205"
            }
          ]
        },
        {
          "id": "b79fcb05-a7fc-4be6-9c6f-4a2e7ad27d6a",
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
              "id": "1b640534-8833-4bea-ac06-cb46c7697ca6"
            }
          ]
        },
        {
          "id": "5e8475a6-500c-4c6d-92bf-1c95f225e93c",
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
              "id": "86997201-49e8-4d11-94cf-201cdd57f396"
            }
          ]
        },
        {
          "id": "b3febd33-3206-41ad-9d3b-bdeb2c01238b",
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
              "id": "de1f6ac7-ce58-4f0a-93e2-75db1c10181a"
            }
          ]
        },
        {
          "id": "50a48211-b0e0-49e7-8264-5c75ef95b935",
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
              "id": "b8e382b3-6b02-4e80-a3da-13f3e69fd101"
            }
          ]
        },
        {
          "id": "5d89dce1-6664-48db-9d32-9586b0eeda31",
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
              "id": "01921b4a-53f1-441f-bc31-a00f39901d13"
            }
          ]
        },
        {
          "id": "7233d563-d603-40b1-8428-3cdd0fa868e7",
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
              "id": "59e013b8-755a-49ee-bdfd-050fca73b43d"
            }
          ]
        },
        {
          "id": "c8963986-4aad-42a4-91a8-b8cf66cb0921",
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
              "id": "8cb595f7-127d-4e19-b78c-c66d65126875"
            }
          ]
        },
        {
          "id": "1fac7d23-3cde-4c29-85e4-3019f090006f",
          "name": "use-this-endpoint-to-update-the-failover-voice-route-for-a-phone-number-you-must-create-the-route-fi",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v2/numbers/:number_id/relationships/failover_route"
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
            "description": "Use this endpoint to update the failover voice route for a phone number. You must create the route first by following \"Create an Inbound Route\". You can then assign the created route by specifying its value in a PATCH request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09edc551-e3b5-45bb-aa52-1c0d77c7bac5"
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