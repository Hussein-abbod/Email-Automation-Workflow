# AI Email Automation Workflow (n8n)

This project contains an n8n workflow that uses an AI Agent (powered by Groq) to manage emails via Telegram. You can ask the AI to read your latest emails or send new ones using 

## 🚀 Features
- **AI Agent**: Uses `llama-3.3-70b-versatile` on Groq for intelligent tool selection.
- **Telegram Integration**: Trigger and control the automation directly from your phone.
- **Gmail Tools**: Ability to read emails and send emails through Google's APIs.

## 🛠️ Setup Instructions

### 1. Prerequisites
- An [n8n](https://n8n.io/) instance (self-hosted or cloud).
- A [Telegram Bot](https://t.me/botfather) token.
- A [Groq API Key](https://console.groq.com/).
- A Google Cloud Project with the Gmail API enabled (for OAuth2).

### 2. Import the Workflow
1. Download `workflow_template.json`.
2. Open your n8n instance.
3. Go to **Workflows** > **Import from File**.
4. Select the downloaded JSON.

### 3. Configure Credentials
You will need to set up/assign credentials for:
- **Telegram API**: Connect your bot token.
- **Groq API**: Add your Groq API key.
- **Gmail OAuth2 API**: Configure your Google Client ID and Secret.

### 4. Security
Remember to replace the following placeholders in the imported workflow:
- `YOUR_TELEGRAM_CHAT_ID`: Your personal Telegram ID (to ensure only you can control the bot).
- `YOUR_WEBHOOK_ID`: n8n will typically regenerate these upon import.

## 📄 License
MIT
