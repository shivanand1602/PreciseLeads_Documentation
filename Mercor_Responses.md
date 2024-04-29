# Positive_Replies of Mercor(Client)

## Overview
The SmartLead Positive Response extension is designed to fetch positive responses from leads managed through SmartLead.ai and store detailed information in an Airtable database.

Positive responses include categories such as "Interested," "Meeting Request," and "Information Request."

## Installation and Setup
1. **Clone Repository:**
   ```bash
   git clone https://github.com/your-username/smartlead-positive-response.git

## install dependencies
npm install

## Configuration:
1. Replace API_KEY with your actual Airtable API key.
   
2. Ensure the base.getTable method is correctly configured to fetch and update records in your Airtable database.

3.Set up the necessary Airtable fields like "Lead ID," "Merged Reply Bodies," "Lead Name," "Lead Email," "Lead Category," "Sequence Number," "Sent Time," and "Reply Time."

## input data
Ensure that your Airtable table "Mercor Response" contains the necessary fields for lead details.

## Output Data:
1. The extension fetches positive response leads from SmartLead.ai based on specific categories. For each positive response lead, it gathers the following information:
   
2. Lead ID: Unique identifier for the lead in SmartLead.ai.
   
3. Merged Reply Bodies: Merged email reply bodies of the lead.

4. Lead Name: Name of the lead.

5. Lead Email: Email address of the lead.

6. Lead Category: Category indicating the type of positive response ("Interested," "Meeting Request," "Information Request").

7. Sequence Number: Sequence number associated with the lead.

8. Sent Time: Time when the email was sent.

9. Reply Time: Time when the positive reply was received.

10. This information is then stored in your Airtable database.

## Code Overview
The provided code performs the following actions:

1. Fetches positive response leads' statistics from SmartLead.ai.
   
2. Filters leads based on positive response categories ("Interested," "Meeting Request," "Information Request").

3. Fetches lead details and email history from SmartLead.ai.

4. Extracts and merges email reply bodies into a single string for each lead.

5. Creates records in Airtable with the extracted lead information.

## Contributing
Contributions to enhance functionality, add features, or improve performance are welcome. Please follow the contribution guidelines in the repository.
