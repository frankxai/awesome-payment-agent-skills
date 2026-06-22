# Contributing to Awesome Payment Agent Skills

Thank you for your interest in contributing! This list aims to be the best curated resource for AI agent payment skills, protocols, and toolkits. Please follow these guidelines to keep the list high quality.

## What belongs here

- **Agent skills** (`SKILL.md` format or equivalent) that teach agents how to handle payments
- **Payment protocols** that move value between agents, services, or machines — open specifications with public repos
- **Commerce protocols** for agent-driven product discovery, cart management, and checkout
- **Provider SDKs and toolkits** from payment processors, wallet providers, or networks with agent-specific functionality
- **MCP servers** that expose payment capabilities as agent tools
- **Identity and trust protocols** for verifying agent identity, spend authorization, or transaction integrity
- **Examples and templates** with working reference implementations of the above

## What doesn't belong here

- Closed-source tools with no developer API or SDK
- General-purpose payment libraries with no agentic or AI-agent-specific capability
- Abandoned projects (last commit > 2 years ago, unless seminal)
- Marketing pages, blog posts, or whitepapers without an accompanying code artifact
- Wallets, exchanges, or payment processors with no documented agent integration path

## Format

Follow the existing style for each entry:

```markdown
- [Tool Name](https://url) - Short description. Maximum two sentences. Trailing period.
```

- Use `- [Name](url) - Description.` — single dash, no bold, trailing period.
- Keep descriptions to one or two sentences that say what the tool does and why it matters for agent payments.
- Place entries alphabetically within each section when possible.
- Do not add language/platform badges — entries here are protocols and SDKs spanning many languages.

## Pull request process

1. Fork the repo and create a feature branch.
2. Add your entry in the correct section.
3. Verify all links are live and correct.
4. Check that your description passes `npx awesome-lint` with zero warnings.
5. Open a pull request with a brief description of what you're adding and why it belongs here.

## Updating an existing entry

If a tool has been significantly updated, renamed, or its URL has changed, open a PR with the correction and a note explaining the change.

## Attribution

This list is licensed under [CC0-1.0](license). Contributions are accepted on the same terms — no copyright claim, freely shareable.
