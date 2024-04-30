# SmartLead Reply Classification Automation

## Overview
This project automates the classification of lead email replies into different categories using Make platform, SmartLead.ai and OpenAI, and then performs actions based on the classification. 

The workflow involves webhook integration, natural language processing (NLP) classification, and data management in Google Sheets and Airtable.

## Workflow
1. **Webhook Setup:**
   - Set up a webhook on the SmartLead.ai platform to receive lead email replies.
   - Configure the webhook to send data to the automation system (Make platform).

2. **Data Retrieval:**
   - Upon receiving a lead email reply, the webhook triggers the automation system.

3. **NLP Classification - Out-of-Office:**
   - Pass the email content through OpenAI to classify it as an "Out-of-Office" message or not.
   - If classified as "Out-of-Office":
     - Update lead details in a Google Sheet for tracking.

4. **NLP Classification - Positive/Negative Response:**
   - If the email is not classified as "Out-of-Office," pass it through OpenAI again to determine if it's a positive response (e.g., Information Request, Meeting Request) or a negative response (e.g., Not Interested).
   - If positive:
     - Send a Slack message to a designated channel with lead data for follow-up.

5. **Data Management - Airtable:**
   - Update the lead details in an Airtable database table, including information such as lead name, email, response category, and any other relevant details.

## Technologies and Tools Used
- SmartLead.ai: Provides lead email replies through webhook integration.
- OpenAI: Utilized for natural language processing (NLP) classification.
- Google Sheets: Used for temporary storage of lead details in the Out-of-Office category.
- Slack: Sends notifications to designated channels for positive response leads.
- Airtable: Manages the lead database with detailed information and categories.
- Make: Provides the modules for custom webhook,OpenAi, Google Sheet,Slack,Airtable,etc.

## Getting Started
1. Clone this repository to your local machine.
2. Set up the required credentials and configurations for SmartLead.ai, OpenAI, Google Sheets, Slack, and Airtable.
3. Configure the webhook endpoint in SmartLead.ai to point to your automation system.
4. Run the automation system on your preferred server or environment.

## Contribution Guidelines
Contributions to enhance classification accuracy, add more response categories, or improve overall workflow efficiency are welcome. Follow the contribution guidelines provided in the repository.

## Support
For any issues or questions, feel free to [open an issue](https://github.com/your-username/smartlead-reply-automation/issues) on GitHub.

## License
This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
