# Getting Started

## Authentication

The Bearer Token is the authentication method used to authenticate you with our API and should be provided as a bearer token in the authorization header.

```
Authorization: Bearer YOUR_BEARER_TOKEN
```

## Request Example
Here is an example of an API call that demonstrates how to authenticate with the UserPoint API using a Bearer Token and make a request:

```
curl -X GET 'https://useragent.api.volistx.io/lookup' \
-H 'Authorization: Bearer YOUR_BEARER_TOKEN' \
--data-urlencode 'agent=Mozilla/5.0 (iPad; CPU OS 16_5 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/114.0.5735.124 Mobile/15E148 Safari/604.1'
```