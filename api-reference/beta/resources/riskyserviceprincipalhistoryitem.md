---
title: "riskyServicePrincipalHistoryItem resource type"
description: "Represents the risk history of Azure AD service principals"
author: "ebasseri"
localization_priority: Normal
ms.prod: "microsoft-identity-platform"
doc_type: resourcePageType
---

# riskyServicePrincipalHistoryItem resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Represents the risk history of an Azure AD service principal as determined by Azure AD Identity Protection. 

## Methods

| Method   | Return Type|Description|
|:---------------|:--------|:----------|
|[List history](../api/riskyserviceprincipal-list-history.md) | [riskyServicePrincipalHistoryItem](riskyserviceprincipalhistoryitem.md) collection|Get the risk history of an Azure AD service principal.|


## Properties

| Property       | Type    | Description |
|:---------------|:--------|:------------|
| servicePrincipalId         | string  | The id of the service principal. |
| initiatedBy    | bool    | The id of actor that does the operation. |
| activity       | [riskyServicePrincipalHistoryItem](riskserviceprincipalactivity.md)| The activity related to service principal risk level change. | 

## JSON representation

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyServicePrincipalHistoryItem",
  "baseType": "microsoft.graph.riskyServicePrincipals"
}-->

```json
{
    "servicePrincipalId": "string",
    "initiatedBy": "string",
    "activity": {"@odata.type": "microsoft.graph.riskyServicePrincipalActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyServicePrincipalHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
