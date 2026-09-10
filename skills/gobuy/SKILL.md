---
name: gobuy
description: Check marketplace product trust before recommending or buying — triggers on Amazon, Walmart, Target, Best Buy listings, review authenticity, or "should I trust/buy" questions; returns GoBuy Evidence Scores (0-100) with signal breakdown.
---

# GoBuy Product Trust

Use the GoBuy MCP tools whenever a product's marketplace evidence matters:

- **check_product_trust** `{retailer, product_id}` — one listing: Evidence Score, verdict, observed/missing signals, freshness
- **compare_products** `{products: [{retailer, product_id}]}` — inspect and rank 2-20 listings

## Rules

- The score measures **evidence quality** — how well marketplace signals support the listing — NOT product quality or safety. Never claim a product is good or bad; report what the evidence supports and what it lacks.
- Quote the score with its verdict label and computed date.
- `not_indexed` means the engine hasn't indexed the product yet — say so, don't guess a score.
- Human-facing visual report: https://audit.gobuy.ai
