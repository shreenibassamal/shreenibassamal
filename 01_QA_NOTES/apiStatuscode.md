## 1xx – Informational Responses
|   Code | Meaning                         | When It Occurs                                   | Example                                 |
| ------:| --------------------------------| ------------------------------------------------ | --------------------------------------- |
|    100 | Continue                        | Server received headers; client continues.       | Uploading large files in chunks.       |
|    101 | Switching Protocols             | Switching to a new protocol as requested.        | WebSocket upgrade request.             |
|    102 | Processing                      | Request accepted but still processing.           | WebDAV long requests.                  |
|    103 | Early Hints                     | Preload resources before full response.          | Preload headers for HTML.              |

## 2xx – Success Responses
|   Code | Meaning                         | When It Occurs                                   | Example                                 |
| ------:| --------------------------------| ------------------------------------------------ | --------------------------------------- |
|    200 | OK                              | Request succeeded; returns data.                 | `GET /users` fetches user list.        |
|    201 | Created                         | Resource successfully created.                   | `POST /users` creates a user.          |
|    202 | Accepted                        | Request accepted, processing later.              | Async file processing.                 |
|    203 | Non-Authoritative Information   | Data modified by proxy or third-party.           | Cached API response.                   |
|    204 | No Content                      | Request successful; no data to return.           | `DELETE /user/123` success.            |
|    205 | Reset Content                   | Request successful; reset form/UI.               | Form submission reset.                 |
|    206 | Partial Content                 | Partial response for range request.              | Video streaming.                       |
|    207 | Multi-Status                    | Multiple statuses in one response.               | WebDAV batch response.                 |
|    208 | Already Reported                | Already included earlier.                        | WebDAV operations.                     |
|    226 | IM Used                         | GET fulfilled using delta encoding.              | Delta updates.                         |

## 3xx – Redirection
|   Code | Meaning                         | When It Occurs                                   | Example                                 |
| ------:| --------------------------------| ------------------------------------------------ | --------------------------------------- |
|    300 | Multiple Choices                | Multiple options for resource.                   | Different image sizes.                  |
|    301 | Moved Permanently               | Resource moved to new URL permanently.           | HTTP → HTTPS redirect.                  |
|    302 | Found (Temp Redirect)           | Temporary redirect.                              | Login redirect.                         |
|    303 | See Other                       | Redirect with GET method.                        | Payment success → order page.           |
|    304 | Not Modified                    | Cached version valid.                            | Browser cache check.                    |
|    305 | Use Proxy                       | Access via proxy only (deprecated).              | Rarely used.                            |
|    307 | Temporary Redirect              | Temporary redirect; method preserved.            | API routing.                            |
|    308 | Permanent Redirect              | Permanent redirect; method preserved.            | Resource permanently moved.             |

## 4xx – Client Errors
|   Code | Meaning                         | When It Occurs                                   | Example                                 |
| ------:| --------------------------------| -------------------------------------------------| --------------------------------------- |
|    400 | Bad Request                     | Invalid syntax in request.                       | Missing parameter in API.               |
|    401 | Unauthorized                    | Authentication required/failed.                  | Missing API key.                        |
|    402 | Payment Required                | Reserved for payment use.                        | Paid service access.                    |
|    403 | Forbidden                       | Access denied even if authenticated.             | No admin rights.                        |
|    404 | Not Found                       | Resource not found.                              | `GET /user/9999` missing.               |
|    405 | Method Not Allowed              | Method not supported.                            | `POST` where only `GET` allowed.        |
|    406 | Not Acceptable                  | Format not acceptable.                           | Client wants XML but only JSON exists.  |
|    407 | Proxy Authentication Required   | Must authenticate with proxy.                    | Corporate proxy login.                  |
|    408 | Request Timeout                 | Request took too long.                           | Slow internet timeout.                  |
|    409 | Conflict                        | Conflict with current state.                     | Updating outdated record.               |
|    410 | Gone                            | Resource permanently removed.                    | Old product page.                       |
|    411 | Length Required                 | Content-Length header missing.                   | Upload without size header.             |
|    412 | Precondition Failed             | Preconditions not met.                           | If-Match header mismatch.               |
|    413 | Payload Too Large               | Request too large.                               | 1GB file upload on 10MB limit.          |
|    414 | URI Too Long                    | URL too long.                                    | Huge query string.                      |
|    415 | Unsupported Media Type          | Unsupported content type.                        | XML instead of JSON.                    |
|    416 | Range Not Satisfiable           | Invalid range.                                   | Video seek out of range.                |
|    417 | Expectation Failed              | Cannot meet Expect header.                       | Rarely used.                            |
|    418 | I’m a Teapot                    | Joke code.                                       | Easter egg in APIs.                     |
|    421 | Misdirected Request             | Sent to wrong server.                            | Load balancer error.                    |
|    422 | Unprocessable Entity            | Semantic error.                                  | Invalid email in JSON.                  |
|    423 | Locked                          | Resource locked.                                 | Editing locked file.                    |
|    424 | Failed Dependency               | Dependent request failed.                        | Chained API request failed.             |
|    425 | Too Early                       | Request sent too early.                          | HTTP/2 early data.                      |
|    426 | Upgrade Required                | Upgrade protocol required.                       | Force HTTPS.                            |
|    428 | Precondition Required           | Precondition headers required.                   | Conditional request missing.            |
|    429 | Too Many Requests               | Rate limit exceeded.                             | API throttling.                         |
|    431 | Request Header Too Large        | Headers too large.                               | Excessive cookies.                      |
|    451 | Unavailable for Legal Reasons   | Blocked for legal reasons.                       | Government censorship.                  |

## 5xx – Server Errors
|   Code | Meaning                         | When It Occurs                                   | Example                                 |
| ------:| --------------------------------| -------------------------------------------------| --------------------------------------- |
|    500 | Internal Server Error           | Generic server error.                            | Code crash.                             |
|    501 | Not Implemented                 | Server does not support feature.                 | API not ready.                          |
|    502 | Bad Gateway                     | Invalid upstream response.                       | Reverse proxy error.                    |
|    503 | Service Unavailable             | Server overloaded or down.                       | Maintenance mode.                       |
|    504 | Gateway Timeout                 | Upstream server timeout.                         | API timeout.                            |
|    505 | HTTP Version Not Supported      | Unsupported HTTP version.                        | Old HTTP/0.9 request.                   |
|    506 | Variant Also Negotiates         | Configuration error.                             | Content negotiation loop.               |
|    507 | Insufficient Storage            | Server out of space.                             | File upload failed.                     |
|    508 | Loop Detected                   | Infinite loop detected.                          | WebDAV loop.                            |
|    510 | Not Extended                    | Extensions required.                             | Custom extension issue.                 |
|    511 | Network Authentication Required | Network authentication needed.                   | WiFi portal login.                      |
----------------------------------------------------------------------------------------------------------------------------------------
