# Errors

All errors will include a message attribute detailing the error message.

```json
{
  "error": {
    "type": "Unauthorized",
    "info": "You have insufficient permissions to access this resource."
  }
}
```

The UserPoint API uses the following error types:

| Error Codes | Meaning                                                          |
|-------------|------------------------------------------------------------------|
| InvalidParameter | The request contains invalid parameters.                   |
| Unauthorized | The request requires authentication.                       |
| Forbidden | The server understood the request, but the access is restricted. |
| NotFound | The requested resource could not be found.                   |
| Conflict | The request conflicts with the current state of the server.  |
| RateLimitReached | The user has exceeded the allowed number of requests.      |
| Unknown | An unknown error occurred.                                  |

The UserPoint API comes with HTTP status code:

| Error Codes | Meaning                                                          |
|-------------|------------------------------------------------------------------|
| 400         | Bad Request - Invalid parameters                                 |
| 401         | Unauthorized - Unable to authenticate, use valid bearer token.   |
| 403         | Forbidden - The request is not allowed.                          |
| 404         | Not Found - The specified resource could not be found.           |
| 406         | Not Acceptable - You requested a format that isn't json.         |
| 429         | Too Many Requests - You have reached the rate limit.             |
| 500         | Internal Server Error - We had a problem with our server.        |
| 503         | Service Unavailable - We're temporarily offline for maintenance. |
