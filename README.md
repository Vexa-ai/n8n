# Vexa n8n Integration Examples

This repository contains ready-to-use n8n workflows for integrating with Vexa API to add AI-powered transcription and translation bots to your Google Meet meetings.

## What is Vexa?

Vexa is an AI-powered platform that provides real-time transcription and translation services for video meetings. It supports multiple platforms including Google Meet, Zoom, and Microsoft Teams.

## Features

- Send AI transcription bots to Google Meet meetings
- Get real-time transcription during meetings
- Get meeting transcripts after meetings
- Support for multiple languages
- Real-time translation capabilities

## Available Workflows

### Google Meet Integration

The `google_meet_with_vexa.json` workflow contains ready-to-use blocks for:

1. **Send bot to meeting**
   - Adds a transcription bot to your Google Meet
   - Supports multiple languages
   - Real-time transcription

2. **Get meeting transcripts**
   - Retrieve real-time transcription during meetings
   - Get complete transcripts after meetings

3. **Bot Management**
   - Check bot status
   - Update bot configuration
   - Stop bot
   - List all meetings

## How to Use

### Getting Your API Key

There are two ways to get your Vexa API key:

1. **From Vexa Website**
   - Visit [Vexa Dashboard](https://vexa.ai/dashboard/api-keys)
   - Sign up for a new account or log in
   - Navigate to the API Keys section
   - Click "Create New API Key"
   - Copy your API key and keep it secure

2. **From Reddit Community**
   - Join the [Vexa Reddit Community](https://www.reddit.com/r/vexa/)
   - Look for the pinned post about API access
   - Follow the instructions to request an API key
   - The community moderators will provide you with access

> **Note**: The API key is sensitive information. Never share it publicly or commit it to version control.

### Importing and Using the Workflow

1. **Import the workflow**
   - Import `google_meet_with_vexa.json` into your n8n instance
   - The workflow contains independent blocks that you can copy and use

2. **Configure the blocks**
   - Replace the hardcoded API key with your own
   - Replace the meeting IDs with your Google Meet IDs
   - Each block is self-contained and can be used independently

## Example: Sending a Bot to a Meeting

1. Start a Google Meet:
   - Go to [meet.new](https://meet.new)
   - Or use your existing meeting

2. Get the meeting ID:
   - From URL: meet.google.com/xxx-xxxx-xxx
   - Example: meet.google.com/mpu-dqtj-jcm
   - The last part is your meeting ID

3. Use the "Send bot to meeting" block:
   - Replace the API key
   - Replace the meeting ID
   - The bot will join your meeting and start transcribing

## API Endpoints

The workflow includes examples for all Vexa API endpoints:

- `POST /bots` - Send bot to meeting
- `GET /transcripts/{platform}/{meeting_id}` - Get transcripts
- `GET /bots/status` - Check bot status
- `PUT /bots/{platform}/{meeting_id}/config` - Update bot config
- `DELETE /bots/{platform}/{meeting_id}` - Stop bot
- `GET /meetings` - List all meetings

## Support

For more information about Vexa API:
- Check [Vexa GitHub](https://github.com/Vexa-ai/vexa)
- Join the [Vexa Discord n8n Community](https://discord.gg/kMXTD2Maw7) for community support
- Contact Vexa support for API-related questions

## License

This project is licensed under the MIT License - see the LICENSE file for details. 