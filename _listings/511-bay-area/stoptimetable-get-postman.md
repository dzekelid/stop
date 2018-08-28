{
  "info": {
    "name": "Bay Area 511 Transit API Stop Timetable API",
    "_postman_id": "cb67fefc-9068-4075-a8dc-e5d6301fb2cb",
    "description": "San francisco 511 transit stop timetable api.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "511",
      "item": [
        {
          "id": "7bb778bb-4e8b-4306-9f24-d310d6d681e4",
          "name": "LinesGet",
          "request": {
            "url": "http://api.511.org/transit/lines?api_key=%7B%7D&operator_id=%7B%7D",
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
            "description": "San francisco 511 transit lines api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b2bab03-95fd-492c-8835-29381814fabd"
            }
          ]
        },
        {
          "id": "090dabcc-f5da-4ccb-a114-c5638c53efc1",
          "name": "PatternsGet",
          "request": {
            "url": "http://api.511.org/transit/patterns?api_key=%7B%7D&operator_id=%7B%7D&pattern_id=%7B%7D",
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
            "description": "San francisco 511 transit transit patterns api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f04a8288-5c5c-4873-a1b6-a0724dc64ca9"
            }
          ]
        },
        {
          "id": "a681dbfc-7270-41c2-8e8f-e0dfed0ce3de",
          "name": "StopsGet",
          "request": {
            "url": "http://api.511.org/transit/stops?api_key=%7B%7D&operator_id=%7B%7D",
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
            "description": "San francisco 511 transit stops api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56dd7182-b2bf-46ce-aeb9-b007ea1cbf49"
            }
          ]
        },
        {
          "id": "b89ce5d2-cf4f-4512-ab32-cd85f85fcca7",
          "name": "StopMonitoringGet",
          "request": {
            "url": "http://api.511.org/transit/StopMonitoring?agency=%7B%7D&api_key=%7B%7D&stopCode=%7B%7D",
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
            "description": "San francisco 511 transit stop monitoring api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b48fed1-ae77-4400-a624-ea3d17e513ff"
            }
          ]
        },
        {
          "id": "dc41a125-f550-45db-96c4-c7750a6f2973",
          "name": "StoptimetableGet",
          "request": {
            "url": "http://api.511.org/transit/stoptimetable?api_key=%7B%7D&MonitoringRef=%7B%7D&OperatorRef=%7B%7D",
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
            "description": "San francisco 511 transit stop timetable api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "537ca782-7c79-4055-adef-336c7558d5e9"
            }
          ]
        }
      ]
    }
  ]
}