{
  "info": {
    "name": "FlowRoute API Account Phone Numbers",
    "_postman_id": "1d54b5f7-40a8-40b9-b6bb-218096a64ecf",
    "description": "Returns a list of all phone numbers currently on your Flowroute account. The response includes details such as the phone number's rate center, state, number type, and whether CNAM Lookup is enabled for that number.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Messaging",
      "item": [
        {
          "id": "961e7a86-0bd3-4dcb-8372-815efa452839",
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
              "id": "7b909e44-cf83-48b2-862b-30dd1d128796"
            }
          ]
        },
        {
          "id": "986e6723-4c5d-4203-965e-56668adf599c",
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
              "id": "411b1992-3d58-4cde-8f78-225f0f8d2418"
            }
          ]
        },
        {
          "id": "49f95c42-a072-4ac3-8c9a-7f8fe8ce2322",
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
              "id": "31b5af7a-c586-4a60-978f-f3f246e6e4aa"
            }
          ]
        },
        {
          "id": "edbd3242-a233-440f-b916-c3195faf6938",
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
              "id": "b500f920-c368-451c-8bea-0ec2abd0f205"
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