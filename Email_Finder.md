# Email Finder Extensions

## Overview
This repository contains two extensions developed to fetch email addresses of leads using different APIs: UseArtemis and Tomba. 

These extensions automate the process of finding and updating email information for leads stored in an Airtable database.

## Tools Used
1. UseArtemis API
2. Tomba API
3. Airatable Database
4. JavaScript Language

## UseArtemis Extension
The UseArtemis extension utilizes the UseArtemis API to enrich lead information and retrieve email addresses based on provided first name, last name, and domain. Here's how to use it:

1. **Installation:**
   - Clone the repository and install dependencies.
   - Replace the `useApiKey` variable with your actual UseArtemis API key.

2. **Usage:**
   - Run the extension using Node.js.
   - It fetches records from the "Email Finder" table in Airtable.
   - For each record, it checks if essential information (website, first name, last name) is available and if the email is not already present.
   - If conditions are met, it makes a POST request to the UseArtemis API to find and update the email field in the Airtable record.

## Tomba Extension
The Tomba extension utilizes the Tomba API to find email addresses based on domain, first name, and last name. Follow these steps to use it:

1. **Installation:**
   - Clone the repository and install dependencies.
   - Replace the `tombaApiKey` and `tombaSecret` variables with your actual Tomba API credentials.

2. **Usage:**
   - Run the extension using Node.js.
   - It fetches records from the "Email Finder" table in Airtable.
   - For each record, it checks if essential information (website, first name, last name) is available and if the email is not already present.
   - It extracts the domain from the website URL, constructs the Tomba API URL, and makes a GET request to fetch email information.
   - Finally, it updates the email field in the Airtable record with the retrieved email address.

## Contributing
Contributions to enhance functionality, add support for more APIs, or improve error handling are welcome. Follow the contribution guidelines provided in the repository.

## Support
For any issues or questions, feel free to [open an issue](https://github.com/your-username/email-finder-extensions/issues) on GitHub.

## License
This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
