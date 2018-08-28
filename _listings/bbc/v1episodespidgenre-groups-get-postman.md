{
  "info": {
    "name": "BBC Nitro Get raw genre groups",
    "_postman_id": "165bfdcd-5c03-4caf-9188-2382c2660394",
    "description": "Get raw genre groups",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "6d812d22-b41d-4f66-81b1-4ad7d2664367",
          "name": "listGroups",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/groups?embargoed=%7B%7D&for_descendants_of=%7B%7D&for_programme=%7B%7D&group=%7B%7D&group_type=%7B%7D&member=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&pid=%7B%7D&q=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Long-lived curated collections of programmes and more, including Collections, Seasons, Franchises and Galleries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61a01eb9-2a17-4eb2-92d6-9206e1b2a06c"
            }
          ]
        }
      ]
    },
    {
      "name": "V1",
      "item": [
        {
          "id": "9514931c-76f6-4083-b6b5-b5508e7aac1a",
          "name": "Get_Raw_genre_groups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/episodes/:pid/genre_groups/"
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
            "description": "Get raw genre groups"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb8d5c4e-7e66-4430-9d62-a2f11c27dd77"
            }
          ]
        }
      ]
    }
  ]
}