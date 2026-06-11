# Awesome Payment Agent Skills [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Agent skills, protocols, SDKs, and MCP servers that let AI agents pay, get paid, and transact.

AI agents are becoming economic actors: they buy API calls, subscribe to services, check out shopping carts, and charge for their own work. This list curates the best building blocks for that agentic economy — from HTTP 402 micropayment protocols and card-network mandates to provider toolkits, Model Context Protocol servers, and installable agent skills.

## Contents

- [Agent Skills](#agent-skills)
- [Payment Protocols](#payment-protocols)
- [Commerce Protocols](#commerce-protocols)
- [Provider Toolkits and SDKs](#provider-toolkits-and-sdks)
- [MCP Servers](#mcp-servers)
- [Identity and Trust](#identity-and-trust)
- [Examples and Templates](#examples-and-templates)
- [Resources](#resources)

## Agent Skills

Installable skills (Claude Agent Skills `SKILL.md` format and similar) that teach agents how to handle money.

- [Anthropic Agent Skills](https://github.com/anthropics/skills) - Official skills registry and `SKILL.md` specification that payment skills build on.
- [Lightning Agent Tools](https://github.com/lightninglabs/lightning-agent-tools) - Seven composable Claude Code skills plus an MCP server for running Lightning nodes, paying for APIs over L402, hosting paid endpoints, and managing macaroon credentials.
- [Shopify UCP CLI](https://github.com/Shopify/ucp-cli) - Shopping skill for AI agents powered by the Universal Commerce Protocol, with discovery, cart, and checkout flows.
- [Skyfire Skills](https://github.com/skyfire-xyz/skills) - Skyfire agent skills for identity-verified, JWT token-based agent payments.
- [Stripe Skills](https://github.com/stripe/ai/tree/main/skills) - Official Stripe Claude Code skills (`stripe-best-practices`, `stripe-directory`, `stripe-projects`, `upgrade-stripe`) for building and upgrading Stripe integrations.
- [xpay CLI](https://github.com/xpaysh/cli) - CLI for discovering and installing x402 payment skills for AI agents.

## Payment Protocols

Open protocols that move money between agents, services, and machines.

- [x402](https://github.com/x402-foundation/x402) - Internet-native payments over the HTTP `402 Payment Required` status code, stewarded by the x402 Foundation with founding members including Visa, Mastercard, Stripe, Google, Cloudflare, and Coinbase.
- [AP2](https://github.com/google-agentic-commerce/AP2) - Google's Agent Payments Protocol using signed payment mandates to authorize agent-initiated payments across cards, account-to-account rails, and digital assets.
- [a2a-x402](https://github.com/google-agentic-commerce/a2a-x402) - Extension bringing x402 on-chain payments to the Agent2Agent (A2A) protocol so agents can monetize their services.
- [H402](https://github.com/bit-gpt/h402) - Independent HTTP 402 machine-to-machine payment protocol for APIs, compute, and data.
- [KYAPay](https://github.com/skyfire-xyz/kyapay) - Know-Your-Agent + Pay protocol combining verified agent identity with JWT token-based payments, no wallets or gas required.
- [KYAPay A2A Extension](https://github.com/skyfire-xyz/kyapay_a2a) - Skyfire's KYA+PAY payment extension for A2A agents.
- [L402](https://github.com/lightninglabs/L402) - Lightning Network HTTP 402 protocol pairing invoices with macaroon bearer credentials, the original revival of `402 Payment Required`.
- [L402 SDK](https://github.com/lightninglabs/L402sdk) - L402 client SDK for AI agent frameworks to pay for APIs with Lightning.

## Commerce Protocols

Protocols for agent-driven product discovery, carts, and checkout.

- [Agentic Commerce Protocol](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol) - Open standard maintained by OpenAI and Stripe connecting buyers, their AI agents, and businesses, including the Agentic Checkout and Delegate Payment specs.
- [Universal Commerce Protocol](https://github.com/Universal-Commerce-Protocol/ucp) - Specification by Google, Shopify, and partners for agent catalog discovery, cart negotiation, and purchase.
- [UCP JavaScript SDK](https://github.com/Universal-Commerce-Protocol/js-sdk) - Official JavaScript SDK for building UCP clients and servers.
- [UCP Python SDK](https://github.com/Universal-Commerce-Protocol/python-sdk) - Official Python SDK for UCP.
- [UCP Samples](https://github.com/Universal-Commerce-Protocol/samples) - Official sample agents and merchant implementations for UCP.

## Provider Toolkits and SDKs

Official SDKs from payment providers that give agent frameworks payment tools out of the box.

- [Coinbase AgentKit](https://github.com/coinbase/agentkit) - Framework-agnostic toolkit that gives every AI agent a crypto wallet and on-chain actions, with adapters for LangChain, Vercel AI SDK, OpenAI Agents SDK, and MCP.
- [GOAT SDK](https://github.com/goat-sdk/goat) - Agentic finance toolkit with 100+ plugins for payments, swaps, and commerce across EVM and Solana, adaptable to any agent framework.
- [Nevermined Payments](https://github.com/nevermined-io/payments) - TypeScript SDK for agent commerce with credit-based pricing plans, fiat and crypto checkout, and built-in MCP and A2A integration.
- [Nevermined Payments for Python](https://github.com/nevermined-io/payments-py) - Python SDK for the Nevermined payments protocol.
- [PayPal Agent Toolkit](https://github.com/paypal/agent-toolkit) - Official PayPal tools for OpenAI Agents SDK, LangChain, Vercel AI SDK, and MCP covering payments, invoices, disputes, subscriptions, and reporting.
- [Stripe AI](https://github.com/stripe/ai) - Official monorepo with `@stripe/agent-toolkit` function calling for popular agent frameworks, the Stripe MCP server, usage-based billing helpers, and Claude skills.

## MCP Servers

Model Context Protocol servers that expose payment capabilities as agent tools.

- [Crossmint Checkout MCP](https://github.com/Crossmint/mcp-crossmint-checkout) - MCP server for purchasing physical and digital goods through Crossmint's headless checkout.
- [Lightning MCP Server](https://github.com/lightninglabs/lightning-agent-tools/tree/main/lightning-mcp-server) - Read-only tools for Lightning node state over Lightning Node Connect, part of Lightning Agent Tools.
- [Nevermined MCP Integration](https://github.com/nevermined-io/payments/tree/main/docs) - Register MCP tools, resources, and prompts behind per-request credit pricing with bearer-token validation.
- [PayPal MCP Server](https://github.com/paypal/agent-toolkit/tree/main/modelcontextprotocol) - Official PayPal MCP server exposing 30+ payment, invoicing, and commerce tools.
- [Stripe MCP Server](https://github.com/stripe/ai/tree/main/tools/modelcontextprotocol) - Official Stripe MCP server, available remote at `mcp.stripe.com` or local via `npx @stripe/mcp`, with restricted-key permission control.

## Identity and Trust

Verifying who an agent is and what it is allowed to spend.

- [Sigilum](https://github.com/PaymanAI/sigilum) - Auditable identity for AI agents from PaymanAI.
- [Trusted Agentic Commerce Protocol](https://github.com/forter/trusted-agentic-commerce-protocol) - Forter's authentication and data-encryption protocol between AI agents, merchants, and merchant vendors.
- [Visa Trusted Agent Protocol](https://developer.visa.com/capabilities/trusted-agent-protocol) - Visa's RFC 9421 HTTP Message Signatures framework for verifying agent identity and intent at checkout.

## Examples and Templates

Working reference implementations to start from.

- [ACP Demo](https://github.com/locus-technologies/agentic-commerce-protocol-demo) - Reference implementation of the Agentic Commerce Protocol with an MCP server and MCP-UI storefront.
- [Agentic Economy Boilerplate](https://github.com/xpaysh/agentic-economy-boilerplate) - One vending-machine storefront implemented across five-plus agent payment protocols for side-by-side comparison.
- [Paid MCP Starter](https://github.com/xpaysh/paid-mcp-starter) - Ready-to-use templates for monetizing MCP servers via no-code, x402, and Stripe approaches.
- [Skyfire Solutions Demo](https://github.com/skyfire-xyz/skyfire-solutions-demo) - End-to-end agentic e-commerce flows using Skyfire identity and payment tokens over MCP.
- [UCP Proxy](https://github.com/Shopify/ucp-proxy) - Shopify's proxy for serving Universal Commerce Protocol traffic.

## Resources

Landscape analyses, specifications, and documentation for going deeper.

- [Agent Payment Protocols Landscape](https://github.com/Custena/agent-payment-protocols) - Neutral technical analysis comparing x402, MPP, L402, AP2, Visa TAP and ICC, Mastercard Agent Pay, UCP, ACP, and more, with footnoted primary sources.
- [Agent Skills Specification](https://agentskills.io) - Open specification for the `SKILL.md` agent skill format.
- [Mastercard Agent Pay](https://www.mastercard.com/global/en/business/issuers/agent-pay.html) - Mastercard's agentic payments program built on SD-JWT verifiable intent credentials.
- [Stripe MCP Documentation](https://docs.stripe.com/mcp) - Official guide for connecting agents to Stripe via MCP.
- [x402 Documentation](https://docs.x402.org) - Official developer documentation for the x402 protocol, facilitators, and SDKs.

### Related Lists

- [awesome-agentic-commerce](https://github.com/damoahdominic/awesome-agentic-commerce) - Documents the shift from humans clicking buy buttons to agents transacting on behalf of users.
- [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - The largest curated list of MCP servers across every category, including finance and payments.
- [awesome-ucp](https://github.com/Upsonic/awesome-ucp) - Curated Universal Commerce Protocol resources, tools, and implementations.
- [awesome-x402](https://github.com/xpaysh/awesome-x402) - Deep-dive list of x402 SDKs, facilitators, examples, and ecosystem tooling.

## Contributing

Contributions welcome! Please read the [contribution guidelines](contributing.md) first.
