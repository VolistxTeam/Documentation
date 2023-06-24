# User Agent Generation

This endpoint allows you to generate a random user agent.

Request

- HTTP Method: GET
- Path: `/generate`
- Query Parameters:
    - `type` (optional): The type of user agent to generate. If not provided, a random user agent will be generated.
    - `callback` (optional): A callback function name for JSONP support.

The type parameter allows you to specify the type of user agent you want to generate. Here are the supported values and their explanations:

- `firefox`: Simulates the Mozilla Firefox web browser.
- `chrome`: Simulates the Google Chrome web browser.
- `safari`: Simulates the Apple Safari web browser.
- `opera`: Simulates the Opera web browser.
- `ie`: Simulates Microsoft Internet Explorer (IE) web browser.
- `windows`: Simulates a web browser on the Windows operating system.
- `mac`: Simulates a web browser on the macOS operating system.
- `iphone`: Simulates a web browser on an iPhone device.
- `android`: Simulates a web browser on an Android device.

You can use the type parameter to generate user agent strings that mimic the behavior of specific browsers or platforms. This can be useful for tasks like testing website compatibility, analyzing user agent statistics, or creating browser-specific experiences.

Response

The response will contain the generated user agent.

```json
{
  "agent": "Mozilla/5.0 (Macintosh; PPC Mac OS X 10_7_5) AppleWebKit/532.0 (KHTML, like Gecko) Chrome/88.0.4788.53 Safari/532.0 Edg/88.01084.51"
}
```