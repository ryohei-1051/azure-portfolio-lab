# Lab 3 - Serverless TO-DO App with Azure Functions and Cosmos DB

## Objective

Build a simple serverless application using Azure Functions for the backend, Cosmos DB for storage, and static website hosting for the frontend.

## What I Built

- Azure Cosmos DB account using NoSQL API
- Cosmos DB database and container
- Azure Function App
- HTTP-triggered Azure Function
- Function app environment variables for Cosmos DB access
- Static website hosting in an Azure Storage Account
- Frontend HTML/JavaScript app connected to the function endpoint

## Architecture Summary

The application flow is:

1. User interacts with the static website frontend
2. Frontend sends requests to an HTTP-triggered Azure Function
3. Azure Function reads/writes task data in Cosmos DB
4. Results are returned to the frontend

## Why This Lab Matters

Although this is a small app, it demonstrates several useful Azure concepts:

- serverless compute
- frontend/backend integration
- app configuration through environment variables
- basic NoSQL design
- cloud-hosted static web delivery

## Validation Performed

- Confirmed Cosmos DB deployment
- Confirmed database and container creation
- Deployed Function App successfully
- Configured required environment variables
- Uploaded and validated function code deployment
- Confirmed function URL worked from the frontend
- Verified static website hosting and page loading
- Confirmed end-to-end TO-DO operations

## Issues / Troubleshooting

Examples of troubleshooting areas documented in this lab:

- function deployment and restart behavior
- app settings / environment variable mistakes
- incorrect function URL usage
- CORS-related frontend/backend communication issues
- Cosmos DB connectivity validation

## Security / Cost Notes

- Used free-tier / low-cost settings where possible
- Recognized that lab secrets stored in app settings should be improved for production
- Treated this as a functional prototype, not a hardened production deployment

## What I Learned

- Serverless integrations fail more often from configuration issues than from code issues
- Clear endpoint and secret handling is essential
- A small app becomes more portfolio-worthy when validation and architecture are documented clearly

## Next Improvements

- Replace direct secret storage with Azure Key Vault
- Use Managed Identity where possible
- Add Application Insights
- Add GitHub Actions deployment workflow
- Add authentication
- Improve input validation and error handling
- Expand the data model with due dates, priority, and status filtering
