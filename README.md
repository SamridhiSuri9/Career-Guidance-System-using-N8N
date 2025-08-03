## 📚 Automated Career Guidance System
This project implements an end-to-end, multi-workflow automation using n8n to collect student interests from Google Sheets, validate and store the data, and then generate personalized career guidance emails with OpenAI-powered AI agents.

### 🚀 Features
✅ Google Sheets Trigger: Watches for new form submissions.
✅ Data Validation: Ensures inputs are complete and clean.
✅ Data Storage: Appends validated data into a Google Sheet for record-keeping.
✅ AI-Generated Guidance: Executes a secondary workflow with an OpenAI Chat Model to generate personalized advice.
✅ Draft Email Creation: Prepares an email draft in Gmail, ready for review and sending.

### 📂 Workflow Breakdown
#### Main Workflow
1. Google Sheets Trigger: Detects new form responses (e.g., student interests).
2. Validate Form Data: Checks inputs for missing or invalid fields.
3. Store to Google Sheet: Saves cleaned data.
4. Prepare Response: Formats a summary or confirmation message.
5. Execute Workflow: Calls the secondary workflow to generate guidance.

#### Secondary Workflow
1. When Executed by Another Workflow: Triggered by the main workflow.
2. Read New Entries: Pulls data from the Google Sheet.
3. AI Agent + OpenAI Chat Model: Crafts personalized career guidance.
4. Create a Draft: Composes a draft email in Gmail.

### 🛠 Requirements
n8n self-hosted or cloud instance.
Google Sheets API credentials.
Gmail API credentials.
OpenAI API key (for the AI agent).

### ⚙️ Setup Instructions
1. Import Workflows: Import both the main and secondary workflows into n8n.
2. Set Up Google Sheets Trigger: Connect your Google Sheets account and specify the sheet receiving form data.
3. Configure OpenAI Agent: Insert your OpenAI API key and choose your preferred chat model.
4. Connect Gmail: Authenticate with Gmail to enable draft creation.

