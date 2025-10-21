# Getting a Random Cat Fact

This guide explains how to use the `GET /fact` endpoint to retrieve a random fact about cats.

## Base URL

All requests should be made to:
```

https://catfact.ninja

```

## Endpoint: `GET /fact`

Returns a single, random cat fact.

### HTTP Request

```

GET https://catfact.ninja/fact

```

### Parameters

This endpoint does not require any parameters.

### Response

#### Success Response

**Code:** `200 OK`

**Body:**
The response body is a JSON object containing the fact and its length.

```json
{
  "fact": "A cat has the ability to rotate its ears 180 degrees.",
  "length": 57
}
```

· fact (string): The random cat fact.
· length (integer): The number of characters in the fact.
