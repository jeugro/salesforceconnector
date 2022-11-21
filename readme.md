Using the Salesforce Connector, you can easily build adaptive apps to work with your Salesforce Data.

This comprises the following steps:

1) In the Open Edition cockpit, using the "Development Package" app, import the Salesforce Connector from this repo. This imports all artifacts which you need in the next steps.
2) Configure the API connection to Salesforce:
    1) Create a Proxy Authentication to SalesForce, using oAuth 2.0
    2) Use API Designer and open "SalesForce Connector Metadata":
        - Add the new created Proxy authentication to the API
        - Change Endpoint from "https://neptune-software.my.salesforce.com" to your SalesForce endpoint
3) Open the configuration app at https:<your_host>:<your_port>/app/planet9_salesforce_connector.
4) Using the configuration app you create connector configurations that can then be used to create adaptive applications without any backend coding required.
    1) In the connector overview, select "New entry".
    2) Provide a name and description and select the Salesforce table you want to use.
    3) ...
 5) Now you can create an Open Edition Connector in the cockpit which uses the configuration created in the step before:
    1) Create a connector with a data source of type "Server Script".
    2) As setup script choose SalesForceConnector->SalesForceAdaptiveSetup.
    3) As run script choose SalesForceConnector->SalesForceAdaptiveRun.
    4) Set StartParameters to the ID/GUID of the SalesForce Connector created in the step before.
 6) Now you can create adaptive applications in the normal way, specifying the Open Edition connector from the last step. The backend is already in place, based on your SalesForce connector configuration. Just configure the adaptive application according to your needs and then you are ready to go. 
 