# API Quickstart

<!-- This document describes how to start using your API: authorization, authentication, accessing API resources. -->
In diesem Abschnitt finden Sie eine Schritt-für-Schritt-Anleitung für den schnellen Einstieg in die Nutzung der API.

## Authentication

Our API is structured in such a way that for most requests that are not POST, PUT, DELETE, OPTION methods no
API key is required. However, certain endpoints such as querying user and wallet data with a special agent
or user API key are mandatory.
If you need an API key, please contact us at the following e-mail: [dev@satowa-network.eu](mailto:dev@satowa-network.eu)

If you already have an API key and need it, it must be included in your header in the "Authorization" header tag.
## Making Your First Request

If you want to try out the API, you can easily test it by trying to receive our messages.
Simply use the following:

```http
GET /v4/reports HTTP/1.1
Host: api.satowa-network.eu
Authorization: YOUR_ACCESS_TOKEN
```

## Response Handling

If you send us a request, we will always reply in JSON format, this JSON format can differ from status code to status code
See [api-docs.md](api-docs.md)

<!--## API Usage Tips
Offer tips and best practices for using the API effectively and efficiently.

## Next Steps
Suggest what users can do next, such as exploring more endpoints or integrating the API into their applications.-->