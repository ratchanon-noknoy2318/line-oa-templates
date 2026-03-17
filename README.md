# LINE Hospital Integration

Integration service connecting a hospital system with a LINE Official Account to automate patient interactions.

The system uses the LINE Messaging API to handle patient requests, deliver automated responses, and provide access to hospital services through structured messaging interfaces.

---

## Problem

Hospital staff previously handled many patient requests manually through messaging channels, including:

- appointment inquiries
- telemedicine access
- hospital information requests

This created administrative overhead and slow response times.

---

## Solution

This project implements a webhook-based integration that:

- connects LINE Official Account to backend services
- handles incoming patient messages
- delivers structured responses using Flex Messages
- exposes hospital services through Rich Menu navigation

The system enables automated patient workflows and improves accessibility to hospital services.

---

## Architecture

```
Patient
↓
LINE Official Account
↓
Webhook (Node.js)
↓
Flex Message Response
```

---

## Tech Stack

- Node.js
- JavaScript
- LINE Messaging API
- Flex Messages (JSON)

---

## Project Structure

```
flex_message/   JSON templates for structured message responses
push_message/   outbound messaging and notification logic
richmenu/       configuration and assets for LINE Rich Menu
route.js        webhook entry point and request routing
```

---

## Features

- automated patient messaging workflows
- structured responses using Flex Messages
- service navigation via LINE Rich Menu
- webhook-based service integration

---

## License

MIT
