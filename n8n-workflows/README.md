# N8N-workflows Notes

---

## Table of Contents
1. [Introduction](#introduction)
2. [Key Features](#key-features)
3. [Getting Started](#getting-started)
4. [Example Workflows](#example-workflows)
5. [Integrations](#integrations)
6. [Best Practices](#best-practices)
7. [Self-Hosting](#self-hosting)
8. [Security](#security)
9. [Further Reading](#further-reading)

---

## Introduction
- n8n is an open-source workflow automation tool that lets you connect apps, APIs, and services to automate tasks without writing code. 
- It is highly extensible and can be self-hosted.
- We can setup n8n using npm, Docker, or through cloud providers.
- n8n supports over 350 integrations and allows for custom node creation.
- It features a visual workflow editor that supports drag-and-drop functionality, making it easy to create and manage workflows.
- n8n is designed for both technical and non-technical users, enabling them to automate complex tasks with ease.

---

## Key Features
- Drag-and-drop workflow builder
- Trigger-Based Automation (Webhooks, Cron jobs, Manual triggers)
- Data Transformation (modify, map, and combine data between services)
- Supports conditional branching and looping.
- 350+ built-in integrations
- Custom node creation
- Self-hostable and scalable
- Error Handling and Logging (Catch errors in workflows using Error Triggers).
- Secure Credential Management 


## Usages
- CRM and email automation
- Data synchronization between services
- E-commerce order processing
- Social media cross-posting
- API-to-API integrations
- Scheduled tasks and cron jobs
- Custom notifications and alerts
- Event-driven workflows (e.g., new user sign-up, form submissions)
- Automated reporting and dashboards

---

## Getting Started
1. Install n8n (npm, Docker, or cloud)
2. Launch the n8n editor UI
3. Create a new workflow
4. Add trigger and action nodes
5. Deploy and monitor your workflow

---

## Example Workflows
- Data syncing between Google Sheets and Airtable
- Automated email notifications
- Social media posting automation
- API to API data synchronization

### Example: Email to Slack
1. Trigger: New email received
2. Action: Extract content
3. Action: Send message to Slack

---

## Integrations
- Google Products (Sheets, Drive, Calendar)
- Microsoft Products (Excel, Outlook)
- Social Media (Twitter, Facebook, Instagram)
- Project Management (Trello, Asana, Jira)
- Communication Tools (Slack, Discord, Microsoft Teams)
- Payment Processors (Stripe, PayPal)
- Marketing Tools (Mailchimp, SendGrid)
- Cloud Services (AWS, Google Cloud, Azure)
- IoT Devices (MQTT, Webhooks)
- Custom APIs (HTTP Request node)
- File Storage (Dropbox, Google Drive, S3)
- Webhooks for real-time data processing
- Email Services (Gmail, Outlook)
- Web Scraping (using HTTP Request and HTML Extract nodes)
- GitHub
- Databases (MySQL, PostgreSQL, MongoDB)

---

## Best Practices
- Secure Your Instance. Use HTTPS in production.
- Use environment variables for secrets
- Keep credentials, URLs, and configuration settings in env files (.env).
- Modularize workflows for reuse
- Set Up Error Handling. Use Error Trigger or Try/Catch logic with IF nodes.
- Use version control for workflow JSON
- Optimize Loops and Pagination. Use SplitInBatches node when processing large datasets.

---

## Self-Hosting
- Deploy with Docker for scalability
- Use HTTPS for secure access
- Set up backups and monitoring

---

## Security
- Store credentials securely
- Limit access to trusted users
- Regularly update n8n and dependencies

---

## Further Reading
- [n8n Docs](https://docs.n8n.io/)
- [n8n Workflows](https://n8n.io/workflows/)
- [n8n GitHub](https://github.com/n8n-io/n8n)

---


## Setup N8N:

1. Install Node LTS Version
- sudo apt install curl gnupg -y
- curl -fsSL https://deb.nodesource.com/setup_22.x | sudo -E bash -
- sudo apt install nodejs -y
- node -v
- npm -v

2. Install N8N
- sudo npm install n8n -g

3. Start n8n through command line
- n8n

4. Access n8n Editor UI
- http://localhost:5678
- http://192.168.1.135:5678

5. Installed Directory:
- /home/c2mtest/.n8n

6. Generate .env varaibles
- create .env file in /home/c2mtest/.n8n and add the following lines
    - N8N_SECURE_COOKIE=false
    - N8N_PROTOCOL=http
7. After adding the above lines, run the below command
- export $(cat ~/.n8n/.env | xargs)

8. After that again run in terminal
- n8n