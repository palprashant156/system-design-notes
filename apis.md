# APIs (Application Programming Interfaces)

An **API** is a defined way for software systems to communicate. It describes what a client can ask a service to do, what information to send, and what response to expect. The API acts as a contract between the client and the service, so the client does not need to know how the service is implemented internally.

## Example: Get a user's profile

A web or mobile app can call an HTTP API to retrieve a user's profile:

```http
GET /api/users/42 HTTP/1.1
Host: example.com
Accept: application/json
```

The server might respond with:

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": 42,
  "name": "Ava Patel"
}
```

Here, `GET` is the operation, `/api/users/42` identifies the requested resource, and the JSON body contains the result. The API also communicates outcomes through status codes—for example, `404 Not Found` if that user does not exist.
