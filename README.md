# AI-Based SSH Brute-Force Detection and Telegram Alert System

## Overview
This project uses n8n automation, JavaScript, a Groq-powered AI Agent, and Telegram to analyze SSH login logs and identify potentially suspicious authentication activity.

## Objectives
- Process SSH login log entries.
- Extract source IP addresses, usernames, and failed login counts.
- Use AI to classify potentially suspicious activity.
- Generate security recommendations and evidence.
- Send security notifications through Telegram.

## Workflow
1. **Start SSH Detection** – Starts the workflow manually.
2. **Generate Sample SSH Logs** – Generates sample SSH authentication events.
3. **Prepare SSH Log Data** – Prepares log data for parsing.
4. **Extract SSH Login Details** – Extracts useful fields from raw logs.
5. **AI-Based Threat Classification** – Uses a Groq Chat Model to analyze the extracted evidence.
6. **Save Security Audit Record** – Handles the analysis result for auditing.
7. **Send Telegram Security Alert** – Sends a notification to the configured Telegram chat.

## Technologies Used
- n8n
- JavaScript
- Groq Chat Model
- AI Agent
- Telegram Bot

## Current Implementation
The current prototype uses simulated SSH logs for testing. It does not automatically collect logs from a live SSH server or block IP addresses.

## Future Enhancements
- Integrate with real Linux SSH authentication logs.
- Add continuous monitoring.
- Store audit records in a persistent database.
- Improve detection and incident reporting.

## Security Notice
Configure API credentials and Telegram bot credentials privately in n8n. Never publish API keys, bot tokens, passwords, or other secrets in this repository.

## Author
Cybersecurity Student
