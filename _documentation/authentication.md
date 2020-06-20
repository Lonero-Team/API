---
title: Authentication
position_number: 2
parameters:
  - name:
    content:
content_markdown: |-
  You need to be authenticated for all API requests. You can generate an API key in your developer dashboard.

  Add the API key to all requests as a GET parameter.

  Nothing will work unless you include this API key
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
