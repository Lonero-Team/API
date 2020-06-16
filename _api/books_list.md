---
title: /z-wave
position_number: 1.0
type: get
description: Device ID, value and time unit
parameters:
  - name: deviceId
    content: Calls the device ID
  - name: SetState
    content: Set the state of devices
content_markdown: |-
  x-swagger-router-controller: "ZWave"
  /lighting/dimmers/{deviceId}/{value}/timer/{timeunit}:

  Sets device Id response through ZWave
left_code_blocks:
  - code_block: |-
      $ref: '#/definitions/ApiResponse'
    title: API Response
    language: javascript
  - code_block: |-
      $ref: '#/definitions/LightingSummary'
    title: Lighting Summary
    language: javascript
  - code_block: |-
     {
      "zones": [
      {
      "id": "string",
      "name": "string",
      "deviceId": 0,
      "deviceType": "dimmer",
      "zone": "string"
         }
       ],
     "zoneStatus": [
       {
       "id": "string",
       "name": "string",
       "lastUpdate": "2020-06-16T23:40:29.510Z",
       "level": 0
         }
       ]
     }
    title: Zone Status
    language: javascript
  - code_block: |-
      curl http://sampleapi.readme.com/orders?key=YOUR_APP_KEY
    title: Curl
    language: bash
right_code_blocks:
  - code_block: |2-
      [
        {
          "id": 1,
          "title": "The Hunger Games",
          "score": 4.5,
          "dateAdded": "12/12/2013"
        },
        {
          "id": 1,
          "title": "The Hunger Games",
          "score": 4.7,
          "dateAdded": "15/12/2013"
        },
      ]
    title: Response
    language: json
  - code_block: |2-
      {
        "error": true,
        "message": "Invalid offset"
      }
    title: Error
    language: json
---
