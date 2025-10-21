п# Getting a Random Cat Fact

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
"fact":"Sir Isaac Newton is credited
 with creating the concept for the pet door
that many cats use today to travel outdoors.",
"length":116}
}
```

· fact (string): The random cat fact.
· length (integer): The number of characters in the fact.
