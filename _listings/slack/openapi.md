swagger: "2.0"
x-collection-name: Slack
x-complete: 1
info:
  title: Slack
  description: one-way-to-interact-with-the-slack-platform-is-its-http-rpcbased-web-api-a-collection-of-methods-requiring-oauth-2-0based-user-bot-or-workspace-tokens-blessed-with-related-oauth-scopes-
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /emoji.list:
    get:
      summary: List Emojis
      description: Lists custom emoji for a team.
      operationId: emoji_list
      x-api-path-slug: emoji-list-get
      parameters:
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Emoji