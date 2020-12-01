# List GPT-3 Engines

```sh
curl https://api.openai.com/v1/engines -H "Authorization: Bearer $OPENAI_API_KEY"
```

{
  "object": "list",
  "data": [
    {
      "id": "ada",
      "object": "engine",
      "owner": "openai",
      "ready": true
    },
    {
      "id": "babbage",
      "object": "engine",
      "owner": "openai",
      "ready": true
    },
    {
      "id": "content-filter-alpha-c4",
      "object": "engine",
      "owner": "openai",
      "ready": true
    },
    {
      "id": "content-filter-dev",
      "object": "engine",
      "owner": "openai",
      "ready": true
    },
    {
      "id": "curie",
      "object": "engine",
      "owner": "openai",
      "ready": true
    },
    {
      "id": "cursing-filter-v6",
      "object": "engine",
      "owner": "openai",
      "ready": true
    },
    {
      "id": "davinci",
      "object": "engine",
      "owner": "openai",
      "ready": true
    }
  ]
}

## Getting a specific engine details
GET https://api.openai.com/v1/engines/{engine_id}

```sh
curl https://api.openai.com/v1/engines/ada -H "Authorization: Bearer $OPENAI_API_KEY"
```