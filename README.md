📅 Calendar Schedule Automation (n8n)

This workflow automatically fetches upcoming events from Google Calendar and sends you a daily email summary of your schedule using Gmail.

🚀 Workflow Overview

Schedule Trigger – Starts automatically at a set time every day (default: 7 AM IST).

Get Events – Fetches all Google Calendar events within the next 8 hours.

Edit Fields – Formats each event as HH:mm -- Event Title.

Aggregate – Combines all events into one list.

Format – Prepares the final output message.

Send Email – Sends the daily schedule to your Gmail inbox with the subject:

Meets Schedule for {Day} {Date}

📝 Example Output

Email Subject:

Meets Schedule for Monday 2025-09-18


Email Body:

09:00 -- Team Standup
11:00 -- Client Call
15:00 -- Project Review

⚙️ Setup Instructions

Import the file Calendar schedule.json into your n8n instance.

Configure the following credentials in n8n:

Google Calendar API (to fetch events)

Gmail API (to send emails)

Adjust the trigger time in the Schedule Trigger node if you want a different daily reminder time.

Activate the workflow.

📂 Files in This Repo

Calendar schedule.json → Workflow definition.

Calendar schedule.jpg → Visual diagram of the workflow.

🔑 Requirements

n8n (cloud or self-hosted)

Google Calendar account

Gmail account
