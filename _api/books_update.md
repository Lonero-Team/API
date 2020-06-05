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
      $.ajax({
        "url": "http://api.myapp.com/books/3",
        "type": "PUT",
        "data": {
          "token": "YOUR_APP_KEY",
          "score": 5.0,
          "title": "The Book Stealer"
        },
        "success": function(data) {
          alert(data);
        }
      });
    title: jQuery
    language: javascript
right_code_blocks:
  - code_block: |2-
      {
        "id": 3,
        "title": "The Book Stealer",
        "score": 5,
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
