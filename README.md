# CentralUnitsRouter.js

This module defines a class for handling routes related to central units using the Express framework. It encapsulates the route definitions, route handlers, and logic for interacting with a database to manage central units.

## Installation

To use this module in your Node.js application, follow these steps:

1. Install the required dependencies if you haven't already:

   ```bash
   npm install express body-parser moment

Import the CentralUnitsRouter class into your main application file:
const CentralUnitsRouter = require('./CentralUnitsRouter');

Create an instance of CentralUnitsRouter and pass your database connection:
const centralUnitsRouter = new CentralUnitsRouter(dbConnection);

Use the router in your main Express app:
app.use('/central_units', centralUnitsRouter.getRouter());

## Usage

The CentralUnitsRouter class defines various routes and their corresponding route handlers for managing central units. Below is a brief overview of each route:

Route Handlers
/central_units/update (POST): Handles updating central unit information.
/central_units/insert (POST): Handles inserting new central units.
/central_units/ (GET): Renders the central units index page.
/central_units/new (GET): Renders the page for adding a new central unit.
/listAllCentralUnits/ (GET): Lists all central units.
/central_units/:id (GET): Renders the details page for a specific central unit.
/central_units/:id/edit (GET): Renders the edit page for a specific central unit.
/listAllCentralUnitsSelect/ (GET): Lists central units for use in select inputs.
Each route handler method is responsible for handling its respective route's logic, including interacting with the database, rendering views, and handling redirects.
