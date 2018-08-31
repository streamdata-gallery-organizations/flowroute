{
  "info": {
    "name": "FlowRoute API Purchase a Phone Number",
    "_postman_id": "6e8b9459-9369-4729-a688-5f3be7ebbfd8",
    "description": "Lets you purchase a phone number from available Flowroute inventory.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Messaging",
      "item": [
        {
          "id": "f0402b2b-e1b6-40b5-a551-a81b51fc4efa",
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
              "id": "30d98e15-282c-442e-a2a2-6993d234cff2"
            }
          ]
        },
        {
          "id": "c1947fc9-515a-4e2a-85d1-00b012392a26",
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
              "id": "e96bf957-4d6f-41e1-a9d0-b7d7914a5484"
            }
          ]
        },
        {
          "id": "f259fdb5-30df-44b1-aea8-379b2b67e631",
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
              "id": "e977bb1d-dac9-4b34-bee8-0380cfcbac85"
            }
          ]
        },
        {
          "id": "35d7d0e4-cbf4-43da-8d4f-498aa38a214a",
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
              "id": "72e15537-bb78-422f-a3e7-87df6560d883"
            }
          ]
        },
        {
          "id": "626c955a-0dd9-40fa-bb99-a6fc08e5e04d",
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
              "id": "ec1c9807-0f42-47a9-a7dd-88f52a70d06d"
            }
          ]
        },
        {
          "id": "f109d70e-be14-4263-b7e0-1af817f71dc3",
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
              "id": "2d99f2cf-07ff-40da-bdec-d5ea3b1a1d34"
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