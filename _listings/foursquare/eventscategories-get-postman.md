{
  "info": {
    "name": "Foursquare Get Events Categories",
    "_postman_id": "fd013c49-5285-4796-b32d-3a786847fd94",
    "description": "/events/{EVENT_ID}",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "50d7aa3c-af51-4de5-b867-1c33e44a0e99",
          "name": "eventsevent-id",
          "request": {
            "url": "http://api.foursquare.com/v2/events/categories?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/{EVENT_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8affe2b-61a5-4f5c-8d03-d4a5fd415df7"
            }
          ]
        }
      ]
    }
  ]
}