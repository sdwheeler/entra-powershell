---
title: Remove-EntraApplication
description: This article provides details on the Remove-EntraApplication command.

ms.topic: reference
ms.date: 06/26/2024
ms.author: eunicewaweru
ms.reviewer: stevemutungi
manager: mwongerapk

external help file: Microsoft.Graph.Entra-Help.xml
Module Name: Microsoft.Graph.Entra
online version: https://learn.microsoft.com/powershell/module/Microsoft.Graph.Entra/Remove-EntraApplication

schema: 2.0.0
---

# Remove-EntraApplication

## Synopsis

Deletes an application object.

## Syntax

```powershell
Remove-EntraApplication
 -ApplicationId <String>
 [<CommonParameters>]
```

## Description

The `Remove-EntraApplication` cmdlet deletes an application object identified by ApplicationId. Specify the `ApplicationId` parameter to delete an application object.

## Examples

### Example 1: Remove an application

```powershell
Connect-Entra -Scopes 'Application.ReadWrite.All'
$Application = Get-EntraApplication -SearchString '<application-name>'
Remove-EntraApplication -ApplicationId $Application.ObjectId
```

This example demonstrates how to delete an application object.

## Parameters

### -ApplicationId

Specifies the ID of an application in Microsoft Entra ID.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: ObjectId

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: `-Debug`, `-ErrorAction`, `-ErrorVariable`, `-InformationAction`, `-InformationVariable`, `-OutVariable`, `-OutBuffer`, `-PipelineVariable`, `-Verbose`, `-WarningAction`, and `-WarningVariable`. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/?LinkID=113216).

## Inputs

### System.String

## Outputs

## Notes

## Related Links

[Get-EntraApplication](Get-EntraApplication.md)

[New-EntraApplication](New-EntraApplication.md)

[Set-EntraApplication](Set-EntraApplication.md)
