# Customer Feedback Automation

An AI-powered automation built with n8n that classifies customer feedback by sentiment, logs it to Airtable, and alerts management via email for negative feedback.

## How It Works

1. A customer submits feedback via a Fillout form (name, email, feedback text)
2. AI classifies the feedback as **positive**, **negative**, or **neutral**
3. A keyword-based fallback layer double-checks the sentiment for extra reliability
4. The feedback and its classification are logged to Airtable
5. If the feedback is **negative**, an HTML email alert is sent to management with the customer's details and feedback

## Tech Stack

- **n8n** – workflow automation
- **OpenAI** – sentiment classification
- **Airtable** – feedback database
- **Fillout** – feedback forms intake
- **Gmail** – management alerts

## Setup

1. Import `workflow.json` into your n8n instance
2. Connect your own credentials for: Fillout, Airtable, OpenAI, and Gmail
3. Update the Airtable base/table IDs to match your own base
4. Update the recipient email address in the "Send a message" node
5. Activate the workflow

## Note

This is a demo/portfolio version. Sensitive data (API keys, real customer data) has been removed.

## Author

Built by Emmanuel Obidigbo — Pharmacist & AI Automation Specialist
