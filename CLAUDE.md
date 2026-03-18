# Undo - CLAUDE.md

## What is Undo

Undo (withundo.com) is B2B returns infrastructure for DTC brands on Shopify. Customers submit photos of returned items at home, AI verifies condition, eligible items ship peer-to-peer from returner to next buyer. No warehouse, no reverse shipping. Ineligible items flow through the brand's existing process unchanged.

Reduces per-return cost from ~$12 to $3, turnaround from two weeks to two days. P2P applies to 30-45% of eligible returns (high-velocity SKUs, unworn items). Traditional disposition handles the rest.

Founded by Rajan Devnath. 7+ years logistics infrastructure (including Portless), fulfillment across China, US, SE Asia. Brand color: #0EA5A9.

---

## Current state

Pre-revenue, pre-product. Seeking 3-5 design partner customers through manual outbound. First pilot may use manual ops before AI/matching is built.

Website: withundo.com (GitHub Pages, Namecheap DNS). Live with "Get Early Access" and "Book a Call" CTAs.

Accuracy: materials now say "up to 95% (AI + human review)." Internal research says 70-85% realistic standalone AI, 90-95% with hybrid review. The cost math ($12 to $3) is the stronger outreach hook.

---

## Target market

$5M-$50M DTC apparel brands on Shopify. Sweet spot for first customers: $10M-$30M (50-150+ orders/day, founder-led purchasing decisions). Minimum 150 returns/month.

Verticals: women's apparel and athleisure now, baby/kids clothing ~month three. Footwear and accessories are valid but not primary outbound targets. Luxury deprioritized (error rate risk at high AOV).

Brands can be qualified for P2P fit using their public products.json endpoint: partial sell-through ratio, product type concentration, and review counts proxy for demand concentration. Scriptable in Claude Code.

---

## Competitive context

Primary incumbent: Loop Returns. Adjacent: Happy Returns, Optoro, Trove/Recurate, AfterShip. Undo differentiates on P2P direct-ship and AI home grading, neither of which incumbents do autonomously.

---

## Pricing

Current stated price: $3/return (early access rate). Recommended anchor: $3.50-$4.00. Introductory rate for early brands: $2.50-$3.00. Future: commission layer once Undo lists on external marketplaces.

---

## Outreach

Channels: cold email (primary) > LinkedIn DM (when founders are active) > contact forms > Instagram DM (last resort). All sends manual. Apollo and Clay for list building only.

Prospect sourcing: mining Loop/Returnly/AfterShip app store reviews (3 stars and below, US), StoreCensus saved search ("Undo ICP", 207 results), Apollo for contact enrichment.

Tools: Apollo (find emails) + Hunter (verify) + Instantly.ai (sequencing/warmup).

Key rules: no generic flattery openers. Don't mention AI grading in early outreach (say "verify condition remotely," save AI for the call). Use "early access" not "pilot." LinkedIn pre-engagement is optional and not worth doing if it reduces volume.

---

## Workflow

- **Claude Chat (this project):** Strategy, research, message drafting. 5 sessions: P2P scratchpad, AI video verification, Pricing Strategy, ICP, GTM strat.
- **Claude Code:** Implementation, scripts, website, email pipelines. Connected to undo folder.
- **Claude Co-Work:** LinkedIn URL generation, prospect research, browser tasks.

Rajan's style: direct, iterative, pushes back and expects engagement not agreement. Plain language, no jargon in customer-facing materials. Decides fast once options are clear.

Trademark filing target: "withundo" (distinct from UNDO Software at undo.software).

---

## Website design rules

- **Line breaks**: When headings or bold text wrap to multiple lines, control where they break using `<br>` tags so each line reads as a complete thought. Never let text break mid-phrase (e.g. "on a 20-\nmin call" is bad; "economics\non a 20-min call" is good). Always check at both desktop (1280px) and mobile (375px).
- **Color consistency**: Traditional/incumbent content uses muted gray (`#6B7080` / `var(--text-secondary)`). Undo content uses brand teal (`#0EA5A9` / `var(--accent)`). No red for competitor metrics — stay neutral and confident, let the numbers speak.
- **No pills/badges** for table values. Use plain bold text with color differentiation only.
- **Typography**: Outfit for headings/labels/brand elements. DM Sans for body text. Don't mix.
- **Tone**: Minimal, not overdesigned. Avoid visual noise (excessive colors, badges, borders). The site should feel like a confident spec sheet, not a sales page.