---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.identity.signins/update-mgpolicyauthenticationmethodpolicy
schema: 2.0.0
---

# Update-MgPolicyAuthenticationMethodPolicy

## SYNOPSIS
The authentication methods and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).

## SYNTAX

### UpdateExpanded1 (Default)
```
Update-MgPolicyAuthenticationMethodPolicy [-AdditionalProperties <Hashtable>]
 [-AuthenticationMethodConfigurations <IMicrosoftGraphAuthenticationMethodConfiguration[]>]
 [-Description <String>] [-DisplayName <String>] [-Id <String>] [-LastModifiedDateTime <DateTime>]
 [-PolicyVersion <String>] [-ReconfirmationInDays <Int32>]
 [-RegistrationEnforcement <IMicrosoftGraphRegistrationEnforcement>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Update1
```
Update-MgPolicyAuthenticationMethodPolicy -BodyParameter <IMicrosoftGraphAuthenticationMethodsPolicy>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The authentication methods and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AuthenticationMethodConfigurations
Represents the settings for each authentication method.
Automatically expanded on GET /policies/authenticationMethodsPolicy.
To construct, please use Get-Help -Online and see NOTES section for AUTHENTICATIONMETHODCONFIGURATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationMethodConfiguration[]
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
authenticationMethodsPolicy
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationMethodsPolicy
Parameter Sets: Update1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Description
A description of the policy.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
The name of the policy.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded1
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
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
The date and time of the last update to the policy.
Read-only.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PolicyVersion
The version of the policy in use.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReconfirmationInDays
.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RegistrationEnforcement
registrationEnforcement
To construct, please use Get-Help -Online and see NOTES section for REGISTRATIONENFORCEMENT properties and create a hash table.

```yaml
Type: IMicrosoftGraphRegistrationEnforcement
Parameter Sets: UpdateExpanded1
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAuthenticationMethodsPolicy
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


AUTHENTICATIONMETHODCONFIGURATIONS <IMicrosoftGraphAuthenticationMethodConfiguration[]>: Represents the settings for each authentication method. Automatically expanded on GET /policies/authenticationMethodsPolicy.
  - `[Id <String>]`: Read-only.
  - `[State <String>]`: authenticationMethodState

BODYPARAMETER <IMicrosoftGraphAuthenticationMethodsPolicy>: authenticationMethodsPolicy
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: Read-only.
  - `[AuthenticationMethodConfigurations <IMicrosoftGraphAuthenticationMethodConfiguration[]>]`: Represents the settings for each authentication method. Automatically expanded on GET /policies/authenticationMethodsPolicy.
    - `[Id <String>]`: Read-only.
    - `[State <String>]`: authenticationMethodState
  - `[Description <String>]`: A description of the policy. Read-only.
  - `[DisplayName <String>]`: The name of the policy. Read-only.
  - `[LastModifiedDateTime <DateTime?>]`: The date and time of the last update to the policy. Read-only.
  - `[PolicyVersion <String>]`: The version of the policy in use. Read-only.
  - `[ReconfirmationInDays <Int32?>]`: 
  - `[RegistrationEnforcement <IMicrosoftGraphRegistrationEnforcement>]`: registrationEnforcement
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AuthenticationMethodsRegistrationCampaign <IMicrosoftGraphAuthenticationMethodsRegistrationCampaign>]`: authenticationMethodsRegistrationCampaign
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ExcludeTargets <IMicrosoftGraphExcludeTarget[]>]`: Users and groups of users that are excluded from being prompted to set up the authentication method.
        - `[Id <String>]`: The object identifier of an Azure Active Directory user or group.
        - `[TargetType <String>]`: authenticationMethodTargetType
      - `[IncludeTargets <IMicrosoftGraphAuthenticationMethodsRegistrationCampaignIncludeTarget[]>]`: Users and groups of users that are prompted to set up the authentication method.
        - `[Id <String>]`: The object identifier of an Azure Active Directory user or group.
        - `[TargetType <String>]`: authenticationMethodTargetType
        - `[TargetedAuthenticationMethod <String>]`: The authentication method that the user is prompted to register. The value must be microsoftAuthenticator.
      - `[SnoozeDurationInDays <Int32?>]`: Specifies the number of days that the user sees a prompt again if they select 'Not now' and snoozes the prompt. Minimum: 0 days. Maximum: 14 days. If the value is '0', the user is prompted during every MFA attempt.
      - `[State <String>]`: advancedConfigState

REGISTRATIONENFORCEMENT <IMicrosoftGraphRegistrationEnforcement>: registrationEnforcement
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AuthenticationMethodsRegistrationCampaign <IMicrosoftGraphAuthenticationMethodsRegistrationCampaign>]`: authenticationMethodsRegistrationCampaign
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ExcludeTargets <IMicrosoftGraphExcludeTarget[]>]`: Users and groups of users that are excluded from being prompted to set up the authentication method.
      - `[Id <String>]`: The object identifier of an Azure Active Directory user or group.
      - `[TargetType <String>]`: authenticationMethodTargetType
    - `[IncludeTargets <IMicrosoftGraphAuthenticationMethodsRegistrationCampaignIncludeTarget[]>]`: Users and groups of users that are prompted to set up the authentication method.
      - `[Id <String>]`: The object identifier of an Azure Active Directory user or group.
      - `[TargetType <String>]`: authenticationMethodTargetType
      - `[TargetedAuthenticationMethod <String>]`: The authentication method that the user is prompted to register. The value must be microsoftAuthenticator.
    - `[SnoozeDurationInDays <Int32?>]`: Specifies the number of days that the user sees a prompt again if they select 'Not now' and snoozes the prompt. Minimum: 0 days. Maximum: 14 days. If the value is '0', the user is prompted during every MFA attempt.
    - `[State <String>]`: advancedConfigState

## RELATED LINKS