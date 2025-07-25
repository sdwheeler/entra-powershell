---
author: msewaweru
description: This article provides details on the New-EntraPermissionGrantPolicy command.
external help file: Microsoft.Entra.SignIns-Help.xml
Locale: en-US
manager: mwongerapk
Module Name: Microsoft.Entra
ms.author: eunicewaweru
ms.date: 06/26/2024
ms.reviewer: stevemutungi
ms.topic: reference
online version: https://learn.microsoft.com/powershell/module/Microsoft.Entra/New-EntraPermissionGrantPolicy
schema: 2.0.0
title: New-EntraPermissionGrantPolicy
---

# New-EntraPermissionGrantPolicy

## SYNOPSIS

Creates a permission grant policy.

## SYNTAX

```powershell
New-EntraPermissionGrantPolicy
 -Id <String>
 [-DisplayName <String>]
 [-Description <String>]
 [<CommonParameters>]
```

## DESCRIPTION

The `New-EntraPermissionGrantPolicy` cmdlet creates a Microsoft Entra ID permission grant policy.

## EXAMPLES

### Example 1: Create a permission grant policy

```powershell
Connect-Entra -Scopes 'Policy.ReadWrite.PermissionGrant'
New-EntraPermissionGrantPolicy -Id 'my_new_permission_grant_policy_id' -DisplayName 'MyNewPermissionGrantPolicy' -Description 'My new permission grant policy'
```

```Output
DeletedDateTime Description                    DisplayName                Id
--------------- -----------                    -----------                --
                My new permission grant policy MyNewPermissionGrantPolicy my_new_permission_grant_policy_id
```

This example creates new permission grant policy in Microsoft Entra ID.

- `-Id` parameter specifies the unique identifier of the permission grant policy.
- `-DisplayName` parameter specifies the display name for the permission grant policy.
- `-Description` parameter specifies the description for the permission grant policy.

## PARAMETERS

### -Description

Specifies the description for the permission grant policy.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName

Specifies the display name for the permission grant policy.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id

Specifies the unique identifier of the permission grant policy.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: `-Debug`, `-ErrorAction`, `-ErrorVariable`, `-InformationAction`, `-InformationVariable`, `-OutVariable`, `-OutBuffer`, `-PipelineVariable`, `-Verbose`, `-WarningAction`, and `-WarningVariable`. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-EntraPermissionGrantPolicy](Get-EntraPermissionGrantPolicy.md)

[Set-EntraPermissionGrantPolicy](Set-EntraPermissionGrantPolicy.md)

[Remove-EntraPermissionGrantPolicy](Remove-EntraPermissionGrantPolicy.md)
