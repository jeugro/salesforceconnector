After installing this repo, do these changes


1) Create a Proxy Authentication to SalesForce, using oAuth 2.0
2) Use API Designer and open "SalesForce Connector Metadata":

- Add the new created Proxy authentication to the API
- Change Endpoint from "https://neptune-software.my.salesforce.com" to your SalesForce endpoint


# Create new Salesforce Connector
Start the Application /app/planet9_salesforce_connector

When defining a Connector (from the Cockpit) in Open Edition, use the following setup:

1) Use type Server Script 

        Setup (Selection & Fields): (SalesForceConnector) SalesforceAdaptiveRun

        Run: (SalesForceConnector) SalesforceAdaptiveRun

        Set StartParameters to the ID of the SalesForce Connector