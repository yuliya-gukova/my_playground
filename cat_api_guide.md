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
"fact":"Sir Isaac Newton is credited
 with creating the concept for the pet door
that many cats use today to travel outdoors.",
"length":116
}
```

**Fields:**

- fact (string): The random cat fact.
- length (integer): The number of characters in the fact.

## Example Usage

### Using Postman

1. Set the HTTP method to GET.
2. Enter the URL: https://catfact.ninja/fact.
3. Click "Send".
4. You should receive a 200 OK response with a JSON body similar to the example above.

### Using Python

Here is a basic example using the requests library.

```python
import requests

url = "https://catfact.ninja/fact"

response = requests.get(url)

if response.status_code == 200:
    data = response.json()
    print(f"Fact: {data['fact']}")
    print(f"Length: {data['length']}")
else:
    print(f"Error: Received status code {response.status_code}")
```
