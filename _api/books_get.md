---
title: /z-wave/:id
position_number: 1.3
type: get
description: Device ID and values
parameters:
  - name:
    content:
content_markdown: |-
  Returns Device ID and Values
left_code_blocks:
  - code_block: |-
      DeviceRegistrationInfo:
       type: object
       properties:
         uri:
         type: string
         format: uri
         example: http://10.0.0.220:8080
          id:
          type: string
           format: uuid
           example: '0729a580-2240-11e6-9eb5-0002a5d5c51b'      
    title: Zone ID
    language: yaml
right_code_blocks:
  - code_block: |2-
      host: virtserver.swaggerhub.com
      basePath: /Lonero/Decentralized-Internet_API/1.0.0
      schemes:       - https      
    title: Host
    language: json
---
