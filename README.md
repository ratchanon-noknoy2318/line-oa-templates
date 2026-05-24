# 🚀 11+ LINE Flex Message Templates

<p align="left">
  Ready-to-use LINE Flex Message templates for healthcare automation.
</p>


## 📸 Preview Gallery
*Captured from [Flex simulator](https://developers.line.biz/flex-simulator/).*

| Telemedicine Start | Telemedicine More Info | About Us | Health Tip |
| :---: | :---: | :---: | :---: |
| <img src="https://res.cloudinary.com/dpa96jvla/image/upload/v1779581774/%E0%B8%94%E0%B8%B5%E0%B9%84%E0%B8%8B%E0%B8%99%E0%B9%8C%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B8%A2%E0%B8%B1%E0%B8%87%E0%B9%84%E0%B8%A1%E0%B9%88%E0%B9%84%E0%B8%94%E0%B9%89%E0%B8%95%E0%B8%B1%E0%B9%89%E0%B8%87%E0%B8%8A%E0%B8%B7%E0%B9%88%E0%B8%AD_h4iu7b.png" width="200"> | <img src="https://res.cloudinary.com/dpa96jvla/image/upload/v1779581739/11_rg53qf.png" width="200"> | <img src="https://res.cloudinary.com/dpa96jvla/image/upload/v1779581741/9_qzcm7o.png" width="200"> | <img src="https://res.cloudinary.com/dpa96jvla/image/upload/v1779581740/10_eclrzt.png" width="200"> |
| [JSON](./TelemedicineStartFlexmessage.json) | [JSON](./TelemedicineMoreInfoFlexmessage.json) | [JSON](./AboutUsFlexmessage.json) | [JSON](./HealthTipsFlexmessage.json) |

## ⚙️ Developer Integration
Directly load JSON files and pass the content to the LINE Messaging API SDK. Environment variables (.env) are used to securely store the LINE Channel Access Token and Channel Secret.<br>
**Node.js Example:**
```javascript
import { Client } from "@line/bot-sdk";
import flexMessage from "./TelemedicineStartFlexmessage.json" with { type: "json" };

const client = new Client({
  channelAccessToken: process.env.CHANNEL_ACCESS_TOKEN,
  channelSecret: process.env.CHANNEL_SECRET,
});

await client.pushMessage(USER_ID, flexMessage);
```



## 🔐 Security Notice

This project uses LINE Messaging API credentials to enable messaging functionality.

- The `CHANNEL_ACCESS_TOKEN` and `CHANNEL_SECRET` must be stored in environment variables only (`.env`)
- Never expose these values in frontend code or public repositories
- If credentials are leaked, immediately revoke and re-issue them from the LINE Developers Console
- Each environment (dev / staging / production) should use separate channel credentials

For security reasons:
- Do not commit `.env` files to version control
- Ensure `.gitignore` includes `.env*`

## 🧪 Environment Setup

Create a `.env.local` file in the root directory:

```env
CHANNEL_ACCESS_TOKEN=your_line_channel_access_token
CHANNEL_SECRET=your_line_channel_secret
