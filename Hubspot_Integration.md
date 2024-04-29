# SmartLead to HubSpot Data Integration

## Overview
This integration automates the process of fetching lead details from the Airtable database and updating them on HubSpot using a POST request. It is designed to streamline lead data management and keep HubSpot data synchronized with SmartLead.

## Installation and Setup
1. **Clone Repository:**
   ```bash
   git clone https://github.com/your-username/smartlead-hubspot-integration.git

## Install Dependencies:
npm install

## Configuration:
Replace pipedriveApiKey with your actual Pipedrive API key.
Update the desired owner's ID in Pipedrive (owner_id variable).
Fill in the appropriate values for visible_to and other relevant fields as needed.
## Usage
Run Integration:
bash
## Copy code
node smartlead_hubspot_integration.js
## Code Overview
The provided code performs the following actions:

1.Fetches lead records from Airtable.

2.Prepares lead data for HubSpot, including email, name, company, website, LinkedIn URL, etc.

3.Makes a POST request to create a new organization in Pipedrive.

4.Makes a POST request to create a new person associated with the organization in Pipedrive.

5.Updates the Airtable status field to mark successful integration.


## Contributing
Contributions are welcome. Follow the guidelines in the repository for contributions.

## Support
For issues or questions, open an issue on GitHub.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
