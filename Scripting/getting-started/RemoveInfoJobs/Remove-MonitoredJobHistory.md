---
external help file: PSJobMonitor-help.xml
Module Name: PSJobMonitor
online version: 
schema: 2.0.0
---

# Remove-MonitoredJobHistory

## SYNOPSIS
Elimina la información del historial de todos los Job del registro de monitoreo, a partir del valor DaysReturnKeepHistoryJob.

## SYNTAX

```powershell
Remove-MonitoredJobHistory [-JobId] <Guid>
```

## DESCRIPTION
Elimina la información del historial de todos los Job del registro de monitoreo, a partir del valor DaysReturnKeepHistoryJob.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```powershell
Get-MonitoredServer | Get-MonitoredJobHistory | Remove-MonitoredJobHistory
```

### -------------------------- EXAMPLE 2 --------------------------
```powershell
Get-MonitoredServer | Get-MonitoredJobHistory -Name 'syspolicy_purge_history' | Remove-MonitoredJobHistory
```

## PARAMETERS

### -JobId
Identificador del job que se debe eliminar.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

## INPUTS
Puede canalizar el valor de InputObject desde la función Get-MonitoredJob.

## OUTPUTS
System.Void

## NOTES
Autor: CFranco

## RELATED LINKS

[Get-MonitoredServer](https://github.com/RD-Processa/PSJobMonitor/blob/master/Scripting/getting-started/ConfigServers/Get-MonitoredServer.md)

[Get-MonitoredJobHistory](https://github.com/RD-Processa/PSJobMonitor/blob/master/Scripting/getting-started/GetInfoJobs/Get-MonitoredJobHistory.md)
