After installing this repo, do these changes


1) Create a Proxy Authentication to SalesForce, using oAuth 2.0
2) Use API Designer and open "SalesForce Connector Metadata":

- Add the new created Proxy authentication to the API
- Change Endpoint from "https://neptune-software.my.salesforce.com" to your SalesForce endpoint


When defining a Connector in Open Edition, set StartParameters to the ID of the SalesForce Connector