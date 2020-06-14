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
    title: jQuery
    language: javascript
right_code_blocks:
  - code_block: |2-
      {
        "id": 3,
        "title": "The Book Thief",
        "score": 4.3,
        "dateAdded": "5/1/2015"
      }
    title: Response
    language: json
  - code_block: |2-
      {
        "error": true,
        "message": "Book doesn't exist"
      }
    title: Error
    language: json
---
