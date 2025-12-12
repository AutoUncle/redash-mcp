## Setup

1) Clone the repo and install dependencies:
```sh
git clone git@github.com:autouncle/redash-mcp.git
cd redash-mcp
nvm use 22
npm install
npm run build
```

2) Configure the MCP server entry (example):
```json
"redash-mcp": {
  "command": "node",
  "args": [
    "<full_path>/redash-mcp/dist/cli.js"
  ],
  "env": {
    "REDASH_API_KEY": "api_key",
    "REDASH_URL": "https://redash.autouncle.com",
    "CF_ACCESS_CLIENT_ID": "client_id",
    "CF_ACCESS_CLIENT_SECRET": "client_secret"
  }
}
```

## Credentials
- `REDASH_API_KEY`: Available in your Redash account settings.
- `CF_ACCESS_CLIENT_ID` / `CF_ACCESS_CLIENT_SECRET`: Stored in 1Password under REDASH MCP CF Credentials and shared with everyone
