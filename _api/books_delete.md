---
title: /devices/:id
position_number: 1.5
type: post
description: Post devices
parameters:
  - device:
    id:
content_markdown: |-
  Successfully registered device
left_code_blocks:
  - code_block: |-
      [
        "http://10.0.0.225:8080"
      ]      
    title: All the Devices
    language: json
right_code_blocks:
  - code_block: |2-
      {
        "uri": "http://10.0.0.220:8080",
        "id": "0729a580-2240-11e6-9eb5-0002a5d5c51b"
      }      
    title: Device
    language: json
  - code_block: |2-
      $ref: '#/definitions/DeviceRegistrationInfo'
    title: Device Registration Info
    language: json
---
