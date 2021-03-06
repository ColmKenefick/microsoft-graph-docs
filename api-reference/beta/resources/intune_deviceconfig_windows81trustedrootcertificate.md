﻿# windows81TrustedRootCertificate resource type

> **Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported.

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Windows 8.1 Trusted Certificate configuration profile

Inherits from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windows81TrustedRootCertificates](../api/intune_deviceconfig_windows81trustedrootcertificate_list.md)|[windows81TrustedRootCertificate](../resources/intune_deviceconfig_windows81trustedrootcertificate.md) collection|List properties and relationships of the [windows81TrustedRootCertificate](../resources/intune_deviceconfig_windows81trustedrootcertificate.md) objects.|
|[Get windows81TrustedRootCertificate](../api/intune_deviceconfig_windows81trustedrootcertificate_get.md)|[windows81TrustedRootCertificate](../resources/intune_deviceconfig_windows81trustedrootcertificate.md)|Read properties and relationships of the [windows81TrustedRootCertificate](../resources/intune_deviceconfig_windows81trustedrootcertificate.md) object.|
|[Create windows81TrustedRootCertificate](../api/intune_deviceconfig_windows81trustedrootcertificate_create.md)|[windows81TrustedRootCertificate](../resources/intune_deviceconfig_windows81trustedrootcertificate.md)|Create a new [windows81TrustedRootCertificate](../resources/intune_deviceconfig_windows81trustedrootcertificate.md) object.|
|[Delete windows81TrustedRootCertificate](../api/intune_deviceconfig_windows81trustedrootcertificate_delete.md)|None|Deletes a [windows81TrustedRootCertificate](../resources/intune_deviceconfig_windows81trustedrootcertificate.md).|
|[Update windows81TrustedRootCertificate](../api/intune_deviceconfig_windows81trustedrootcertificate_update.md)|[windows81TrustedRootCertificate](../resources/intune_deviceconfig_windows81trustedrootcertificate.md)|Update the properties of a [windows81TrustedRootCertificate](../resources/intune_deviceconfig_windows81trustedrootcertificate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the entity. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|trustedRootCertificate|Binary|Trusted Root Certificate|
|certFileName|String|File name to display in UI.|
|destinationStore|String|Destination store location for the Trusted Root Certificate. Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune_deviceconfig_deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection|Device configuration installation stauts by user. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows81TrustedRootCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "destinationStore": "String"
}
```



