# Setup Guide

## Prerequisites
- n8n instance (self-hosted or cloud)
- Airtable or Google Sheets
- Google Cloud account (Calendar API)
- Zapier account
- Voiceflow / Chatbase / ManyChat account
- Slack workspace

## Step-by-Step Setup

### 1. Set up the AI Agent
- Create agent in Voiceflow or Chatbase
- Configure qualifying questions and scoring
- Set webhook URL to your n8n instance

### 2. Import n8n Workflow
- Import 02_n8n_Workflow/growthpath_workflow.json
- Add credentials for each service

### 3. Configure the CRM
- Set up Airtable base using schema in 03_CRM_Database
- Copy your Airtable API key and base ID

### 4. Set up Google Calendar
- Enable Calendar API in Google Cloud
- Create OAuth credentials and add to n8n

### 5. Set up Zapier Email Campaign
- Follow 05_Email_Campaign/zapier_workflow_setup.md
- Customize emails with GrowthPath branding

### 6. Test End-to-End
- Simulate a lead conversation
- Verify data appears in CRM
- Confirm calendar event is created
- Check emails triggered in Zapier
- Confirm Slack notification received
