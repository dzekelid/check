{
  "info": {
    "name": "SendGrid Get Mail Settings Spam Check",
    "_postman_id": "34553012-242d-4a9e-93b1-dabbeda391c0",
    "description": "**This endpoint allows you to retrieve your current Spam Checker mail settings.**\n\nThe spam checker filter notifies you when emails are detected that exceed a predefined spam threshold.\n\nMail settings allow you to tell SendGrid specific things to do to every email that you send to your recipients over SendGrid???s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "ba4a6d29-472a-4b38-9a4a-c6a0801db356",
          "name": "mail_settings.spam_check.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/mail_settings/spam_check?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current Spam Checker mail settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e836cce-3adc-417d-9106-1aee378eb9a6"
            }
          ]
        }
      ]
    }
  ]
}