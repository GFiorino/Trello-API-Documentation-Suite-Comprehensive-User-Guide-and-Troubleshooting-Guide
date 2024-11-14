# Authentication

To use the Trello API, you need to authenticate using an API key and token. Authentication is required for most API requests to ensure security and privacy.

## Step 1: Obtain Your API Key and Token

1. Log in to your Trello account.
2. Navigate to the [Trello API Key page](https://trello.com/app-key).
3. Copy your API key from the displayed page.
4. To generate a token, click "Generate a Token" and follow the instructions.

## Step 2: Include API Key in Requests

When making requests to the Trello API, include your API key and token as query parameters.

**Example:**
```
https://api.trello.com/1/boards/<board_id>?key=<your_api_key>&token=<your_api_token>
```
## Step 3: Example Request
Using curl:
```bash
curl -X GET \
  'https://api.trello.com/1/boards/<board_id>?key=<your_api_key>&token=<your_api_token>'
```
Response:
```json
{
  "id": "5a7be6cd1b2abaad456",
  "name": "Project Management",
  "url": "https://trello.com/b/abcdef123"
}
```
## Notes

- **Keep your API key and token secure.** Do not expose them in public repositories or share them with others.
- **Tokens expire** after a specific period or upon user revocation. If your token stops working, generate a new one from the [Trello API Key page](https://trello.com/app-key).
