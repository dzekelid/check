{
  "info": {
    "name": "Predix Access Control Monitoring API that allows to check the ACS heartbeat",
    "_postman_id": "15938f94-a0a5-489e-aa9c-eced5dfab58f",
    "description": "Monitoring api that allows to check the acs heartbeat.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "638a8792-f951-4dc3-b112-145cb8ac8f38",
          "name": "getHeartBeatUsingGET",
          "request": {
            "url": "http://predix-acs.run.aws-usw02-pr.ice.predix.io/monitoring/heartbeat",
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
            "description": "Monitoring api that allows to check the acs heartbeat."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "1bd4c9af-cf07-4c75-b815-332ad7391871"
            }
          ]
        }
      ]
    }
  ]
}