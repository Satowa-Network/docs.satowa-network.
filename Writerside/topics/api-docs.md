# API Overview

<!-- This document provides an introduction into your API. -->

## Introduction

Provide a brief introduction to the API, explaining its purpose and scope.

## What you can do using SN API

Die Satowa Network API (kurz SN API) bietet Entwicklern Möglichkeiten wie Meldungen Abrufen, Meldungen erstellen, Transaktionen zu tätigen und viele mehr.

## Authentication

Das Satowa Network verwendet seit Version 4 die ganze Normale HTTP Header Authentifizierung mit dem Authorization header.

## Base URL

https://api.satowa-network.eu

## Rate Limiting

Das Satowa Network verwendet aus Sicherheitsgründen ein Rate-limit.
Man kann mit einer ganzen normalen API Key oder auch ohne nur 10 Anfragen die Minute durchführen bevor man ein Rate Limit bekommt
Sollte man einen Enterprise API Key besitzen, gibt es keine Rat Limiting begrenzungen mehr.

## Error Handling

Sollte ein Fehler aufkommen sollte bei bestimmten Fehlermeldungen eine bestimmte JSON Response zurück gegeben werden. 

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
Um eine Version auszuwählen muss bei dem Root Link dann die jeweilige Version angegeben werden.


<seealso>

<!--List any additional resources, such as tutorials or guides, that can help users understand and use the API effectively.-->

</seealso>