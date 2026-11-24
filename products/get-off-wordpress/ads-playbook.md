# Ads playbook

Two engines. Claude runs what it can through MCP. André approves every new campaign and every budget increase before it goes live.

## Engine 1: Meta, self-liquidating US$9 guide

A tripwire funnel sells a low-priced offer (usually $7–$47). Once tuned, the tripwire plus its bumps and upsells pays for the ads that brought the traffic ([systeme.io](https://systeme.io/learn/tripwire-funnel/)).

**Maths:** US$9 guide, +US$20 Kit upgrade (assume 30% take it) and US$70 more for Pro (assume 10%). That's an average first order of about US$22. Target cost per buyer: under US$20.

**Test:** A$20/day for 14 days. Keep the ad sets that come in under target; kill the rest. Set the Meta ad account spending limit to the test budget.

**Campaign structure (Sales objective, purchase event on the thank-you page):**
- Audiences: small-business owners and freelancers, AU / US / UK / NZ, interests WordPress, Wix, Squarespace, Claude.
- Creative angles, 3 each:
  - "Your website renewal bill" (cost)
  - "My site got hacked" (fear)
  - "Claude rebuilt this in an afternoon" (curiosity, with a screen recording)
- Retargeting: audit-tool users and guide buyers → Pro and masterclass.

**Tooling:** Meta's official Ads MCP server (open beta since 29 Apr 2026, 29 tools) ([dev.to](https://dev.to/mattkundo/meta-ads-mcp-launch-ai-agents-can-now-run-your-campaigns-mkdm-4gnl); [Meta docs](https://developers.facebook.com/documentation/ads-commerce/ads-ai-connectors/ads-mcp-server/ads-mcp-server-overview)).

Claude Code setup, from Meta's get-started guide ([Meta](https://developers.facebook.com/documentation/ads-commerce/ads-ai-connectors/ads-mcp-server/ads-mcp-server-get-started)):

```bash
claude mcp add --transport http --client-id <META_APP_ID> meta-ads https://mcp.facebook.com/ads
```

In claude.ai you can instead add `https://mcp.facebook.com/ads` as a custom connector and sign in with OAuth. Limit access to the Hinterland Web ad account only.

## Engine 2: Google Search, done-for-you (AUD)

- Geo: Sunshine Coast + SE Queensland.
- Keywords: "wordpress site hacked", "website rebuild", "leave wix", "website hosting too expensive".
- Landing pages: `/wordpress-hacked` and `/move-my-site`.
- Goal metric: cost per done-for-you enquiry.
- **Tooling:** Google's official Google Ads MCP server reads data only: reporting works, changes don't ([Zernio](https://zernio.com/blog/connect-google-ads-mcp-to-claude); [Google](https://developers.google.com/google-ads/api/docs/developer-toolkit/mcp-server)). Claude drafts campaigns and keywords and reads results; André makes the changes in Google Ads, or we add a third-party server that can write.

## LinkedIn

Organic carousels first (the design system has the carousel spec). Paid LinkedIn only once done-for-you converts. Third-party MCP options exist, e.g. AdKit, which saves changes as drafts until you approve them ([AdKit](https://mcpservers.org/servers/linkedin-ads-mcp-server-by-adkit)).

## Weekly loop (Claude)

1. Pull last 7 days: spend, buyers, cost per buyer, upgrade rates, DFY enquiries.
2. Propose changes with expected effect. Wait for approval.
3. Apply the approved changes through MCP.
4. Draft the build-in-public post for that week.

## Build-in-public series

1. "Claude rebuilt this WordPress site in an afternoon": before/after speed, cost, recording.
2. "Claude built my sales funnel": audit tool and pages going live on Cloudflare.
3. "I gave Claude my Meta ad account": setup, guardrails, first campaign.
4. "Week 1 numbers": spend, buyers, cost per buyer, what Claude changed and why.
5. "The ads paid for themselves (or didn't)": the maths, honestly.
