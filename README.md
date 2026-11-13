# n8n Real Estate Social Media Posts Captions Generation Workflow
An n8n-powered AI automation that retrieves property information using RentCast API and generates customized real estate marketing content for Zillow, Instagram, and Facebook using Google Gemini. An intelligent real estate marketing automation built using n8n, Google Gemini, and RentCast API.

This workflow helps real estate agents generate property marketing content automatically by combining user-provided information with property data retrieved through the RentCast API. It transforms basic property details into platform-specific marketing content for Zillow, Instagram, and Facebook.

## Project Overview

Real estate agents often spend considerable time researching property information and creating marketing content for different platforms.

This automation simplifies the process by collecting property details, retrieving additional property information, and using generative AI to create customized marketing content based on the target buyer persona and property highlights.

## How It Works

1. ### User Input – n8n Form

The workflow begins with an n8n form where users provide:

- Property Address
- Target Buyer Persona
- Standout Key Feature

2. ### Property Data Retrieval – RentCast API

The RentCast API retrieves additional property information, including:

- Number of Bedrooms
- Number of Bathrooms
- Square Footage
- Year Built

3. ### Data Processing

The retrieved property information and user-provided inputs are processed and structured for AI content generation.

4. ### AI Content Generation – Google Gemini

Google Gemini generates three customized marketing outputs:

Zillow Property Description ("zillow_desc")

- Professional property descriptions.
- Highlights important property features.
- Incorporates relevant property information.

Instagram Marketing Caption ("instagram_post")

- Engaging social media captions.
- Property highlights.
- Marketing-focused messaging.

Facebook Advertising Copy ("facebook_ad")

- Target-audience-focused ad copy.
- Highlights property benefits.
- Persuasive marketing messaging.

5. ### Structured Output

The AI-generated response is formatted as structured JSON, allowing individual marketing outputs to be extracted and used separately.

Example Input

Property Address: 89 Hedden Terrace, Newark, NJ

Property Details:

- Bedrooms: 3
- Bathrooms: 2.5
- Square Footage: 2,200 sq. ft.
- Construction: Modern

Target Buyer Persona: Small and growing families.

Standout Features: Convenient NYC transit access, nearby parks and schools, open-concept living areas, modern kitchen, and backyard.

## Technologies Used

- n8n: Workflow automation and orchestration.
- RentCast API: Property information retrieval.
- Google Gemini: AI-powered marketing content generation.
- JavaScript: Data processing and JSON parsing.
- n8n Form: User input collection.

## Key Features

- Automated property information retrieval.
- Dynamic AI prompt generation.
- Buyer-persona-based content customization.
- Multi-platform marketing content generation.
- Structured JSON output.
- Reduced manual effort in property marketing.

## Workflow Architecture
<img width="1028" height="238" alt="Screenshot 2026-11-13 182647" src="https://github.com/user-attachments/assets/1423ffed-32af-438c-910a-5bcc2732964f" />

n8n Form
   |
   
User Property Details
   |
   
RentCast API
   |
   
Property Data Retrieval
   |
   
Data Processing
   |
   
Dynamic AI Prompt
   |
   
Google Gemini
   |
   
Marketing Content Generation
   |
   
Structured JSON Output
   |
   +----> Zillow Description
   |
   +----> Instagram Caption
   |
   +----> Facebook Ad Copy

## Setup and Configuration

1. Set up an n8n instance (self-hosted or cloud).
2. Create an n8n Form with the required property input fields.
3. Obtain API access from RentCast.
4. Configure RentCast API credentials in n8n.
5. Configure Google Gemini credentials.
6. Set up the AI prompt using the submitted property and buyer persona details.
7. Configure JSON parsing and output extraction.
8. Execute the workflow and test with property information.

## Requirements

- n8n instance.
- RentCast API access.
- Google Gemini API access.
- Basic understanding of n8n and JavaScript.

## Security

- Never expose API keys or authentication credentials.
- Store credentials securely using n8n credentials.
- Remove sensitive information before sharing workflow exports.
- Avoid uploading private property or customer information.

## Project Purpose

This project demonstrates how workflow automation can streamline real estate marketing by transforming property data into customized, platform-specific marketing content.

Built with n8n + Google Gemini + RentCast API.
