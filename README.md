# AI Visibility

See how ChatGPT, Gemini, Google AI Overviews, Google AI Mode, Perplexity, Claude, Grok and DeepSeek
describe a product. Your agent gets the answers and the sources they cite, finds what's keeping the
product out of those answers, makes the fix in your repo, and verifies it on the live site.

This repo holds the agent skill and the connection settings for the remote MCP server at
`https://mcp.aivisibilityskill.com/mcp`.

## Install

| Client                    | How                                                                                                       |
| ------------------------- | --------------------------------------------------------------------------------------------------------- |
| Claude Code               | `/plugin marketplace add aivisibilityskill/plugin`, then `/plugin install aivisibility@aivisibilityskill` |
| Claude Code (server only) | `claude mcp add --transport http aivisibility https://mcp.aivisibilityskill.com/mcp`                      |
| Codex                     | `codex mcp add aivisibility --url https://mcp.aivisibilityskill.com/mcp`                                  |
| Others                    | Add a custom MCP server with the URL above                                                                |

Your client opens a browser so you can sign in and approve the connection.

## What's sent

The server receives the product name, domains, competitors and buyer questions your agent gives it.
It sends those questions to AI and search providers and reads public pages. This plugin has no hooks
or scripts, and it never reads your code or sends it anywhere.

## Credits

Requires an aivisibilityskill.com account. Some tools use credits from your account; the account,
estimate and results tools don't.

## Links

- Docs: https://api.aivisibilityskill.com/docs
- Privacy: https://aivisibilityskill.com/privacy
- Terms: https://aivisibilityskill.com/terms
- Support: support@aivisibilityskill.com
