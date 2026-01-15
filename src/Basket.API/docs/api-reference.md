# API Reference

This section provides a detailed reference for the Basket API endpoints.

## Get Basket

- **Endpoint:** `GET /api/v1/basket/{id}`
- **Description:** Retrieves the shopping basket for a given user ID.
- **Parameters:**
  - `id` (string, path): The ID of the user.
- **Responses:**
  - `200 OK`: Returns the user's basket.
  - `404 Not Found`: If the user or basket is not found.

## Update Basket

- **Endpoint:** `POST /api/v1/basket/{id}`
- **Description:** Updates the shopping basket for a given user ID.
- **Parameters:**
  - `id` (string, path): The ID of the user.
- **Request Body:**
  - A JSON object representing the items to be updated in the basket.
- **Responses:**
  - `200 OK`: Returns the updated basket.

## Delete Basket

- **Endpoint:** `DELETE /api/v1/basket/{id}`
- **Description:** Deletes the shopping basket for a given user ID.
- **Parameters:**
  - `id` (string, path): The ID of the user.
- **Responses:**
  - `200 OK`: If the basket was successfully deleted.
