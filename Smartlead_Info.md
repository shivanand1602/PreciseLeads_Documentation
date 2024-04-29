# Smartlead_Info Extension

The Smartlead_Info extension is a Node.js script designed to interact with the smartlead.ai API and Airtable database. It fetches campaign details from smartlead.ai and populates the "Campaigns" table in Airtable with comprehensive information about each campaign.

## Overview

The extension utilizes the smartlead.ai API key (`API_KEY`) to access campaign data. It performs the following key functions:

- **Fetch Campaign Details:** The script sends a GET request to `https://server.smartlead.ai/api/v1/campaigns` with the API key appended as a query parameter. It retrieves information such as campaign name, ID, user ID, and status.
- **Store Campaigns in Airtable:** After successfully fetching campaign data, the extension creates new records in the Airtable "Campaigns" table. It maps the fetched attributes to corresponding fields in Airtable, such as "Campaign Name," "Campaign Id," "User_Id," and "Campaign Status."
- **Additional Analytics:** For each campaign, the extension makes a secondary API call to fetch more detailed analytics from `https://server.smartlead.ai/api/v1/campaigns/{campaign_id}/analytics`. It gathers data such as lead counts, email statistics (sent, opened, clicked), and client information (name, email, company name).

## Usage

To use the Smartlead_Info extension:

1. Obtain your API key from smartlead.ai and ensure it has permissions to access campaign and analytics data.
2. Set up a table named "Campaigns" in your Airtable workspace with the specified fields (as mentioned in the README).
3. Clone the repository containing the extension script (`smartlead_info.js`) to your local machine.
4. Install Node.js and any required dependencies.
5. Configure the script by replacing `API_KEY` with your actual smartlead.ai API key and updating any other necessary parameters.
6. Run the script using Node.js:
   ```bash
   node smartlead_info.js
## Code Explanation
The code snippet provided in the README corresponds to the main functionality of the extension. It initiates API requests to fetch campaign details and update Airtable records accordingly.

## Troubleshooting
If you encounter any issues while using the extension, consider the following steps for troubleshooting:

Verify that your smartlead.ai API key (API_KEY) is correctly configured in the script.
Ensure that the Airtable "Campaigns" table fields match the expected data structure for successful record creation and updates.
Check for any console logs or error messages generated during script execution to identify potential issues.
Review the smartlead.ai API documentation for any changes or updates that may affect the script's functionality.
Contributing
Contributions to the Smartlead_Info extension are encouraged! If you have feature requests, bug fixes, or improvements to suggest, please follow the contribution guidelines outlined in the repository.

## License
This extension is licensed under the MIT License. See the LICENSE file for more details.
