{
  "info": {
    "name": "BBC Nitro List all Master Brands",
    "_postman_id": "a08168ba-6664-43f3-8a36-1b5954a58e0c",
    "description": "List all Master Brands",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "5149dfd2-f081-4492-a590-8b16cad608dc",
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
              "id": "b079ea74-81c2-49f8-b045-73cd6b09e0cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Availabilities",
      "item": [
        {
          "id": "c3d94a63-ce35-4089-828c-2bba9c1ae943",
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
              "id": "40bbcd5f-b4ac-4bc5-8b9c-2ccee061eb68"
            }
          ]
        }
      ]
    },
    {
      "name": "Broadcasts",
      "item": [
        {
          "id": "5c7264c4-457f-4b1a-947b-f92e745ea4eb",
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
              "id": "1bcaf84d-4d3f-4559-89df-aa51a62196db"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "11384b81-52d4-48ab-bc5e-0db3ab00e773",
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
              "id": "77c2c361-e247-4475-b168-4ba405ebd7dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Images",
      "item": [
        {
          "id": "73772463-2280-4131-8287-67d0e75284e1",
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
              "id": "47c26e42-f57f-4a14-bc40-13053f90d75a"
            }
          ]
        }
      ]
    },
    {
      "name": "Items",
      "item": [
        {
          "id": "e3524720-8eaa-4ad3-b981-7b0551c02268",
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
              "id": "f4c89941-88e2-41b7-9a44-6f77f3745cc4"
            }
          ]
        }
      ]
    },
    {
      "name": "Master",
      "item": [
        {
          "id": "68736185-63b4-49c7-884a-de597b541008",
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
              "id": "dd3eb5bc-bcfc-4ce7-aa29-38f7c1033b83"
            }
          ]
        }
      ]
    }
  ]
}