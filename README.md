# 🔗 Productboard Opportunity Sender – ChatGPT Plugin

This ChatGPT Plugin allows users to send customer feedback opportunities directly to Productboard via a Zapier webhook. It is designed to structure user input into a Productboard-compatible format and forward it automatically.

## ✨ Features

- Define and send structured **opportunity statements**
- Automatically include parent opportunities (if applicable)
- Uses **Zapier Webhooks** to push data into Productboard
- OpenAPI-powered for AI-friendly integration
- No authentication required

## 📦 Hosted Files

This plugin is defined by the following files:

| File                                | Description                            |
|-------------------------------------|----------------------------------------|
| `.well-known/ai-plugin.json`        | Plugin manifest                        |
| `.well-known/openapi.yaml`          | OpenAPI spec for plugin interaction    |
| `logo.png`                          | Plugin icon displayed in ChatGPT UI    |

## 🌐 GitHub Pages Hosting

The plugin is hosted via GitHub Pages:

https://hlcmn.github.io/productboard-action/.well-known/ai-plugin.json


> ⚠️ Ensure that GitHub Pages is enabled for the **main branch** and set to the **root** directory in your repo's settings.

## 🧪 Usage

Once installed in ChatGPT (GPT-4, Plugins mode):

```text
"Send the following opportunity to Productboard: Users are frustrated that they can’t quickly access key actions like export. Call it ‘Quick action access issues’. The parent is ‘Easier navigation for frequent tasks’.”

ChatGPT will format the opportunity and send it to your Zapier webhook:
https://hooks.zapier.com/hooks/catch/4816676/2cjxmcl/

🔧 Plugin Setup
This plugin uses no authentication and relies on a simple schema:

Example JSON Payload
json
Kopieren
Bearbeiten
{
  "name": "Quick action access issues",
  "description": "Users struggle to quickly access key functions like exporting or switching views.",
  "type": "subfeature",
  "parent": {
    "name": "Easier navigation for frequent tasks",
    "type": "feature"
  }
}
🛟 Contact
For questions or support, contact: 
