# API Overview

<!-- This document provides an introduction into your API. -->

## Introduction

Welcome to the Satowa Network API documentation. Here you will find all important information about
the official API documentation. Due to the fact that the API is currently in open beta it is possible
that this documentation is not 100% correct or that all information is available.

## What you can do using SN API

The Satowa Network offers developers and other networks, social media servers and many more the possibility to work with us and thus create a network full of trust and possibilities to work together.
Since the release of API version 4, the Satowa Network also has its own transaction system. With this system it is possible to create and receive transactions and other important requests.

## Authentication

Since version 4, the Satowa Network uses the entire normal HTTP header authentication with the Authorization header.
## Base URL

https://api.satowa-network.eu

## Rate Limiting

The Satowa Network uses a rate limit for security reasons.
You can make only 10 requests per minute with or without a normal API key before you get a rate limit
If you have an Enterprise API Key, there are no more rate-limiting restrictions.

## Error Handling

We have built our API from the beginning so that you always get a very detailed error message.
However, there may be error messages that you cannot understand 100%. If there are internal
errors, please report them to us, even if we have an error reporting system

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

The 200 status messages always have a certain value, but nothing changes in the "success" line.
```JSON
{
  "success": true,
  ...
}
```
**500 Internal Server Error**

The 500 status messages are a special case for us and in most cases have the following content:

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

The Satowa Network has a release day. The release day is the 15th day of the month as of 08.01.2024.
Unlike the Satowa Network projects, the API has its own, simple type of versioning.
The versioning always consists of the letter v followed by a number. The latest version is v4
To select a version, the respective version must be specified in the root link.


<seealso>

<!--List any additional resources, such as tutorials or guides, that can help users understand and use the API effectively.-->

</seealso>