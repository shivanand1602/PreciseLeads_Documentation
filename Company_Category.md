# Company Category Classifier 

## Overview
This extension leverages OpenAI's GPT-3.5 model to classify companies into categories such as remote, hybrid, or onsite based on their provided company name, description, and about information.

It helps in understanding the work culture or setup of companies quickly and efficiently.

## Tools Used-
1. Database- Airtable
2. OpenAI- GPT-3.5
3. Airtable Scripting Extension

## Tech Stack Used-
1. Language-JavaScript
2. Rest API

## Installation and Setup
1. **Clone Repository:**
   ```bash
   git clone https://github.com/your-username/company-category-classifier.git

## Install Dependencies
npm install

## Configuration
1. Replace apiKey with your actual OpenAI API key.
2. Ensure the base.getTable method is correctly configured to fetch records from your Airtable database.

## Usage
1. Input Data
  a) Provide the following information for each company record in your Airtable:
  b) Company Name
  c)Company Description
  d)About Company

2. Output Data:
The extension will populate the 'Category' field in Airtable with the classification result ('Remote', 'Hybrid', or 'Onsite') for each company.

## Code Overview
The provided code performs the following actions:

1.Fetches company records from the specified Airtable table.

2.Constructs prompts for the OpenAI API using company details.

3.Sends a POST request to the OpenAI API for classification.

4.Updates the Airtable records with the classification result.

## Contributing
Contributions to enhance or optimize the classification process are welcome. Please follow the contribution guidelines in the repository.
