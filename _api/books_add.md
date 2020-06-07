---
title: /devices
position_number: 1.1
type: post
description: Get devices
parameters:
  - name: skip
    content: Number of records to skip
  - name: limit
    content: Max number of records to return
content_markdown: |-
  limit
  integer($int32)
  Max number of records to return
left_code_blocks:
  - code_block: |-
      $ref: '#/definitions/DeviceRegistrationInfo'
      responses:
        200:
          description: successfully registered device
      });
    title: jQuery
    language: javascript
right_code_blocks:
  - code_block: |-
      {
        "id": 3,
        "title": "The Book Thief",
        "score": 4.3,
        "dateAdded": "5/1/2015"
      }
    title: Response
    language: json
  - code_block: |-
      {
        "error": true,
        "message": "Invalid score"
      }
    title: Error
    language: json
---
