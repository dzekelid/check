{
  "info": {
    "name": "Pay Run.IO Get health check status",
    "_postman_id": "9ab2f74c-9217-483b-9757-30a9b0d81b21",
    "description": "Returns the health status of the application",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Health",
      "item": [
        {
          "id": "a2fb70dc-bd0d-4592-8f2a-5318fce8cd7a",
          "name": "GetHealthCheck",
          "request": {
            "url": "http://api.test.payrun.io/Healthcheck",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the health status of the application"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e146f68e-a234-4deb-843d-38f7c09a67d8"
            }
          ]
        }
      ]
    }
  ]
}