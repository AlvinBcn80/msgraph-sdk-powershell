---
external help file: Microsoft.Graph.Devices.CloudPrint-help.xml
Module Name: Microsoft.Graph.Devices.CloudPrint
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devices.cloudprint/new-mgprintservice
schema: 2.0.0
---

# New-MgPrintService

## SYNOPSIS
The list of available Universal Print service endpoints.

## SYNTAX

### CreateExpanded (Default)
```
New-MgPrintService [-AdditionalProperties <Hashtable>] [-Endpoints <IMicrosoftGraphPrintServiceEndpoint[]>]
 [-Id <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgPrintService -BodyParameter <IMicrosoftGraphPrintService> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The list of available Universal Print service endpoints.

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
printService
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphPrintService
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Endpoints
Endpoints that can be used to access the service.
Read-only.
Nullable.
To construct, please use Get-Help -Online and see NOTES section for ENDPOINTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphPrintServiceEndpoint[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Read-only.

```yaml
Type: String
Parameter Sets: CreateExpanded
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPrintService
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPrintService
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER <IMicrosoftGraphPrintService>: printService
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: Read-only.
  - `[Endpoints <IMicrosoftGraphPrintServiceEndpoint[]>]`: Endpoints that can be used to access the service. Read-only. Nullable.
    - `[Id <String>]`: Read-only.
    - `[DisplayName <String>]`: A human-readable display name for the endpoint.
    - `[Uri <String>]`: The URI that can be used to access the service.

ENDPOINTS <IMicrosoftGraphPrintServiceEndpoint[]>: Endpoints that can be used to access the service. Read-only. Nullable.
  - `[Id <String>]`: Read-only.
  - `[DisplayName <String>]`: A human-readable display name for the endpoint.
  - `[Uri <String>]`: The URI that can be used to access the service.

## RELATED LINKS