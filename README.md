<div align="center">
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT3HkrFkToxF0Hgrq_-LdbaUvDcHcNehHhQug&s" />
</div>

Per installare agent Zabbix e puntarlo a 145.14.161.84

```
irm https://raw.githubusercontent.com/Omegatech-Srl/Zabbix-Windows/main/InstallazioneZabbixAgent.ps1 | iex
```

Su Windows server >2016 è necessario forzare l'utilizzo di TLS 1.2 con il comando sotto prima di eseguire lo sript d'installazione dell'agent
```
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12
```
