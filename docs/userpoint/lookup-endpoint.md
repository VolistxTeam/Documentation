# User Agent Lookup

This endpoint allows you to retrieve information about a user agent.

Request

- HTTP Method: GET
- Path: `/lookup`
- Query Parameters:
    - `agent` (required): The user agent string to lookup.
    - `callback` (optional): A callback function name for JSONP support.

Response

The response will contain information about the user agent.

Example Response:
```json
{
  "agent": "Mozilla/5.0 (iPad; CPU OS 16_5 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/114.0.5735.124 Mobile/15E148 Safari/604.1",
  "type": {
    "mobile": false,
    "tablet": true,
    "pc": false,
    "tv": false,
    "camera": false,
    "bot": false
  },
  "os": {
    "name": "iPadOS",
    "wiki": "https://en.wikipedia.org/wiki/IPadOS",
    "version": "16.5",
    "platform": "",
    "icon": "https://cdn.volistx.io/userpoint/icons/os/ipados.png"
  },
  "browser": {
    "name": "Chrome Mobile iOS",
    "family": "Chrome",
    "version": {
      "full": "114.0.5735.124",
      "major": "114",
      "minor": "0",
      "patch": "5735"
    },
    "engine": "WebKit"
  },
  "device": {
    "brand": {
      "name": "Apple",
      "wiki": "https://en.wikipedia.org/wiki/Apple_Inc.",
      "icon": "https://cdn.volistx.io/userpoint/icons/brands/apple.png",
      "website": "https://www.apple.com/"
    },
    "model": "iPad"
  },
  "bot": null
}
```

In the event that it's identified as a bot, the following response will be appended:

```json
"bot": {
  "category": "Search bot",
  "name": "Googlebot",
  "url": "http://www.google.com/bot.html",
  "producer": {
    "name": "Google Inc.",
    "url": "http://www.google.com"
  }
}
```