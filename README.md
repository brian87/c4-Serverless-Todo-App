### Amazon Web Services (AWS)

An AWS account is required to deploy the application.

### Auth0 R256

Auth0 is used for authentication and an Auth0 application should be created with asymmetrically encrypted keys (RS256).

## Getting started

### Backend

To build and deploy the application, first edit the `backend/serverless.yml` file to set the appropriate AWS and Auth0 parameters, then run the following commands:

1. cd to the backend folder: `cd backend`
2. Install dependencies: `npm install`
3. Build and deploy to AWS: `sls deploy -v`

### Frontend

To run the client application, first edit the `client/src/config.ts` file to set the appropriate AWS and Auth0 parameters, then run the following commands:

1. cd to the client folder: `cd client`
2. Install dependencies: `npm install`
3. Run the client application: `npm run start`

This should start a development server with the React application that will interact with the serverless TODO application.

### Postman collection

A Postman collection is available in the root folder of the project, as an alternative way to test the API.