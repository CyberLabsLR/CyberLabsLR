## Inhaltsverzeichnis

1. [Deploy](#deploy)
   - [Log Analytics Workspace erstellen](#log-analytics-workspace-erstellen)
   - [LAW zu Sentinel hinzufügen](#law-zu-sentinel-hinzufügen)
2. [Ingest Data](#ingest-data)
3. [Detect](#detect)
4. [Investigate](#investigate)
5. [Fazit](#fazit)


# Microsoft Sentinel Lab
Microsoft Sentinel ist eine cloudbasierte Sicherheitslösung von Microsoft, welche SIEM (Security Information and Event Management) mit SOAR (Security Orchestration, Automation and Response) kombiniert. Die Plattform sammelt und analysiert Logs aus verschiedenen Quellen wie Servern, Clients, Anwendungen, EntraID und Cloud-Apps. Dadurch erhält ein Unternehmen einen zentralen Überblick über ihre IT-Sicherheitsumgebung. Durch automatisierte Workflows, sogenannte Playbooks, lassen sich bestimmte Reaktionen auf Sicherheitsvorfälle automatisieren. Microsoft Sentinel unterstützt somit Security Operations Center (SOC)-Teams dabei, Bedrohungen schneller zu erkennen, effizienter zu analysieren und angemessen darauf zu reagieren.

## Deploy
Ein Log Analytics Workspace (LAW) ist ein zentraler Speicherort für Logdaten. Mit der Kusto Query Language (KQL) können diese Logdaten gezielt abgefragt und analysiert werden. Damit können verdächtige Aktivitäten und mögliche Sicherheitsbedrohungen erkannt werden. Der Log Analytics Workspace bildet also die Datengrundlage von Sentinel.

### Log Analytics Workspace erstellen
Search bar > "Microsoft Sentinel" eingeben > 	Create new Workspace

<p align="center">
  <img src="images/Deploy_LAW_01.png" width="60%">
  <br>
  <em>LAW erstellen</em>
</p>

### LAW zu Sentinel hinzufügen
Den gerade erstellen LAW auswählen und auf "Add" klicken. Anschliessend wird unter "General" > "Overview" die aktuellen Events, Alerts und Incidents angezeigt (auf meinem Screenshot wird nichts angezeigt, weil der LAW gerade erst erstellt wurde).

<p align="center">
  <img src="images/Deploy_LAW_Sentinel_02.png" width="60%">
  <br>
  <em>LAW zu Sentinel hinzufügen</em>
</p>

Damit wurde die Grundlage für den Einsatz von Microsoft Sentinel geschaffen. Durch die Verknüpfung des Log Analytics Workspace mit Sentinel können zukünftig Sicherheitsdaten zentral gesammelt, analysiert und überwacht werden. Im nächsten Schritt müssen entsprechende Datenquellen (Dataconnectors) angebunden werden, damit Sentinel sicherheitsrelevante Ereignisse erfassen und mögliche Bedrohungen erkennen kann.

## Ingest Data

## Detect

## Investigate

## Fazit
