# API Quickstart

<!-- This document describes how to start using your API: authorization, authentication, accessing API resources. -->
In this section, you'll find a step-by-step guide to quickly start using the API.

## Authentication

Unsere API ist für Entwickler die, die API nur Verwenden um Daten abzurufen wie Melden ist ohne einem API Key aufrufbar.
Allerdings ist ein API Key verpflichtend, wenn es um private Daten geht oder POST, OPTION, PUT Anfragen gesendet werden

Solltest du ein API Key brauchen wende dich bitte an uns unter der folgenden E-Mail: [dev@satowa-network.eu](mailto:dev@satowa-network.eu)

Solltest du bereits eine API Key besitzen und die benötigst diese muss diese in deinem Header im "Authorization" Header Tag stehen.

## Making Your First Request

Wenn du die API ausprobieren willst, kannst du diese ganz einfach austesten, indem du versuchst unsere Meldungen zu erhalten.
Verwende dazu einfach folgendes:

```http
GET /v4/reports HTTP/1.1
Host: api.satowa-network.eu
Authorization: YOUR_ACCESS_TOKEN
```

## Response Handling

Alle ausgaben, sind im JSON Format. Diese sind ganz einfach zu Verwenden.

<!--## API Usage Tips
Offer tips and best practices for using the API effectively and efficiently.

## Next Steps
Suggest what users can do next, such as exploring more endpoints or integrating the API into their applications.-->