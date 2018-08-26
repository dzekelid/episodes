{
  "info": {
    "name": "BBC Nitro Get raw ancestors",
    "_postman_id": "fac2fbe7-0d46-4e26-a8b6-56c97566011c",
    "description": "Get raw ancestors",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "d052e628-aca9-4dc7-b53a-4c465eeec38b",
          "name": "getAPI",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get API definition"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d899c37c-2dec-4f09-9e53-2d2cae8dd349"
            }
          ]
        }
      ]
    },
    {
      "name": "Availabilities",
      "item": [
        {
          "id": "0c231c18-95dd-4499-be12-28cfde12e366",
          "name": "listAvailability",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/availabilities?availability=%7B%7D&debug=%7B%7D&descendants_of=%7B%7D&media_set=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D&territory=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Discover details of on-demand availability for programmes and their versions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b879d1f4-70db-45f7-b61b-d7602024f1ae"
            }
          ]
        }
      ]
    },
    {
      "name": "Broadcasts",
      "item": [
        {
          "id": "9038f7fb-c38d-4715-82ee-16fac3de565d",
          "name": "listBroadcasts",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/broadcasts?authority=%7B%7D&descendants_of=%7B%7D&end_from=%7B%7D&end_to=%7B%7D&format=%7B%7D&genre=%7B%7D&id=%7B%7D&item=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&people=%7B%7D&pid=%7B%7D&q=%7B%7D&schedule_day=%7B%7D&schedule_day_from=%7B%7D&schedule_day_to=%7B%7D&service_master_brand=%7B%7D&sid=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D&start_from=%7B%7D&start_to=%7B%7D&version=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch metadata about linear Broadcasts and Services, allowing the generation of Television and Radio schedules and other datasets for broadcast items. Use /schedules instead of this feed as it is more efficient. Broadcasts will be deprecated in the future."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0da414ad-4992-460e-a412-dd243a8edbc2"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "db727629-63c6-4ef9-a39b-e5dd7658745d",
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
              "id": "acc54997-aa0d-4681-ba24-822b2a48e711"
            }
          ]
        }
      ]
    },
    {
      "name": "Images",
      "item": [
        {
          "id": "a2d56b26-6830-4e85-84fe-2a69abca31e4",
          "name": "listImages",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/images?embargoed=%7B%7D&group=%7B%7D&image_type=%7B%7D&is_alternate_image_for=%7B%7D&is_image_for=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&pid=%7B%7D&q=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Find metadata for images, particularly those in galleries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f23dd5f6-5f6c-483a-987d-1100b2deaa49"
            }
          ]
        }
      ]
    },
    {
      "name": "Items",
      "item": [
        {
          "id": "4c43d453-58ab-4cea-a0e7-6deca5e842a1",
          "name": "listItems",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/items?authority=%7B%7D&id=%7B%7D&id_type=%7B%7D&item_type=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&people=%7B%7D&pid=%7B%7D&programme=%7B%7D&q=%7B%7D&segment_event=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Look inside programmes to find segments: chapters, tracks and more"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e3851c3-7877-4bc9-9d4c-0792911785a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Master",
      "item": [
        {
          "id": "0791c839-5d8b-4b3d-9393-0abdcb49ec5b",
          "name": "listMasterbrands",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/master_brands?mid=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&q=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all Master Brands"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76f80aa1-8b3b-4972-957c-6ecab9bccf8b"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "d7352ff8-42c8-4614-8f9c-88e7afc9129f",
          "name": "listPeople",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/people?authority=%7B%7D&has_external_id=%7B%7D&id=%7B%7D&id_type=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&pid=%7B%7D&programme=%7B%7D&q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The People feed allows you to search for the people and groups that contribute to programmes. This is the starting point for cast and crew credits, as well as finding contributors using external IDs (such as Wikipedia URLs)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5600a5c-403e-49c0-97c6-4e4aa806f6b1"
            }
          ]
        }
      ]
    },
    {
      "name": "Pips",
      "item": [
        {
          "id": "4f04032a-66de-49e9-92b0-f258d7e7ed98",
          "name": "listPips",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/pips?page=%7B%7D&page_size=%7B%7D&q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Look inside pips entities"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5718bb54-4b1c-472e-a70e-5fc20055e6c7"
            }
          ]
        }
      ]
    },
    {
      "name": "Programme",
      "item": [
        {
          "id": "708a7ce9-3b9f-46ae-8a5c-d8a6f075b222",
          "name": "listProgrammeDetails",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/programme_details?page=%7B%7D&page_size=%7B%7D&partner_pid=%7B%7D&pid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Exposes programme information for a single pid"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "463dc53e-4a0c-4d85-a5d9-895a17581e25"
            }
          ]
        }
      ]
    },
    {
      "name": "Programmes",
      "item": [
        {
          "id": "b1bcb4a6-d9d8-4e8b-9947-8354ef606a24",
          "name": "listProgrammes",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/programmes?audio_described=%7B%7D&availability=%7B%7D&availability_entity_type=%7B%7D&availability_from=%7B%7D&availability_type=%7B%7D&children_of=%7B%7D&descendants_of=%7B%7D&duration=%7B%7D&embargoed=%7B%7D&entity_type=%7B%7D&format=%7B%7D&genre=%7B%7D&group=%7B%7D&initial_letter=%7B%7D&initial_letter_end=%7B%7D&initial_letter_start=%7B%7D&initial_letter_strict=%7B%7D&item=%7B%7D&master_brand=%7B%7D&media_set=%7B%7D&media_type=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&payment_type=%7B%7D&people=%7B%7D&pid=%7B%7D&promoted_for=%7B%7D&q=%7B%7D&signed=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D&tag_name=%7B%7D&tag_scheme=%7B%7D&tleo=%7B%7D&version=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch metadata about Programmes (brands, series, episodes, clips). By applying different filter restrictions this feed can be used in many ways, for example to retrieve all series belonging to a brand, all the episodes and/or clips for a specific series, or any TLEO objects for a masterbrand. Other filters permit restricting to specific formats and/or genres, and you can request specific versions (for example Signed or Audio-Described). Parameters may be combined in any way suitable for your application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f724e0a-1a74-4542-8d60-ea731cd77315"
            }
          ]
        }
      ]
    },
    {
      "name": "Promotions",
      "item": [
        {
          "id": "79888677-31c2-4fa6-a0f9-8a8ea52a2deb",
          "name": "listPromotions",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/promotions?context=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&pid=%7B%7D&promoted_by=%7B%7D&promoted_for=%7B%7D&q=%7B%7D&status=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details of short-term editorially curated \"promotions\", for instance those programmes featured on iPlayer today"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d8d3588-4385-41d7-9b11-080b012474c5"
            }
          ]
        }
      ]
    },
    {
      "name": "Schedules",
      "item": [
        {
          "id": "08fc2d7a-a1cb-44c1-8515-2c46f91c35a0",
          "name": "listSchedules",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/schedules?authority=%7B%7D&descendants_of=%7B%7D&end_from=%7B%7D&end_to=%7B%7D&format=%7B%7D&genre=%7B%7D&group=%7B%7D&id=%7B%7D&id_type=%7B%7D&item=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&people=%7B%7D&pid=%7B%7D&q=%7B%7D&repeat=%7B%7D&schedule_day=%7B%7D&schedule_day_from=%7B%7D&schedule_day_to=%7B%7D&service_master_brand=%7B%7D&sid=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D&start_from=%7B%7D&start_to=%7B%7D&version=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Dates, Times, Schedules: when and where are programmes being shown?"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e281131d-cd47-4732-a9b7-a6a92276c92c"
            }
          ]
        }
      ]
    },
    {
      "name": "Schema",
      "item": [
        {
          "id": "86c3dd75-27a3-436c-968a-8bcee5e07aac",
          "name": "getXSD",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/schema",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Schema definition"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a3295c9-9ccb-4dbf-830a-cb3cf5b80c58"
            }
          ]
        }
      ]
    },
    {
      "name": "Services",
      "item": [
        {
          "id": "d03e8015-4b47-4335-a4d0-c00584a79a7c",
          "name": "listServices",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/services?end_from=%7B%7D&end_to=%7B%7D&mid=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&q=%7B%7D&service_type=%7B%7D&sid=%7B%7D&start_from=%7B%7D&start_to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The services feed exposes the linear broadcast \"services\" from PIPs. These are the actual services which broadcast programmes (eg bbc_one_oxford is the service for BBC One in Oxford)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18e4bf8e-f221-4de5-b7a9-97b0b4c907d6"
            }
          ]
        }
      ]
    },
    {
      "name": "V1",
      "item": [
        {
          "id": "9115a909-3afe-415f-ac30-9c2cb62aae8d",
          "name": "Get_Raw_brand",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/brands/:pid"
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
            "description": "Get raw brand"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7b642ad-7680-4a6b-93b0-7bc75d45b2d4"
            }
          ]
        },
        {
          "id": "ca5ad9a3-416d-4bd7-bbc4-c48cb2577937",
          "name": "Get_Raw_brand franchises",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/brands/:pid/franchises/"
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
            "description": "Get raw brand franchises"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c75658d-b971-4ced-9938-1d75cf5e2ea6"
            }
          ]
        },
        {
          "id": "39b9564e-c264-4c6d-81d3-9a93873506a3",
          "name": "Get_Raw_episode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/episodes/:pid"
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
            "description": "Get raw episode"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e72b06b2-f3aa-486c-abb6-e8791445e47f"
            }
          ]
        },
        {
          "id": "a750c515-99fd-4580-bfb1-80b4b925fe85",
          "name": "Get_Raw_ancestors",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/episodes/:pid/ancestors/"
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
            "description": "Get raw ancestors"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0560294e-f396-402a-9291-d85c6f6cca27"
            }
          ]
        }
      ]
    }
  ]
}