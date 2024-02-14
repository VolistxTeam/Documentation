# Getting Started
## Authentication

The Bearer Token is the authentication method used to authenticate you with our API and should be provided as a bearer token in the authorization header.

```
Authorization: Bearer YOUR_BEARER_TOKEN
```

## Request Example
Here is an example of an API call that demonstrates how to authenticate with the LingoPoint API using a Bearer Token and make a request:

```
curl -G 'https://lingopoint.api.volistx.io/lookup' \
-H 'Authorization: Bearer YOUR_BEARER_TOKEN' \
--data-urlencode 'text=In a world where technology and innovation intertwine, the journey towards discovering new horizons is endless. As we navigate through the complexities of modern life, our pursuit of knowledge and understanding becomes the beacon guiding us towards a brighter future.'
```