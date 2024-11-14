# Endpoints

This section provides detailed documentation for key Trello API endpoints, including their purpose, request structure, parameters, and example responses.

---

## GET /boards/<board_id>
Retrieve details about a specific Trello board.

### Request
```bash
GET https://api.trello.com/1/boards/<board_id>?key=<your_api_key>&token=<your_api_token>
```
### Parameters
| Parameter   | Type   | Required | Description               |
|-------------|--------|----------|---------------------------|
| `board_id`  | string | Yes      | The ID of the Trello board. |
| `key`       | string | Yes      | Your Trello API key.       |
| `token`     | string | Yes      | Your Trello API token.     |

### Example Response
```json
{
  "id": "5a7be6cd1b2abaad456",
  "name": "Project Management",
  "description": "A board for managing projects.",
  "url": "https://trello.com/b/abcdef123"
}
```
---
## POST /cards
Create a new card on a specific Trello list.

### Request
```bash
POST https://api.trello.com/1/cards?key=<your_api_key>&token=<your_api_token>
```
### Parameters
| Parameter   | Type   | Required | Description                           |
|-------------|--------|----------|---------------------------------------|
| `idList`    | string | Yes      | The ID of the list to add the card to.|
| `name`      | string | Yes      | The name of the card.                 |
| `desc`      | string | No       | A description for the card.           |
| `pos`       | string | No       | Position of the card on the list.     |
| `key`       | string | Yes      | Your Trello API key.                  |
| `token`     | string | Yes      | Your Trello API token.                |

### Example Request Body
```json
{
  "idList": "60d21bf01d842c1c23456789",
  "name": "Create API Documentation",
  "desc": "This card is for documenting Trello's API.",
  "pos": "top"
}
```
### Example Response
```json
{
  "id": "60d21bf01d842c1c23456789",
  "name": "Create API Documentation",
  "desc": "This card is for documenting Trello's API.",
  "idList": "60d21bf01d842c1c23456789",
  "url": "https://trello.com/c/abcdef123"
}
```
---
## DELETE /cards/<card_id>
Delete a specific card from a Trello list.

### Request
```bash
DELETE https://api.trello.com/1/cards/<card_id>?key=<your_api_key>&token=<your_api_token>
```
### Parameters
| Parameter   | Type   | Required | Description                     |
|-------------|--------|----------|---------------------------------|
| `card_id`   | string | Yes      | The ID of the card to delete.   |
| `key`       | string | Yes      | Your Trello API key.            |
| `token`     | string | Yes      | Your Trello API token.          |

### Example Response
```json
{
  "id": "60d21bf01d842c1c23456789",
  "status": "deleted"
}
```
---
## Notes

- **Always ensure your `key` and `token` are included in every API request.**
- **Use tools like Postman** to test and debug API calls effectively.
- **Keep your API key and token private** to prevent unauthorized access.
