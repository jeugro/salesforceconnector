After installing this repo, do these changes


1) Create a Proxy Authentication to SalesForce, using oAuth 2.0
2) Change endpoint of API "SalesForce Connector Metadata"
     a) Add the newy created Proxy authentication 
     b) Change Endpoint from "https://neptune-software.my.salesforce.com" to your SalesForce endpoint


When defining a Connector in Open Edition, set StartParameters to the ID of the SalesForce Connector