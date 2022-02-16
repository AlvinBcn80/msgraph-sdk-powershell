---
external help file: Microsoft.Graph.DeviceManagement.Actions-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Actions
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devicemanagement.actions/test-mgdevicemanagementassignmentfilter
schema: 2.0.0
---

# Test-MgDeviceManagementAssignmentFilter

## SYNOPSIS
Invoke action validateFilter

## SYNTAX

### ValidateExpanded (Default)
```
Test-MgDeviceManagementAssignmentFilter [-AdditionalProperties <Hashtable>]
 [-DeviceAndAppManagementAssignmentFilter <IMicrosoftGraphDeviceAndAppManagementAssignmentFilter>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Validate
```
Test-MgDeviceManagementAssignmentFilter
 -BodyParameter <IPaths1Y9WuhoDevicemanagementAssignmentfiltersMicrosoftGraphValidatefilterPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action validateFilter

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: ValidateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPaths1Y9WuhoDevicemanagementAssignmentfiltersMicrosoftGraphValidatefilterPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Validate
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DeviceAndAppManagementAssignmentFilter
A class containing the properties used for Assignment Filter.
To construct, please use Get-Help -Online and see NOTES section for DEVICEANDAPPMANAGEMENTASSIGNMENTFILTER properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceAndAppManagementAssignmentFilter
Parameter Sets: ValidateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IPaths1Y9WuhoDevicemanagementAssignmentfiltersMicrosoftGraphValidatefilterPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER <IPaths1Y9WuhoDevicemanagementAssignmentfiltersMicrosoftGraphValidatefilterPostRequestbodyContentApplicationJsonSchema>: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DeviceAndAppManagementAssignmentFilter <IMicrosoftGraphDeviceAndAppManagementAssignmentFilter>]`: A class containing the properties used for Assignment Filter.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: Read-only.
    - `[CreatedDateTime <DateTime?>]`: Creation time of the Assignment Filter.
    - `[Description <String>]`: Description of the Assignment Filter.
    - `[DisplayName <String>]`: DisplayName of the Assignment Filter.
    - `[LastModifiedDateTime <DateTime?>]`: Last modified time of the Assignment Filter.
    - `[Platform <String>]`: Supported platform types.
    - `[RoleScopeTags <String[]>]`: RoleScopeTags of the Assignment Filter.
    - `[Rule <String>]`: Rule definition of the Assignment Filter.

DEVICEANDAPPMANAGEMENTASSIGNMENTFILTER <IMicrosoftGraphDeviceAndAppManagementAssignmentFilter>: A class containing the properties used for Assignment Filter.
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: Read-only.
  - `[CreatedDateTime <DateTime?>]`: Creation time of the Assignment Filter.
  - `[Description <String>]`: Description of the Assignment Filter.
  - `[DisplayName <String>]`: DisplayName of the Assignment Filter.
  - `[LastModifiedDateTime <DateTime?>]`: Last modified time of the Assignment Filter.
  - `[Platform <String>]`: Supported platform types.
  - `[RoleScopeTags <String[]>]`: RoleScopeTags of the Assignment Filter.
  - `[Rule <String>]`: Rule definition of the Assignment Filter.

## RELATED LINKS