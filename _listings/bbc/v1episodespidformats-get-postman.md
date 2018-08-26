{
  "info": {
    "name": "BBC Nitro Get raw formats",
    "_postman_id": "9db6ef74-d617-463a-9602-63f7ad74c475",
    "description": "Get raw formats",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "V1",
      "item": [
        {
          "id": "f44d6516-cb5f-4aee-8fa1-7c29c1cbb0ed",
          "name": "Get_Raw_formats",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/episodes/:pid/formats/"
              ],
              "variable": [
                {
                  "id": "pid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get raw formats"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d076a32c-8630-4f56-90a6-c45d672a053b"
            }
          ]
        }
      ]
    }
  ]
}