# 📤 SUBMISSION — AI Decider: Wedding Venue Comparison

Model used: `llama3.1:8b` via Ollama (local). Prompts sent verbatim from `ACTIVITY_decider.md`.

---

## Stage 1 — Base Priorities

**Couple's priorities:** under $8,000 rental · ~120 guests · romantic, not corporate · outdoor ceremony required · in-house or approved-vendor catering.

### Comparison Table

| Venue | Capacity | Approx. Price/Night | Catering | Outdoor | Parking | Vibe |
|---|---|---|---|---|---|---|
| The Rosewood Estate | 175 | $17,500 (Fri–Sun) | Preferred list (4) | Yes + rain tent | On-site ~80 | Romantic |
| The Grand Metropolitan Hotel | 300 | $12,000+ rental | In-house only | No | Valet | Elegant |
| Lakeview Pavilion | 90–110 | $2,500 (weekend) | BYOB | Yes (no backup) | Not stated | Rustic |
| Thornfield Manor | 150 | $18,000 | In-house | Yes (grounds/chapel) | Not stated | Historic |
| The Foundry at Millworks | 250 | $5,000 | BYO vendors | Rooftop only | Street/garage | Industrial |
| Sunrise Farm & Vineyard | 130 | $9,800 (weekend) | In-house + 2 approved | Yes (terrace) | Ample | Romantic |
| The Atrium Club | 300+ | $9,000–$14,000 | Flexible | Not stated | Not stated | Corporate |
| Cedar Hollow Retreat | 60 | $3,200 (Sat) | Outside allowed | Implied woodland | Field | Rustic |
| The Belvedere | 180 | $28,000 (rental + F&B min) | In-house required | Yes (indoor/outdoor) | Valet | Elegant |
| Harborside Event Center | 220 | *TBD* | Flexible | Yes (terrace) | Lot | Modern |
| The Ivy House | 100 | $4,500 | BYOB | Yes (garden) | Street + shuttle | Garden |
| Maple Ridge Country Club | 160 | $28,500+ | In-house only | Implied (golf course) | Ample | Classic |
| The Glasshouse Conservatory | 140 | $18,000 | Open | Yes (garden) | On-site | Dramatic |
| Millbrook Inn | 120 | $10,500 | Outside allowed | Yes (lawn) | Not stated | Charming |
| The Warehouse District Loft | 200 | $8,800 | None (no kitchen) | Not stated | Not stated | Raw |
| Cloverfield Farms | 135 | $6,000 (Fri–Sun) | Preferred list (3) | Yes (barn + field) | Lots | Warm |

### Top 3 Shortlist

1. **Cloverfield Farms** — the only venue that satisfies every hard constraint: $6,000 rental (under budget), 135-guest capacity, outdoor barn/field, 3-vendor preferred caterer list, warm non-corporate feel.
2. **Sunrise Farm & Vineyard** — $9,800 is ~$1,800 over the ceiling, but it is otherwise a textbook fit (130 capacity, outdoor terrace, in-house + 2 approved caterers, vineyard romance); worth flagging for budget negotiation.
3. **The Ivy House** — $4,500 and a real outdoor garden for 100 guests; capacity is tight and BYOB catering violates the approved-vendor rule, so only viable if the couple can contract an approved caterer separately.

### Exclusions

One venue (**Harborside Event Center**) had to be set aside from ranking because its pricing is listed as TBD; the rest were comparable on the stated fields.

---

## Stage 2 — Revised Priorities

**New priorities:** budget up to $15,000 · ~200 guests · elegant, grand · outdoor nice-to-have · no catering constraint.

### Revised Top 3 Shortlist

1. **The Grand Metropolitan Hotel** — 300-guest downtown ballroom at $12,000 rental; the "elegant, grand" brief is exactly what this venue sells, and dropping the catering constraint removes the prior in-house-only objection. No outdoor, but that is now only nice-to-have.
2. **The Atrium Club** — 300+ capacity, $9,000–$14,000 fits the budget band, flexible catering. The description skews corporate rather than warmly "elegant," but for a formal, grand-scale reception it clears every hard line.
3. **Harborside Event Center** — 220 capacity with a waterfront terrace for an outdoor option; pricing is still TBD so recommend confirming the quote falls under $15,000 before deposit.

### What Moved and Why

- **Up:** Grand Metropolitan Hotel (was excluded for no outdoor + in-house-only; both constraints relaxed), Atrium Club (budget band now inside range, corporate tone acceptable for "grand"), Harborside (capacity for 200 and outdoor terrace now matter more than they did at 120).
- **Down:** Cloverfield Farms, Sunrise Farm & Vineyard, and The Ivy House all fall out of contention — none can seat 200 guests, and none reads "elegant/grand." The Foundry and Warehouse Loft also stay out: they fit the capacity but not the vibe shift from "trendy/raw" to "elegant."
- **Still over budget:** The Belvedere ($28,000) and Maple Ridge Country Club ($28,500+) match on elegance but blow the new $15,000 ceiling.

---

## Stage 3 — Reflection

The model did the mechanical work well: it normalized 16 paragraphs of prose into a clean table, correctly extracted numeric ranges (e.g., "$9,000–$14,000"), and filtered on hard constraints hierarchically — dropping outdoor-less and wrong-catering venues in Stage 1, then re-promoting them in Stage 2 when those rules were lifted. Where it struggled was on soft, interpretive fields: reducing vibe to one word loses nuance (Cloverfield is "warm" and "rustic" and arguably "romantic" all at once), and it collapsed capacity ranges like "90 comfortably, 110 at a squeeze" into a single number, which matters at a 120-guest target. It also quietly treated the $8,000 budget as flexible to recommend Sunrise Farm at $9,800 — reasonable, but worth stating explicitly. Before trusting any shortlist I would verify the quoted rental is all-in (service fees, minimums, taxes), confirm rain-backup plans for outdoor ceremonies, check what cuisines the preferred-vendor lists actually cover, and pull a real price from Harborside so it can be scored instead of excluded.

---
