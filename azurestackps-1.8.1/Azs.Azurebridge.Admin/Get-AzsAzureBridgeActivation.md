---
external help file: Azs.Azurebridge.Admin-help.xml
Module Name: Azs.Azurebridge.Admin
online version:
schema: 2.0.0
---

# Get-AzsAzureBridgeActivation

## SYNOPSIS
Returns the Azure Bridge Activation.

## SYNTAX

### List (Default)
```
Get-AzsAzureBridgeActivation -ResourceGroupName <String> [-Skip <Int32>] [-Top <Int32>] [<CommonParameters>]
```

### Get
```
Get-AzsAzureBridgeActivation -Name <String> -ResourceGroupName <String> [<CommonParameters>]
```

### ResourceId
```
Get-AzsAzureBridgeActivation -ResourceId <String> [<CommonParameters>]
```

## DESCRIPTION
Once Azure Stack has been registered, the activation object contains information that links an Azure Stack deployment to its registration in Azure, for example, the registration expiration date, name, etc.

## EXAMPLES

### EXAMPLE 1
```
Get-AzsAzureBridgeActivation -ResourceGroupName 'activationRG'
```

Get a list of Azure Bridge Activations under the resource group "activationRG"

### EXAMPLE 2
```
Get-AzsAzureBridgeActivation -Name 'myActivation' -ResourceGroupName 'activationRG'
```

Get an Azure Bridge Activation by name 'myActivation' situated under 'activationRG'

## PARAMETERS

### -Name
Name of the activation.

```yaml
Type: String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
The Resource Group used during the registration of Azure Stack; you can also view Resource Group names in the portal.

```yaml
Type: String
Parameter Sets: List, Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceId
The resource id.

```yaml
Type: String
Parameter Sets: ResourceId
Aliases: id

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Skip
Skip the first N items as specified by the parameter value.

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: -1
Accept pipeline input: False
Accept wildcard characters: False
```

### -Top
Return the top N items as specified by the parameter value.
Applies after the -Skip parameter.

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: -1
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.AzureStack.Management.AzureBridge.Admin.Models.ActivationResource

## NOTES

## RELATED LINKS
