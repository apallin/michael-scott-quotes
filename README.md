# michael-scott-quotes
A simple node.js service for serving Michael Scott quotes via an API

Adapted from [a Ron Swanson quote API](https://github.com/jamesseanwright/ron-swanson-quotes)

## Production host

[https://michael-scott-api.herokuapp.com/v1/quotes](http:///michael-scott-api.herokuapp.com/v1/quotes)

The `Access-Control-Allow-Origin` header is set to `*` so that you can make requests from any domain.

## APIs

### `GET /v1/quotes`

Returns an array with one quote:

```json
[
    "Thats what she said."
]
```

### `GET /v1/quotes/<count>`

Returns an array with `<count>` quotes e.g. `GET /quotes/2`

```json
[
    "Thats what she said.",
    "I am Beyoncé, always."
]
```

## OpenAPI 3 Schema

An [OpenAPI](https://swagger.io/docs/specification/about/) 3 schema is available at `/v1/schema`.
