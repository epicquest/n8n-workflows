EQS Google Meet Assistant (n8n Workflow)

This repository contains an n8n workflow that acts as a smart assistant for Google Meet sessions.
It validates user input, provisions an AI meeting bot, listens for stop commands inside the transcript, and delivers meeting notes via email.

🚀 What it does:

Provides a form-based trigger where users can submit:

Google Meet URL

Participant emails

Admin email

Runs input validation (Google Meet link format, emails, etc.)

Automatically creates an AI assistant bot inside the Google Meet (via Vexa API).

Periodically fetches the meeting transcript.

Detects stop commands (like “stop ai assistant”) from meeting chat or transcript.

Sends out meeting notes and transcripts via email to all participants.

Supports bot cleanup with a second form to remove the assistant from a meeting.

⚡ Why it’s useful:

Saves time by automating bot setup and transcript handling.

Ensures clean, validated inputs before starting.

Lets admins stop the bot from inside the meeting with natural commands.

Provides a repeatable, shareable automation template for anyone using n8n + Google Meet.

📦 Tech stack:

n8n
 (workflow automation)

Vexa AI Cloud API (bot + transcripts)

Custom JavaScript code for validation & transcript processing

Email integration for notifications & meeting summaries

🛠 How to use:

Import the workflow JSON file into your n8n instance.

Configure your credentials (Vexa API, SMTP, etc.).

Run the workflow and test it with the provided form.

Extend/customize it for your own Google Meet automation needs.
