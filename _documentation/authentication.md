---
title: Authentication
position_number: 2
parameters:
  - name:
    content:
content_markdown: |-
  This is the API for old ZWave compatibility that can be ran untop of a parallel processing mesh network

  Add the API key to all requests as a GET parameter.

  Nothing will work unless you include the Device ID
  {: .error}
left_code_blocks:
  - code_block:
    title:
    language:
right_code_blocks:
  - code_block: |2-
       [
       "http://10.0.0.225:8080"
       ]
    title: All the Devices
    language: json
  - code_block: |2-
       {
       "uri": "http://10.0.0.220:8080",
       "id": "0729a580-2240-11e6-9eb5-0002a5d5c51b"
       }
    title: Device ID Registeration
    language: json
---
