# Brightcove Analytics API Sample: Unique Users Per Day

This sample demonstrates how to retrieve the number of unique users per day using the Brightcove Analytics API.

## Prerequisites

- A [Brightcove API account](https://studio.brightcove.com/products/analytics-api.html)
- API credentials with access to the Analytics API
- A tool for making API requests, such as:
  - [Postman](https://www.postman.com/)
  - `curl`
  - A programming language like JavaScript (Node.js) or Python

## API Request

### Endpoint

```plaintext
GET https://analytics.api.brightcove.com/v1/data
```

### Query Parameters

| Parameter     | Description                                      | Example |
|--------------|--------------------------------------------------|---------|
| `accounts`   | Brightcove account ID                           | `1234567890` |
| `dimensions` | Data aggregation dimension                      | `date` |
| `fields`     | Metrics to retrieve                             | `video_view,unique_users` |
| `from`       | Start date (ISO 8601 format or relative date)  | `2024-01-01` |
| `to`         | End date (ISO 8601 format or relative date)    | `2024-01-31` |

### Example Request

#### Using `curl`

```bash
curl -X GET \
  "https://analytics.api.brightcove.com/v1/data?accounts=1234567890&dimensions=date&fields=video_view,unique_users&from=2024-01-01&to=2024-01-31" \
  -H "Authorization: Bearer YOUR_ACCESS_TOKEN"
```

#### Using JavaScript (Node.js)

```javascript
const fetch = require('node-fetch');

const url = "https://analytics.api.brightcove.com/v1/data?accounts=1234567890&dimensions=date&fields=video_view,unique_users&from=2024-01-01&to=2024-01-31";
const options = {
  method: 'GET',
  headers: {
    'Authorization': 'Bearer YOUR_ACCESS_TOKEN'
  }
};

fetch(url, options)
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error:', error));
```

#### Using Python

```python
import requests

url = "https://analytics.api.brightcove.com/v1/data"
params = {
    "accounts": "1234567890",
    "dimensions": "date",
    "fields": "video_view,unique_users",
    "from": "2024-01-01",
    "to": "2024-01-31"
}
headers = {
    "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}

response = requests.get(url, headers=headers, params=params)
print(response.json())
```

## Response

A successful response returns a JSON object:

```json
{
  "account": "1234567890",
  "dimension": "date",
  "items": [
    {
      "date": "2024-01-01",
      "video_view": 150,
      "unique_users": 120
    },
    {
      "date": "2024-01-02",
      "video_view": 200,
      "unique_users": 170
    }
  ]
}
```

## Error Handling

If there is an error, the response will include an error message:

```json
{
  "error_code": "INVALID_AUTHENTICATION",
  "message": "Invalid access token"
}
```

Ensure that:
- The access token is valid and not expired.
- The API request syntax is correct.
- The account has permissions to access the requested data.

## Additional Resources

- [Brightcove Analytics API Reference](https://apis.support.brightcove.com/analytics/)
- [OAuth Authentication Guide](https://apis.support.brightcove.com/oauth/)

