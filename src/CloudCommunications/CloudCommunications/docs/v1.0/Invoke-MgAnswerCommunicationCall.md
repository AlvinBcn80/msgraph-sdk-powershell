---
external help file: Microsoft.Graph.CloudCommunications-help.xml
Module Name: Microsoft.Graph.CloudCommunications
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.cloudcommunications/invoke-mganswercommunicationcall
schema: 2.0.0
---

# Invoke-MgAnswerCommunicationCall

## SYNOPSIS
Invoke action answer

## SYNTAX

### AnswerExpanded1 (Default)
```
Invoke-MgAnswerCommunicationCall -CallId <String> [-AcceptedModalities <String[]>]
 [-AdditionalProperties <Hashtable>] [-CallOptions <Hashtable>] [-CallbackUri <String>]
 [-MediaConfig <Hashtable>] [-ParticipantCapacity <Int32>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Answer1
```
Invoke-MgAnswerCommunicationCall -CallId <String>
 -BodyParameter <IPathsQvpqn4CommunicationsCallsCallIdMicrosoftGraphAnswerPostRequestbodyContentApplicationJsonSchema1>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### AnswerViaIdentityExpanded1
```
Invoke-MgAnswerCommunicationCall -InputObject <ICloudCommunicationsIdentity> [-AcceptedModalities <String[]>]
 [-AdditionalProperties <Hashtable>] [-CallOptions <Hashtable>] [-CallbackUri <String>]
 [-MediaConfig <Hashtable>] [-ParticipantCapacity <Int32>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### AnswerViaIdentity1
```
Invoke-MgAnswerCommunicationCall -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IPathsQvpqn4CommunicationsCallsCallIdMicrosoftGraphAnswerPostRequestbodyContentApplicationJsonSchema1>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action answer

## EXAMPLES

## PARAMETERS

### -AcceptedModalities
.

```yaml
Type: String[]
Parameter Sets: AnswerExpanded1, AnswerViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: AnswerExpanded1, AnswerViaIdentityExpanded1
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
Type: IPathsQvpqn4CommunicationsCallsCallIdMicrosoftGraphAnswerPostRequestbodyContentApplicationJsonSchema1
Parameter Sets: Answer1, AnswerViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CallbackUri
.

```yaml
Type: String
Parameter Sets: AnswerExpanded1, AnswerViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CallId
key: id of call

```yaml
Type: String
Parameter Sets: AnswerExpanded1, Answer1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CallOptions
incomingCallOptions

```yaml
Type: Hashtable
Parameter Sets: AnswerExpanded1, AnswerViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, please use Get-Help -Online and see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: ICloudCommunicationsIdentity
Parameter Sets: AnswerViaIdentityExpanded1, AnswerViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MediaConfig
mediaConfig

```yaml
Type: Hashtable
Parameter Sets: AnswerExpanded1, AnswerViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ParticipantCapacity
.

```yaml
Type: Int32
Parameter Sets: AnswerExpanded1, AnswerViaIdentityExpanded1
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

### Microsoft.Graph.PowerShell.Models.ICloudCommunicationsIdentity
### Microsoft.Graph.PowerShell.Models.IPathsQvpqn4CommunicationsCallsCallIdMicrosoftGraphAnswerPostRequestbodyContentApplicationJsonSchema1
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER <IPathsQvpqn4CommunicationsCallsCallIdMicrosoftGraphAnswerPostRequestbodyContentApplicationJsonSchema1>: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AcceptedModalities <String[]>]`: 
  - `[CallOptions <IMicrosoftGraphIncomingCallOptions>]`: incomingCallOptions
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[HideBotAfterEscalation <Boolean?>]`: 
  - `[CallbackUri <String>]`: 
  - `[MediaConfig <IMicrosoftGraphMediaConfig>]`: mediaConfig
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ParticipantCapacity <Int32?>]`: 

INPUTOBJECT <ICloudCommunicationsIdentity>: Identity Parameter
  - `[AttendanceRecordId <String>]`: key: id of attendanceRecord
  - `[AudioRoutingGroupId <String>]`: key: id of audioRoutingGroup
  - `[CallId <String>]`: key: id of call
  - `[CallRecordId <String>]`: key: id of callRecord
  - `[CommsOperationId <String>]`: key: id of commsOperation
  - `[MeetingAttendanceReportId <String>]`: key: id of meetingAttendanceReport
  - `[MeetingRegistrationQuestionId <String>]`: key: id of meetingRegistrationQuestion
  - `[OnlineMeetingId <String>]`: key: id of onlineMeeting
  - `[ParticipantId <String>]`: key: id of participant
  - `[PresenceId <String>]`: key: id of presence
  - `[SessionId <String>]`: key: id of session
  - `[UserId <String>]`: key: id of user

## RELATED LINKS