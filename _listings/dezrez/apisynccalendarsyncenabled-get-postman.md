{
  "info": {
    "name": "Dezrez check if the calendar sync is enabled for this user\r\nthis could be used to enabled/disable the calendar setup button",
    "_postman_id": "ea466d57-d07c-4d86-a529-e0f0bbfc5860",
    "description": "Check if the calendar sync is enabled for this user\r\nthis could be used to enabled/disable the calendar setup button.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Initially",
      "item": [
        {
          "id": "3934d771-56c0-4024-aed5-d735f674f538",
          "name": "Sync_CalendarBypersonId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/sync/calendarsetup/:personId"
              ],
              "variable": [
                {
                  "id": "personId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Initially setup the calendar, create rezi calendar, copy upto 16 days prior into calendar, create a subscription channel for the callback."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1eab66c9-b8ab-4801-9734-31a26c43cb09"
            }
          ]
        }
      ]
    },
    {
      "name": "Oauth",
      "item": [
        {
          "id": "4efc4433-23d3-42b6-a4d2-bc933e55d445",
          "name": "Sync_CalendarSyncOauthUrlBypersonId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/sync/calendarsyncoauthurl/:personId"
              ],
              "variable": [
                {
                  "id": "personId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the oauth url for the calendar sync service."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ed978bd-ac35-488e-bf2f-098f116364e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Check",
      "item": [
        {
          "id": "0f1735e0-a789-4b23-8c9e-f2979c5beb36",
          "name": "Sync_CalendarSyncEnabled",
          "request": {
            "url": "http://api.dezrez.com/api/sync/calendarsyncenabled",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Check if the calendar sync is enabled for this user\r\nthis could be used to enabled/disable the calendar setup button."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9473bb4e-7d99-4ba4-8503-beba9ef0654b"
            }
          ]
        }
      ]
    }
  ]
}