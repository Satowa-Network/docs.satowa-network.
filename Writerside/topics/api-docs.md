# API Overview

<!-- This document provides an introduction into your API. -->

## Introduction

Willkommen zu der Satowa Network API Dokumentation. Hier findest du alle Wichtigen Informationen zu
der Offizielle API Dokumentation. Aufgrund dessen das die API derzeit in der Open Beta ist kann es sein
das diese Dokumentation nicht zu 100% richtig ist oder alle Informationen verfügbar sind.

## What you can do using SN API

Die Satowa Network API (kurz SN API) bietet Entwicklern Möglichkeiten wie Meldungen Abrufen, Meldungen erstellen, Transaktionen zu tätigen und viele mehr.

## Authentication

Das Satowa Network verwendet seit Version 4 die ganze Normale HTTP Header Authentifizierung mit dem Authorization header.

## Base URL

https://api.satowa-network.eu

## Rate Limiting

Das Satowa Network verwendet aus Sicherheitsgründen ein Rate-limit.
Man kann mit einer ganzen normalen API Key oder auch ohne nur 10 Anfragen die Minute durchführen bevor man ein Rate-limit bekommt
Sollte man einen Enterprise API Key besitzen, gibt es keine Rate-limiting begrenzungen mehr.

## Error Handling

Wir haben unsere API von anfang an so aufgebaut das man immer eine recht detaillierte Fehlermeldung bekommt. 
Allerdings kann es dazu kommen, dass Fehlermeldungen kommen, die man nicht zu 100 % Verstehen kann. Sollte es interne 
Fehler geben bitten wir darum, uns diese zu melden, auch wenn wir ein Error Reporting System besitzen

**404 Not found**

```JSON
{
  "success": false,
  "error": [
    {
      "message": "Not found",
      "code": 404
    }
  ]
}
```

**200 Success**

Die 200 Statusmeldungen haben immer einen bestimmten wert allerdings ändert sich nichts an der "success" Zeile.
```JSON
{
  "success": true,
  ...
}
```
**500 Internal Server Error**

Die 500 Statusmeldungen sind ein Spezieller fall bei uns diese besitzen in den meisten Fällen folgenden Inhalt:

```JSON
{
  "success": false,
  "error": [
    {
      "message": "Internal Server Error",
      "code": 500
    },
    {
      "message": "...",
      "code": "..."
    }
  ]
}
```
## Versioning

Das Satowa Network besitzt ein Release Day. Der Release Day ist stand 2.11.2023 der 15. Tag des Monats. 
Anders als bei den Projekten vom Satowa Network besitzt die API eine eigene und einfache Art von Versioning.
Das Versioning besteht immer aus dem buchstaben v gefolgt von einer Zahl. Die aktuellste Version ist v4
um eine Version auszuwählen muss bei dem Root Link dann die jeweilige Version angegeben werden.


<seealso>

<!--List any additional resources, such as tutorials or guides, that can help users understand and use the API effectively.-->

</seealso>