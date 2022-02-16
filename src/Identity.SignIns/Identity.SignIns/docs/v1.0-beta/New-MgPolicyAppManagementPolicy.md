---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.identity.signins/new-mgpolicyappmanagementpolicy
schema: 2.0.0
---

# New-MgPolicyAppManagementPolicy

## SYNOPSIS
The policies that enforce app management restrictions for specific applications and service principals, overriding the defaultAppManagementPolicy.

## SYNTAX

### CreateExpanded (Default)
```
New-MgPolicyAppManagementPolicy [-AdditionalProperties <Hashtable>]
 [-AppliesTo <IMicrosoftGraphDirectoryObject[]>] [-DeletedDateTime <DateTime>] [-Description <String>]
 [-DisplayName <String>] [-Id <String>] [-IsEnabled]
 [-Restrictions <IMicrosoftGraphAppManagementConfiguration>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgPolicyAppManagementPolicy -BodyParameter <IMicrosoftGraphAppManagementPolicy> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The policies that enforce app management restrictions for specific applications and service principals, overriding the defaultAppManagementPolicy.

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

### -AppliesTo
Collection of application and service principals to which a policy is applied.
To construct, please use Get-Help -Online and see NOTES section for APPLIESTO properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryObject[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
appManagementPolicy
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAppManagementPolicy
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DeletedDateTime
.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
Description for this policy.
Required.

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

### -DisplayName
Display name for this policy.
Required.

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

### -IsEnabled
Denotes whether the policy is enabled.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Restrictions
appManagementConfiguration
To construct, please use Get-Help -Online and see NOTES section for RESTRICTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAppManagementConfiguration
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAppManagementPolicy
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAppManagementPolicy
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


APPLIESTO <IMicrosoftGraphDirectoryObject[]>: Collection of application and service principals to which a policy is applied.
  - `[Id <String>]`: Read-only.
  - `[DeletedDateTime <DateTime?>]`: 

BODYPARAMETER <IMicrosoftGraphAppManagementPolicy>: appManagementPolicy
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Description <String>]`: Description for this policy. Required.
  - `[DisplayName <String>]`: Display name for this policy. Required.
  - `[DeletedDateTime <DateTime?>]`: 
  - `[Id <String>]`: Read-only.
  - `[AppliesTo <IMicrosoftGraphDirectoryObject[]>]`: Collection of application and service principals to which a policy is applied.
    - `[Id <String>]`: Read-only.
    - `[DeletedDateTime <DateTime?>]`: 
  - `[IsEnabled <Boolean?>]`: Denotes whether the policy is enabled.
  - `[Restrictions <IMicrosoftGraphAppManagementConfiguration>]`: appManagementConfiguration
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[KeyCredentials <IMicrosoftGraphKeyCredentialConfiguration[]>]`: Collection of keyCredential restrictions settings to be applied to an application or service principal.
      - `[MaxLifetime <TimeSpan?>]`: 
      - `[RestrictForAppsCreatedAfterDateTime <DateTime?>]`: Timestamp when the policy is enforced for all apps created on or after the specified date. For existing applications, the enforcement date would be back dated. To apply to all applications regardless of their creation date, this property would be null. Nullable.
      - `[RestrictionType <String>]`: appKeyCredentialRestrictionType
    - `[PasswordCredentials <IMicrosoftGraphPasswordCredentialConfiguration[]>]`: Collection of password restrictions settings to be applied to an application or service principal.
      - `[MaxLifetime <TimeSpan?>]`: 
      - `[RestrictForAppsCreatedAfterDateTime <DateTime?>]`: Enforces the policy for an app created on or after the enforcement date. For existing applications, the enforcement date would be back dated. To apply to all applications, enforcement datetime would be null.
      - `[RestrictionType <String>]`: appCredentialRestrictionType

RESTRICTIONS <IMicrosoftGraphAppManagementConfiguration>: appManagementConfiguration
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[KeyCredentials <IMicrosoftGraphKeyCredentialConfiguration[]>]`: Collection of keyCredential restrictions settings to be applied to an application or service principal.
    - `[MaxLifetime <TimeSpan?>]`: 
    - `[RestrictForAppsCreatedAfterDateTime <DateTime?>]`: Timestamp when the policy is enforced for all apps created on or after the specified date. For existing applications, the enforcement date would be back dated. To apply to all applications regardless of their creation date, this property would be null. Nullable.
    - `[RestrictionType <String>]`: appKeyCredentialRestrictionType
  - `[PasswordCredentials <IMicrosoftGraphPasswordCredentialConfiguration[]>]`: Collection of password restrictions settings to be applied to an application or service principal.
    - `[MaxLifetime <TimeSpan?>]`: 
    - `[RestrictForAppsCreatedAfterDateTime <DateTime?>]`: Enforces the policy for an app created on or after the enforcement date. For existing applications, the enforcement date would be back dated. To apply to all applications, enforcement datetime would be null.
    - `[RestrictionType <String>]`: appCredentialRestrictionType

## RELATED LINKS