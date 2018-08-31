{
  "info": {
    "name": "FlowRoute API List Available Area Codes",
    "_postman_id": "16dab148-7691-4375-a8b1-863c4cac9e04",
    "description": "Returns a list of all Numbering Plan Area (NPA) codes containing purchasable phone numbers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Messaging",
      "item": [
        {
          "id": "928ad418-e9b8-4235-b7da-2057f3beeb24",
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
              "id": "be536df8-2c12-469d-a028-3e21db945e2e"
            }
          ]
        },
        {
          "id": "0ee794aa-ef90-457d-bbb0-8593821c4f90",
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
              "id": "dfd81a20-cef4-4384-849a-588f52a2dc77"
            }
          ]
        },
        {
          "id": "c14d7374-8869-421d-b063-82864ea0fff5",
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
              "id": "65508ea6-c07d-401f-b1df-c4f784a55112"
            }
          ]
        },
        {
          "id": "a3efb638-52a0-4cb6-9868-5258e9f03ea6",
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
              "id": "670cb3cb-cd08-4d68-96fe-ff296d346a6a"
            }
          ]
        },
        {
          "id": "23049e04-e38e-4bf6-a6a3-69db50fe5e5c",
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
              "id": "8a9b0546-c643-4e56-bc8c-1c6097ad72b7"
            }
          ]
        },
        {
          "id": "5d742401-4a1f-47d7-85b0-321852df78a7",
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
              "id": "fc1d776c-a365-4241-8fbb-dada7441c637"
            }
          ]
        },
        {
          "id": "6221b17d-a2f2-4eed-9d06-3cd7b27bee36",
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
              "id": "db0b7cef-237c-40c1-af7d-179f05d23b1d"
            }
          ]
        },
        {
          "id": "9e23096c-2906-4325-ab08-cb3dd59795c1",
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
              "id": "7e091040-8a6e-466d-a286-d622b6955fed"
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