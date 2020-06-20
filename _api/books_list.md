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
    language: yaml
  - code_block: |-
      $ref: '#/definitions/LightingSummary'
    title: Lighting Summary
    language: yaml
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
    language: json
  - code_block: |-
      $ref: '#/definitions/HeaterState'
    title: HeaterState
    language: json
right_code_blocks:
  - code_block: |2-
      $ref: '#/definitions/TemperatureZone'
    title: Temp Zone
    language: json
  - code_block: |2-
      $ref: '#/definitions/TemperatueZoneStatus'
    title: Temp Zone Status
    language: json
---
