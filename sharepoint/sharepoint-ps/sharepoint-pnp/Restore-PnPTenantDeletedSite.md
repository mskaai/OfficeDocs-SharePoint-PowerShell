---
Module Name: PnP.PowerShell
title: Restore-PnPTenantSite
schema: 2.0.0
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
online version: https://pnp.github.io/powershell/cmdlets/Restore-PnPTenantSite.html
---
 
# Restore-PnPTenantSite

## SYNOPSIS

> [!TIP]
> We encourage you to make improvements to this documentation. Please navigate to https://github.com/pnp/powershell/blob/dev/documentation/Restore-PnPTenantDeletedSite.md to change this file.


**Required Permissions**

* SharePoint: Access to the SharePoint Tenant Administration site

Restores a site collection from the Tenant recycle bin.

## SYNTAX

```powershell
Restore-PnPTenantSite [-Identity] <String> [-Force] [-NoWait] [-Connection <PnPConnection>]
 [<CommonParameters>]
```

## DESCRIPTION
Restores a site collection which is listed in your tenant administration site from the tenant's recycle bin.

## EXAMPLES

### EXAMPLE 1
```powershell
Restore-PnPTenantSite -Identity "https://tenant.sharepoint.com/sites/contoso"
```

This will restore the site collection with the url 'https://tenant.sharepoint.com/sites/contoso' from the recycle bin.

### EXAMPLE 2
```powershell
Restore-PnPTenantSite -Identity "https://tenant.sharepoint.com/sites/contoso" -Force
```

This will restore the site collection with the url 'https://tenant.sharepoint.com/sites/contoso' with force from the recycle bin.

## PARAMETERS

### -Connection
Optional connection to be used by the cmdlet. Retrieve the value for this parameter by either specifying -ReturnConnection on Connect-PnPOnline or by executing Get-PnPConnection.

```yaml
Type: PnPConnection
Parameter Sets: (All)

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Do not ask for confirmation.

```yaml
Type: SwitchParameter
Parameter Sets: (All)

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoWait
If specified the task will return immediately after creating the restore site job.

```yaml
Type: SwitchParameter
Parameter Sets: (All)

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```


### -Identity
Specifies the full URL of the site collection that needs to be restored.

```yaml
Type: String
Parameter Sets: (All)

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## RELATED LINKS

[Microsoft 365 Patterns and Practices](https://aka.ms/m365pnp)

