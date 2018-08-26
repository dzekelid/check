{
  "info": {
    "name": "Clockwork SMS Check Balance",
    "_postman_id": "c5c9324a-1fd0-479e-a2ed-3c9292c6b6a8",
    "description": "Check how much credit you have left on your account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Check",
      "item": [
        {
          "id": "649e014b-fa66-4a25-88e8-cf82f0dab0c4",
          "name": "getBalance",
          "request": {
            "url": "http://api.clockworksms.com/http/balance?Key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Check how much credit you have left on your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8b92463-04f0-4bbf-98c7-befa6ccb6582"
            }
          ]
        }
      ]
    }
  ]
}