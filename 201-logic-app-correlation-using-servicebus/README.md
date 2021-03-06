# Correlating messages over Logic Apps using Service Bus

<IMG SRC="https://azbotstorage.blob.core.windows.net/badges/201-logic-app-correlation-using-servicebus/PublicLastTestDate.svg" />&nbsp;
<IMG SRC="https://azbotstorage.blob.core.windows.net/badges/201-logic-app-correlation-using-servicebus/PublicDeployment.svg" />&nbsp;

<IMG SRC="https://azbotstorage.blob.core.windows.net/badges/201-logic-app-correlation-using-servicebus/FairfaxLastTestDate.svg" />&nbsp;
<IMG SRC="https://azbotstorage.blob.core.windows.net/badges/201-logic-app-correlation-using-servicebus/FairfaxDeployment.svg" />&nbsp;

<IMG SRC="https://azbotstorage.blob.core.windows.net/badges/201-logic-app-correlation-using-servicebus/BestPracticeResult.svg" />&nbsp;
<IMG SRC="https://azbotstorage.blob.core.windows.net/badges/201-logic-app-correlation-using-servicebus/CredScanResult.svg" />&nbsp;

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2F201-logic-app-correlation-using-servicebus%2Fazuredeploy.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2F201-logic-app-correlation-using-servicebus%2Fazuredeploy.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.png"/>
</a>

## Solution overview and deployed resources

This template deploys a solution which shows how we can correlate messages over Logic Apps using Azure Service Bus. The Logic App receives a message through a web endpoint, and sends the message to a MockBin endpoint, and returns the response to the original caller.

The following resources are deployed as part of the solution.

+ **Logic App**

To test the Logic App, grab the endpoint of the Request shape in the Logic App, and use a tool like PostMan to POST a message to the endpoint. The message to be sent in should be in the following format.

```json
{
    "Customer":"Eldert Grootenboer",
    "Product":"Surface Book 2",
    "Amount":"1"
}
```

`Tags: Logic Apps, Logic App, LogicApps, ServiceBus, Service Bus, SessionId, Session Id, Correlation`
