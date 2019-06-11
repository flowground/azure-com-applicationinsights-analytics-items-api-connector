# ![LOGO](logo.png) ApplicationInsightsManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the ApplicationInsightsManagementClient API (version 2015-05-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/applicationinsights-analyticsItems_API/2015-05-01/swagger.json<br/>
Generated at: 2019-06-11T18:13:17+03:00

## API Description

Azure Application Insights client for saved items.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Gets a list of Analytics Items defined within an Application Insights component.

#### Input Parameters
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceGroupName` - _required_ - The name of the resource group.
* `resourceName` - _required_ - The name of the Application Insights component resource.
* `scopePath` - _required_ - Enum indicating if this item definition is owned by a specific user or is shared between all users with access to the Application Insights component.
    Possible values: analyticsItems, myanalyticsItems.
* `api-version` - _required_ - Client Api Version.
* `scope` - _optional_ - Enum indicating if this item definition is owned by a specific user or is shared between all users with access to the Application Insights component.
    Possible values: shared, user.
* `type` - _optional_ - Enum indicating the type of the Analytics item.
    Possible values: none, query, function, folder, recent.
* `includeContent` - _optional_ - Flag indicating whether or not to return the content of each applicable item. If false, only return the item information.

### Deletes a specific Analytics Items defined within an Application Insights component.

#### Input Parameters
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceGroupName` - _required_ - The name of the resource group.
* `resourceName` - _required_ - The name of the Application Insights component resource.
* `scopePath` - _required_ - Enum indicating if this item definition is owned by a specific user or is shared between all users with access to the Application Insights component.
    Possible values: analyticsItems, myanalyticsItems.
* `api-version` - _required_ - Client Api Version.
* `id` - _optional_ - The Id of a specific item defined in the Application Insights component
* `name` - _optional_ - The name of a specific item defined in the Application Insights component

### Gets a specific Analytics Items defined within an Application Insights component.

#### Input Parameters
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceGroupName` - _required_ - The name of the resource group.
* `resourceName` - _required_ - The name of the Application Insights component resource.
* `scopePath` - _required_ - Enum indicating if this item definition is owned by a specific user or is shared between all users with access to the Application Insights component.
    Possible values: analyticsItems, myanalyticsItems.
* `api-version` - _required_ - Client Api Version.
* `id` - _optional_ - The Id of a specific item defined in the Application Insights component
* `name` - _optional_ - The name of a specific item defined in the Application Insights component

### Adds or Updates a specific Analytics Item within an Application Insights component.

#### Input Parameters
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceGroupName` - _required_ - The name of the resource group.
* `resourceName` - _required_ - The name of the Application Insights component resource.
* `scopePath` - _required_ - Enum indicating if this item definition is owned by a specific user or is shared between all users with access to the Application Insights component.
    Possible values: analyticsItems, myanalyticsItems.
* `api-version` - _required_ - Client Api Version.
* `overrideItem` - _optional_ - Flag indicating whether or not to force save an item. This allows overriding an item if it already exists.

## License

**flow**ground :- Telekom iPaaS / azure-com-applicationinsights-analytics-items-api-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
