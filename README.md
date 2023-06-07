# Propel Demo Dashboard - NextJS & React

This is a basic NextJS that allows you to connect to your Propel account and display Metrics in a table. 

> Note: This app was created to accompany a blog article that explains how to set it up. When the article is published, I will link to it here.

## How to use

### Create an application using Propel

You can find the API docs at https://www.propeldata.com/docs.

You'll need to complete the following steps:

1. Create an Account at https://www.propeldata.com/request-access
2. Connect a Data Source
3. Create a Data Pool
4. Define a Metric
5. Build an Application

Once you have built an Application inside Propel, you're ready to move on.

### Set up your local development environment

Rename the `.env.sample` file in the project's root directory to `.env.local`, then edit that file to contain your own API keys.

```.env
CLIENT_ID_SAMPLE_APP=1jb...
CLIENT_SECRET_SAMPLE_APP=1og...
```

You'll find these API keys by navigating to https://console.propeldata.com/applications/, selecting your sample application, and looking at the section labeled **OAuth2 client credentials**.

Leave the other environment variables that are already present in that file, such as `TOKEN_HOST` and `TOKEN_PATH`.

### Run your local development server

1. Run `yarn` to install the sample application's dependencies.
2. Run `yarn dev` to launch the local development server.
3. Browse to https://localhost:3000.

### Edit your GraphQL queries

Edit the `MetricsQuery` file in /graphql/ directory to use a different query. 


