# B2B or B2C Classifier using OpenAI

## Overview
This extension automates the classification of companies into B2B (Business-to-Business) or B2C (Business-to-Consumer) categories using OpenAI's natural language processing (NLP) capabilities. It takes input parameters such as company name and description, then uses OpenAI's API to determine the appropriate classification.

## Workflow
1. **Data Retrieval:**
   - Fetch company data from an Airtable database, including company names and descriptions.

2. **NLP Classification:**
   - Pass company details through OpenAI's API for classification.
   - OpenAI determines if the company is B2B or B2C based on the provided information.

3. **Update Records:**
   - Update the Airtable records with the determined classification (B2B or B2C).

## Technologies Used
- Airtable: Stores company data and classification results.
- OpenAI API: Utilized for natural language processing (NLP) classification.
- JavaScript: Used for scripting the automation logic.
- Webhook (not explicitly mentioned in code): Can trigger the classification process based on events or schedules.

## Setup Instructions
1. Clone this repository to your local environment.
2. Set up an Airtable base with a table named 'b2b or b2c' and relevant columns ('company names', 'company description', 'b2b or b2c').
3. Obtain an API key from OpenAI and replace the placeholder in the code with your actual API key.
4. Configure the script to run on your preferred automation platform or server.
5. Ensure that the webhook or trigger mechanism is set up to execute the script based on your workflow requirements.

## Usage
1. Add company details (name and description) to the 'b2b or b2c' table in Airtable.
2. Run the script or trigger the webhook to initiate the classification process.
3. Check the 'b2b or b2c' column in Airtable to see the classification results.

## Customization
- You can modify the script to handle additional input parameters or customize the classification logic based on your specific business needs.
- Adjust the response handling to handle scenarios where OpenAI may not provide a clear classification.

## Contribution
Contributions to enhance classification accuracy, add new features, or improve the workflow are welcome. Fork this repository, make your changes, and submit a pull request following the contribution guidelines.

## Support
For any questions, issues, or support requests, please open an issue on GitHub or contact the project maintainers directly.

## License
This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
