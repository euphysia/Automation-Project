# n8n Automation Projects

A collection of n8n workflows I built for real business use cases: HR operations, recruitment, AI chatbots, document processing and IT risk. Many of them use AI agents with tools and memory, LLMs (OpenAI, Google Gemini, Mistral) and Google Workspace integrations.

Each workflow is an exported `.json` file. To try one, open n8n, choose **Import from File**, select the JSON file, and add your own credentials.

## HR Automation

| Workflow | What it does |
|---|---|
| Recruitment and hiring | AI agent reads CVs from Google Drive, screens candidates, and schedules interviews and sends emails through Google Calendar and Gmail tools |
| Recruitment and hiring (Passed Interview) | Generates offer letters from a Google Docs template, emails them to successful candidates and sends rejection emails to the rest |
| Onboarding | Once a candidate confirms, notifies the department manager and IT, and emails the new hire the documents they need |
| Offboarding | Detects inactive employees, checks that company assets are returned and sends offboarding emails |
| Leave Management | Checks annual and medical leave balances, approves or rejects requests and updates balances in Google Sheets |
| Payroll | Monthly run that pulls overtime hours, calculates gross and net pay and generates payslips |
| Performance Review Scheduling | Schedules review cycles and emails reminders to employees and managers |
| Performance Review Checking | Checks review completion on a schedule and follows up on pending reviews |
| Generate Employment Verification Letter | Creates verification letters from a Google Docs template, saves them to Drive and emails them |
| Employee Self Service Chatbot | AI chatbot with memory that answers HR questions using Google Sheets and Docs as its knowledge base |
| Anonymous Employee Feedback | Collects anonymous feedback, runs sentiment analysis with OpenAI and emails HR a weekly digest |
| General Notifications & Employee Engagement | AI agent that sends scheduled announcements and engagement messages using Calendar, Sheets and Gmail |
| Email List Cleaning | Cleans and verifies email lists in Google Sheets using the Hunter API |

## Headhunter

| Workflow | What it does |
|---|---|
| Generate ICP Based on JD and Transcript | AI agent builds an Ideal Candidate Profile from a job description and a client call transcript, saved to Google Docs |
| Generate Sample Candidate Profile Based on ICP | Produces sample candidate profiles from the ICP to guide sourcing |
| Long Listing Scoring | Scores candidate CVs against the ICP using an LLM with structured output and ranks them in Google Sheets |

## Chatbots

| Workflow | What it does |
|---|---|
| Database Query AI Chatbot | WhatsApp AI chatbot that answers questions by querying data in Google Sheets |
| Telegram Scheduling Bot | Telegram bot that creates and manages Google Calendar events through natural language |

## Risk and IT

| Workflow | What it does |
|---|---|
| Phishing Email/URL Detection | Watches Gmail, checks links with VirusTotal, has an AI assistant assess the email and labels suspicious messages |
| Weekly Risk Summary Automation | AI agent summarises the week's risks from a Google Sheets risk register and emails the summary |

## Document AI and Other

| Workflow | What it does |
|---|---|
| OCR Workflow | Extracts structured data from uploaded documents with Google Gemini, logs it to Google Sheets and emails the results |
| Convert Schedule Image to Google Calendar | Reads a schedule image with Mistral OCR and OpenAI, then creates the matching Google Calendar events |
| Generate Company Preview Image | Batch-generates company preview images from spreadsheet data and saves them to Google Drive |

## Tools used

n8n · OpenAI · Google Gemini · Mistral AI · Google Workspace (Sheets, Drive, Docs, Calendar, Gmail) · WhatsApp · Telegram · VirusTotal · Hunter · JavaScript
