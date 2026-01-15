# Getting Started with the Basket API

This tutorial will guide you through the process of making your first API calls to the Basket API.

## Prerequisites

- An API client (e.g., Postman, curl).
- A valid authentication token.

## Step 1: Get your User ID

First, you need to have a user ID. For this tutorial, we will use `test-user`.

## Step 2: Add items to your basket

To add items to your basket, you need to make a POST request to the `/api/v1/basket/test-user` endpoint with a request body containing the items.

```bash
curl -X POST \
  http://<your-api-gateway>/api/v1/basket/test-user \
  -H 'Content-Type: application/json' \
  -d '{
    "items": [
      {
        "productId": "prod-123",
        "quantity": 2
      }
    ]
  }'
```

## Step 3: Retrieve your basket

To retrieve your basket, make a GET request to the `/api/v1/basket/test-user` endpoint.

```bash
curl http://<your-api-gateway>/api/v1/basket/test-user
```

You should receive a response containing the items you added in the previous step.
