---
title: /z-wave/:id
position_number: 1.4
type: put
description: Device IDs
parameters:
  - name: device
    content: Collect device ids for peers
  - name: deviceId
    content: Set path for collecting device ids
content_markdown: |-
  Set path for the calling of device ids
left_code_blocks:
  - code_block: |-
      {
        "uri": "http://10.0.0.220:8080",
        "id": "0729a580-2240-11e6-9eb5-0002a5d5c51b"
      }      
    title: Device ID JSON
    language: json
right_code_blocks:
  - code_block: |2-
      operationId: "setDimmer"
      parameters:
      - name: "deviceId"
        in: "path"
        required: true
        type: "string"
      - name: "value"
        in: "path"
        required: true
        type: "integer"
        maximum: 100.0
        minimum: 0.0
        format: "int32"      
    title: Parameters
    language: json
    properties:
      id:
        type: string
      name:
        type: string
      lastUpdate:
        type: string
        format: date-time
      level:
        type: integer
        format: int32      
    title: Device State Properties
    language: json
---
