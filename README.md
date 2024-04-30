# Automation Toolkit README

This repository contains a collection of powerful automation tools and extensions designed to streamline various tasks related to lead management, email enrichment, response classification, job scraping, company categorization, and more. Each tool is described below along with setup instructions, usage guidelines, and customization options.

## 1. Waterfall Enrichment

The Waterfall Enrichment extension is designed to enrich lead emails by utilizing multiple tools such as LeadMagic, UseArtemis, Tomba, and BounceBan. It follows a waterfall approach where if one tool fails to find the email, the next tool in line is used until the email is successfully retrieved. The retrieved email is then validated using BounceBan to determine its validity.

### Workflow
1. Input Data: Receive input data such as lead's first name, last name, and company domain.
2. Tool Selection: Try LeadMagic API first to find the email based on the provided information. If unsuccessful, switch to UseArtemis and then Tomba.
3. Email Validation: Validate retrieved emails using BounceBan API to determine deliverability and validity.

### Setup Instructions
- Clone the repository and install dependencies.
- Configure API keys for LeadMagic, UseArtemis, Tomba, and BounceBan.
- Set up Airtable fields for lead data and email validation status.

## 2. SmartLead Email Account Warmup

The SmartLead Email Account Warmup extension automates updating specific email accounts and adds them to the warmup process in SmartLead.ai for improved email deliverability.

### Tools Used
- SmartLead.ai Platform
- Airtable Database
- JavaScript
- REST API

### Installation and Setup
- Clone the repository and install dependencies.
- Replace sd with your actual SmartLead API key.
- Configure Airtable fields for email account details and warmup status.

## 3. SmartLead Reply Classification Automation

This project automates lead email reply classification using SmartLead.ai and OpenAI, categorizing replies into Out-of-Office, Positive Response, or Negative Response categories. It then performs actions based on the classification.

### Workflow
1. Webhook Setup: Configure a webhook on SmartLead.ai to receive lead email replies.
2. NLP Classification: Classify emails using OpenAI into categories.
3. Data Management: Update Google Sheets and Airtable based on classification.

### Technologies Used
- SmartLead.ai
- OpenAI
- Google Sheets
- Airtable
- JavaScript
- Webhook Integration

## 4. Positive Replies of Mercor (Client)

The SmartLead Positive Response extension fetches positive responses from leads managed through SmartLead.ai and stores detailed information in an Airtable database.

### Tools Used
- SmartLead.ai
- Airtable
- JavaScript
- REST API

### Installation and Setup
- Clone the repository and install dependencies.
- Configure Airtable API key and fields for lead data.

## 5. LinkedIn Fetcher (Proxycurl)

The Proxycurl Lead Fetcher fetches detailed information about leads using the Proxycurl API and displays the results in an Airtable database.

### Tools Used
- Proxycurl API
- Airtable
- JavaScript
- REST API

### Installation and Setup
- Clone the repository and install dependencies.
- Configure Proxycurl API key and Airtable fields.

## 6. Job Scrapper Extension

The Job Scrapper extension retrieves and stores job details from various sources using the Apollo and SourceStack APIs. It populates an Airtable database with comprehensive job information.

### Tools Used
- Apollo API
- SourceStack API
- Airtable
- JavaScript
- REST API

### Installation and Setup
- Clone the repository and install dependencies.
- Configure API keys and Airtable fields for job data.

## 7. Email Finder Extensions

These extensions fetch email addresses of leads using APIs like UseArtemis and Tomba and update the Airtable database with the retrieved information.

### Tools Used
- UseArtemis API
- Tomba API
- Airtable
- JavaScript
- REST API

### Installation and Setup
- Clone the repository and install dependencies.
- Configure API keys and Airtable fields.

## 8. Company Category Classifier

The Company Category Classifier uses OpenAI's GPT-3.5 model to classify companies into B2B or B2C categories based on company name and description.

### Tools Used
- OpenAI
- Airtable
- JavaScript
- REST API

### Installation and Setup
- Clone the repository and install dependencies.
- Configure OpenAI API key and Airtable fields.

## Conclusion

These automation tools provide a comprehensive solution for lead management, email enrichment, response classification, job scraping, company categorization, and more. They leverage powerful APIs, AI models, and database integrations to streamline workflows and improve efficiency in various business processes.

## 9. SmartLead to HubSpot Data Integration

The SmartLead to HubSpot Data Integration automates fetching lead details from Airtable and updating them on HubSpot using a POST request. It ensures synchronization between SmartLead and HubSpot for efficient lead management.

### Tools Used
- SmartLead.ai Platform
- Airtable Database
- JavaScript
- REST API

### Installation and Setup
- Clone the repository and install dependencies.
- Configure SmartLead API key, HubSpot API key, and Airtable fields.
- Set up lead data in Airtable for integration.

## 10. SmartLead Reply Classification Automation

The SmartLead Reply Classification Automation tool classifies lead email replies into different categories using Make platform, SmartLead.ai, and OpenAI. It then performs actions based on the classification, such as updating databases and sending notifications.

### Tools Used
- Make Platform
- SmartLead.ai
- OpenAI
- Google Sheets
- Slack
- Airtable
- JavaScript
- Webhooks

### Installation and Setup
- Configure webhooks on SmartLead.ai to trigger the automation.
- Set up Make modules for classification and actions.
- Update configurations for SmartLead API, OpenAI API, Slack integration, and Airtable.

## 11. B2B or B2C Classifier using OpenAI

The B2B or B2C Classifier extension leverages OpenAI's natural language processing (NLP) capabilities to classify companies into B2B or B2C categories based on company name and description.

### Tools Used
- OpenAI
- Airtable
- JavaScript
- REST API

### Installation and Setup
- Clone the repository and install dependencies.
- Configure OpenAI API key and Airtable fields.
- Provide company details in Airtable for classification.

## Conclusion

These automation tools provide a comprehensive solution for lead management, email enrichment, response classification, job scraping, company categorization, and more. They leverage powerful APIs, AI models, and database integrations to streamline workflows and improve efficiency in various business processes.

Contributions and customizations can be made to enhance functionality, add support for more APIs, or improve error handling as per specific business needs.
