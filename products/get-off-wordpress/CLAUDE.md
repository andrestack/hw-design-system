# Get Off WordPress: working notes for Claude

This folder holds the product, pricing, funnel and ads plan for Hinterland Web's "get off WordPress, Squarespace and Wix" offer.

## Files

- `plan.md`: the full plan (offer ladder, done-for-you, e-commerce, where to sell, risks, launch phases). A snapshot of the live Claude doc, which is the source of truth during planning: https://claude.ai/artifact/UpViN3ZPm1agekUXJ9h1Ko
- `funnel-pages.md`: build brief for the seven funnel pages, with reference sites.
- `ads-playbook.md`: Meta and Google ad plan, MCP setup, weekly loop, build-in-public posts.

## Rules

- All pages and creative follow `../../design-system/README.md` and `../../design-system/tokens.json`: first-person "I" voice, Australian spelling, dark navy theme, teal for actions only.
- Digital products are priced in USD and sold through Polar. Done-for-you and care plans are priced in AUD including GST.
- Never launch an ad campaign or raise a budget without André's explicit approval in chat.
- Only migrate sites the buyer owns.
- When the plan changes, update `plan.md` and say what changed in the commit message.

## Next up

1. Answer the open questions at the end of `plan.md`.
2. Build `/audit` (Worker + PageSpeed API + Turnstile) and `/exit` in the hinterlandweb.com repo.
3. Set up Polar products and the GitHub repo benefit for the Kit.
4. Connect the Meta Ads MCP server; draft the first test campaign for approval.
