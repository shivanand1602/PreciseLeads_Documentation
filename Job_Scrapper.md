markdown
# Job Scrapper Extension

The Job Scrapper extension is a Node.js script designed to retrieve and store job details from various sources using the Apollo and SourceStack APIs. It automates the process of fetching job openings of organizations and populating an Airtable database with comprehensive job details.

## Features
- **Apollo Integration:** Utilizes the Apollo API (api.apollo.io) to enrich organization data and fetch job postings.
- **SourceStack Integration:** Fetches additional job details using the SourceStack API (sourcestack-api.com).
- **Airtable Integration:** Stores job details in an Airtable database table named 'Jobs_Scrapper'.

## Usage
To use the Job Scrapper extension:

1. Obtain your API keys for Apollo (`apiKey`) and SourceStack (`apiss`).
2. Set up a table named 'Jobs_Scrapper' in your Airtable workspace with the following fields:
   - **Domain** (Text): Organization's domain name.
   - **Job Details** (Long Text): Stores job details fetched from the Apollo API.
   - **Job Details2** (Long Text): Stores job details fetched from the SourceStack API.
3. Clone the repository containing the extension script (`job_scrapper.js`) to your local machine.
4. Install Node.js and any required dependencies.
5. Configure the script by replacing the placeholder API keys (`apiKey` and `apiss`) with your actual API keys.
6. Run the script using Node.js:

bash
node job_scrapper.js


The script will iterate through records in the 'Jobs_Scrapper' table, fetch job details, and update the corresponding records with job information.

## Code Explanation
The code snippet provided in the README corresponds to the main functionality of the Job Scrapper extension:

- **Apollo API Integration:** Fetches organization details using the Apollo API based on the provided domain name. Retrieves job postings associated with the organization and updates the 'Job Details' field in Airtable with job titles and URLs.
- **SourceStack API Integration:** Fetches additional job details from SourceStack using the organization's domain. Updates the 'Job Details2' field in Airtable with job names, company names, and post URLs.
- **Error Handling:** Includes error handling to manage API response statuses, JSON parsing errors, and network issues.

## Troubleshooting
If you encounter any issues while using the extension, consider the following troubleshooting steps:

- Verify that your API keys (`apiKey` and `apiss`) are correctly configured in the script.
- Ensure that the Airtable table fields ('Domain', 'Job Details', 'Job Details2') match the expected data structure for successful updates.
- Check for console logs or error messages generated during script execution to identify potential issues.
- Review the Apollo and SourceStack API documentation for any changes or updates that may affect the script's functionality.

## Contributing
Contributions to the Job Scrapper extension are welcome! If you have feature requests, bug fixes, or improvements to suggest, please follow the contribution guidelines outlined in the repository.

This README provides a comprehensive guide on using, understanding, troubleshooting, and contributing to the Job Scrapper extension. Let me know if you need further adjustments or additional information!
