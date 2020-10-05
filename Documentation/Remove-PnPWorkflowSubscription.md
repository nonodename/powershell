---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpworkflowsubscription
schema: 2.0.0
title: Remove-PnPWorkflowSubscription
---

# Remove-PnPWorkflowSubscription

## SYNOPSIS
Removes a SharePoint 2010/2013 workflow subscription

## SYNTAX

```
Remove-PnPWorkflowSubscription [-Identity] <WorkflowSubscriptionPipeBind> [-Web <WebPipeBind>]
 [-Connection <PnPConnection>] [<CommonParameters>]
```

## DESCRIPTION
Removes a previously registered SharePoint 2010/2013 workflow subscription

## EXAMPLES

### EXAMPLE 1
```powershell
Remove-PnPWorkflowSubscription -Identity $wfSub
```

Removes the workflowsubscription, retrieved by Get-PnPWorkflowSubscription.

### EXAMPLE 2
```powershell
Get-PnPWorkflowSubscription -Name MyWorkflow | Remove-PnPWorkflowSubscription
```

Get the workflowSubscription MyWorkFlow and remove it.

## PARAMETERS

### -Connection
Optional connection to be used by the cmdlet. Retrieve the value for this parameter by either specifying -ReturnConnection on Connect-PnPOnline or by executing Get-PnPConnection.

```yaml
Type: PnPConnection
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
The subscription to remove

```yaml
Type: WorkflowSubscriptionPipeBind
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Web
This parameter allows you to optionally apply the cmdlet action to a subweb within the current web. In most situations this parameter is not required and you can connect to the subweb using Connect-PnPOnline instead. Specify the GUID, server relative url (i.e. /sites/team1) or web instance of the web to apply the command to. Omit this parameter to use the current web.

```yaml
Type: WebPipeBind
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)