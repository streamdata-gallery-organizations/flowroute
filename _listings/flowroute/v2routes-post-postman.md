{
  "info": {
    "name": "FlowRoute API Create an Inbound Route",
    "_postman_id": "3fd16951-776c-45f9-b87e-1f524a4e3e31",
    "description": "Creates a new inbound route which can then be associated with phone numbers. Please see \"List Inbound Routes\" to review the route values that you can associate with your Flowroute phone numbers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Messaging",
      "item": [
        {
          "id": "4aee1d85-a060-4000-883e-3abf38a36b68",
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
              "id": "ebe0fda2-f3b6-42dd-b915-46c291d3e332"
            }
          ]
        },
        {
          "id": "fe510314-4823-40b0-9ff6-78b0fdb462fd",
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
              "id": "23fa743b-f58b-49c5-b0aa-c7c9f332622e"
            }
          ]
        },
        {
          "id": "6bace17c-ff64-46ef-9a63-aa1e653eb220",
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
              "id": "742a4a8c-3334-47b4-9858-0b6b4a00e973"
            }
          ]
        },
        {
          "id": "f13c705b-8cb3-4143-82ea-3629fa856d82",
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
              "id": "22e359fe-db66-46e2-9996-4f586897f3db"
            }
          ]
        },
        {
          "id": "22679135-f4fe-4ebc-8630-e6076e3dc2df",
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
              "id": "3895a5ce-9bcd-4922-b820-acd18c3d8ae8"
            }
          ]
        },
        {
          "id": "a3bf347c-c4e0-4fae-88cf-c781e886f567",
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
              "id": "801bce7b-34bc-40f6-9f15-38cac743f647"
            }
          ]
        },
        {
          "id": "79bccd76-072c-47d4-bdc7-861f38ba5581",
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
              "id": "26c553c2-2488-491e-82a3-c715fd3e6521"
            }
          ]
        },
        {
          "id": "ae01bf40-bba3-4577-8148-f1107a39b056",
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
              "id": "c3ed5434-1e30-4731-8857-bd554702d9e3"
            }
          ]
        },
        {
          "id": "58cf2ab9-999f-45a7-b4e1-c64461ed64b3",
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
              "id": "cc901ec3-f29e-4ee4-98f7-ab069074b02b"
            }
          ]
        },
        {
          "id": "b41e357b-7ddd-462d-9b82-4089d7ee0d57",
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
              "id": "9e16d97b-0982-4d00-ab72-6d0c31a38f5b"
            }
          ]
        },
        {
          "id": "444c3f71-cd1e-4a83-96cf-1ce91383186e",
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
              "id": "de922b08-582a-4a07-bfaa-a38f24b12fa3"
            }
          ]
        },
        {
          "id": "2c579d49-ed48-407d-b19c-914a0316316a",
          "name": "creates-a-new-inbound-route-which-can-then-be-associated-with-phone-numbers-please-see-list-inbound-",
          "request": {
            "url": "{{default}}/v2/routes",
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
            "description": "Creates a new inbound route which can then be associated with phone numbers. Please see \"List Inbound Routes\" to review the route values that you can associate with your Flowroute phone numbers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f86e22d7-84c0-4359-90a3-165b2e4f9ead"
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