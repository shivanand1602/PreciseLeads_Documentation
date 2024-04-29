# LinkedIn_Fetcher(Proxycurl)

The Proxycurl Lead Fetcher is a powerful tool designed to fetch detailed information about leads using the Proxycurl API and display the fetched results in an Airtable database. This tool is particularly useful for businesses and professionals seeking to enrich their lead data and streamline their processes.

## Installation

1. **Clone Repository:**
   ```bash
   git clone https://github.com/your-username/proxycurl-lead-fetcher.git

## Install dependencies
npm install

## Configuration::
Replace apiKey with your actual Proxycurl API key.
Update apiUrlBase with your Proxycurl API endpoint base URL.

## Code Explaination::

1. Retrieves records from the Airtable table named 'LinkedIn'.
2. Fetch LinkedIn Details:
3. Uses the Proxycurl API to fetch LinkedIn details based on the provided LinkedIn URL.
4. Updates the Airtable fields with the fetched LinkedIn data.
5. Data Transformation:
6. Formats and structures the fetched data to populate Airtable fields such as 'public_identifier', 'first_name', 'last_name', 'full_name', 'follower_count', 'occupation', 'headline', 'summary', 'country', 'city', 'state', 'Experience', 'Education', 'Languages', 'Certifications', 'Activities', 'Gender', 'Birth_Date', 'Industry', 'Interests', 'Personal_Emails', 'Personal_Numbers', and 'Skills'.

## Error Handling:
Handles API response errors and JSON parsing errors.
Logs error messages for debugging purposes.
## Contributing
Contributions to this project are welcome. Please follow the contribution guidelines in the repository.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
