# 04 — Google Calendar Integration

## How It Works
1. n8n receives a Hot lead from the AI agent
2. Checks Google Calendar for next available slot
3. Creates event with lead details
4. Sends confirmation to lead and sales team

## Setup Notes
- Enable Google Calendar API in Google Cloud Console
- Add OAuth credentials to n8n (never commit credentials to repo)
