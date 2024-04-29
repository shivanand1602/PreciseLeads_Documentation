# SmartLead Email Account Warmup 

## Overview
The SmartLead Email Account Warmup extension automates the process of updating a specific email account of a client based on the provided ID and adds it to the warmup process in SmartLead.ai. 

This allows for efficient management and warmup of email accounts for better email deliverability.

## Tools Used-
1. Smartlead.ai Platform
2. Airtable Database

## Tech Stack Used-

1. JavaScript Languages
2. REST Api

## Installation and Setup
1. **Clone Repository:**
   ```bash
   git clone https://github.com/your-username/smartlead-email-warmup.git
   
## install Dependencies:
npm install

## Configuration:
1.Replace sd with your actual SmartLead API key.

2.Set up the necessary Airtable fields like "Name," "Email," "Password," "Domain," "smartLead_id," and "WarmupStatus" to store and manage email account details and warmup status.

## input Data:

1. Select a record from the "User Accounts" table in Airtable to update the corresponding email account.

2. Ensure that the selected record contains the required fields like "Name," "Email," "Password," and "Domain" for updating the email account.

## Output Data:
1. The extension sends a POST request to SmartLead.ai's API to update the email account details and add it to the warmup process.

2. It logs the response from the API and updates the Airtable record with the SmartLead email account ID and warmup status.

## Code Explanation
The provided code snippet performs the following actions:

1. Fetches a record from the "User Accounts" table in Airtable based on user input.

2. Constructs the necessary parameters for updating the email account using the SmartLead.ai API.

3. Sends a POST request to SmartLead.ai with the updated email account details.

4. Updates the Airtable record with the SmartLead email account ID and sets the warmup status to "Warmup started" upon successful addition to the warmup process.

## Contributing
Contributions to enhance functionality, improve error handling, or add new features are welcome. Please follow the contribution guidelines in the repository.
