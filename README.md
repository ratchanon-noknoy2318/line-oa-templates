<p align="center">
  <img src="https://res.cloudinary.com/dpa96jvla/image/upload/v1779241423/%E0%B8%AA%E0%B8%81%E0%B8%A3%E0%B8%B5%E0%B8%99%E0%B8%8A%E0%B9%87%E0%B8%AD%E0%B8%95_2026-05-20_084327_qaqnhc.png" width="220"/>
  <img src="https://res.cloudinary.com/dpa96jvla/image/upload/v1779241693/%E0%B8%AA%E0%B8%81%E0%B8%A3%E0%B8%B5%E0%B8%99%E0%B8%8A%E0%B9%87%E0%B8%AD%E0%B8%95_2026-05-20_084806_arsa4m.png" width="220"/>
  <img src="https://res.cloudinary.com/dpa96jvla/image/upload/v1779241747/%E0%B8%AA%E0%B8%81%E0%B8%A3%E0%B8%B5%E0%B8%99%E0%B8%8A%E0%B9%87%E0%B8%AD%E0%B8%95_2026-05-20_084858_se4vfw.png" width="165"/>
</p>

## Example Flex Message (JSON)

Below is an example of a Flex Message used in this system for healthcare communication via LINE Messaging API.

```json
{
  "type": "bubble",
  "hero": {
    "type": "box",
    "layout": "vertical",
    "contents": [
      {
        "type": "image",
        "url": "https://res.cloudinary.com/ds6xq6wbm/image/upload/v1756009686/%E0%B8%84%E0%B8%B7%E0%B8%AD%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3.png",
        "size": "full",
        "aspectRatio": "20:13",
        "aspectMode": "cover"
      },
      {
        "type": "box",
        "layout": "vertical",
        "position": "absolute",
        "width": "100%",
        "height": "100%",
        "backgroundColor": "#00000088",
        "justifyContent": "center",
        "alignItems": "center",
        "contents": [
          {
            "type": "text",
            "text": "Telemedicine",
            "weight": "bold",
            "size": "xxl",
            "color": "#FFFFFF",
            "align": "center"
          },
          {
            "type": "text",
            "text": "บริการปรึกษาแพทย์ทางไกล",
            "size": "lg",
            "color": "#E0E0E0",
            "margin": "md",
            "align": "center"
          }
        ]
      }
    ],
    "paddingAll": "0px"
  },
  "body": {
    "type": "box",
    "layout": "vertical",
    "spacing": "xl",
    "paddingAll": "20px",
    "contents": [
      {
        "type": "box",
        "layout": "vertical",
        "spacing": "sm",
        "contents": [
          {
            "type": "text",
            "text": "พบแพทย์ได้จากทุกที่ สะดวก รวดเร็ว ปลอดภัย",
            "wrap": true,
            "size": "md",
            "weight": "bold",
            "color": "#2C5282"
          },
          {
            "type": "text",
            "text": "บริการปรึกษาแพทย์ทางไกล (Telemedicine) ช่วยให้คุณได้รับคำปรึกษา วินิจฉัย และสั่งยาจากทีมแพทย์ผู้เชี่ยวชาญของเราได้ง่ายๆ ผ่านวิดีโอคอล ไม่ว่าคุณจะอยู่ที่ไหน",
            "wrap": true,
            "size": "sm",
            "color": "#666666",
            "margin": "md"
          }
        ]
      },
      {
        "type": "separator"
      },
      {
        "type": "box",
        "layout": "vertical",
        "spacing": "lg",
        "margin": "lg",
        "contents": [
          {
            "type": "box",
            "layout": "horizontal",
            "spacing": "lg",
            "contents": [
              {
                "type": "box",
                "layout": "vertical",
                "flex": 1,
                "spacing": "sm",
                "paddingAll": "lg",
                "backgroundColor": "#FFFFFF",
                "cornerRadius": "md",
                "borderColor": "#E0E0E0",
                "borderWidth": "1px",
                "alignItems": "center",
                "justifyContent": "center",
                "action": {
                  "type": "uri",
                  "label": "ลงทะเบียน",
                  "uri": "https://kppmch-register.vercel.app/PatientRegister",
                  "altUri": {
                    "desktop": "https://kppmch-register.vercel.app/PatientRegister"
                  }
                },
                "contents": [
                  {
                    "type": "image",
                    "url": "https://cdn-icons-png.flaticon.com/512/2921/2921147.png",
                    "aspectMode": "fit",
                    "size": "md"
                  },
                  {
                    "type": "text",
                    "text": "ลงทะเบียน",
                    "size": "sm",
                    "color": "#333333",
                    "align": "center",
                    "margin": "md",
                    "weight": "bold"
                  }
                ]
              },
              {
                "type": "box",
                "layout": "vertical",
                "flex": 1,
                "spacing": "sm",
                "paddingAll": "lg",
                "backgroundColor": "#FFFFFF",
                "cornerRadius": "md",
                "borderColor": "#E0E0E0",
                "borderWidth": "1px",
                "alignItems": "center",
                "justifyContent": "center",
                "action": {
                  "type": "uri",
                  "label": "ค้นหาวันนัด",
                  "uri": "https://telemedscheduler.vercel.app/",
                  "altUri": {
                    "desktop": "https://telemedscheduler.vercel.app/"
                  }
                },
                "contents": [
                  {
                    "type": "image",
                    "url": "https://cdn-icons-png.flaticon.com/512/1827/1827319.png",
                    "aspectMode": "fit",
                    "size": "md"
                  },
                  {
                    "type": "text",
                    "text": "ค้นหาวันนัด",
                    "size": "sm",
                    "color": "#333333",
                    "align": "center",
                    "margin": "md",
                    "weight": "bold"
                  }
                ]
              }
            ]
          }
        ]
      }
    ]
  },
  "footer": {
    "type": "box",
    "layout": "vertical",
    "contents": [
      {
        "type": "separator"
      },
      {
        "type": "button",
        "action": {
          "type": "message",
          "label": "ดูข้อมูลเพิ่มเติม",
          "text": "ข้อมูลเพิ่มเติมเกี่ยวกับtelemedicine"
        },
        "style": "link",
        "color": "#2B6CB0",
        "height": "sm",
        "margin": "sm"
      }
    ]
  }
}
```
## Notes

Built using the LINE Messaging API free tier with 11+ custom Flex Message designs for healthcare communication workflows.
