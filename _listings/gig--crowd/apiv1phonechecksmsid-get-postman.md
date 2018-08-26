{
  "info": {
    "name": "GIGANDCROWD Get Phone Check Smsid",
    "_postman_id": "9886477b-9b05-48a5-9e59-e8f37776928b",
    "description": "Get phone check smsid.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Phone",
      "item": [
        {
          "id": "e8100481-2f0c-4d36-b102-9e004e78ff14",
          "name": "getApiV1PhoneCheckSms",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/phone/check/:smsId"
              ],
              "variable": [
                {
                  "id": "smsId",
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
            "description": "Get phone check smsid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e86c10f1-c6f0-4d4d-aae7-cd4e35723bf9"
            }
          ]
        }
      ]
    }
  ]
}