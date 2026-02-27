# 02 — n8n Automation Workflow

## How to Import
1. Open your n8n instance
2. Click Import from File
3. Select the .json file from this folder
4. Update all credentials in the nodes

## Workflow Overview
- Trigger: Webhook from AI agent
- Nodes: Lead processing > Scoring > CRM write > Calendar booking > Email trigger > Slack notification
- Error Handling: Fallback paths for failed API calls
