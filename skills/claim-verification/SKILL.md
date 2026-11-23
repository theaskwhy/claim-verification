---
name: claim-verification
description: Verify important factual claims with traceable sources, dates, provenance, corroboration, and explicit uncertainty.
---

# Claim Verification

Important factual claims must be traceable to evidence appropriate to the claim. A useful answer without an adequate source trail is not a verified answer.

## Source hierarchy

Prefer, when available:

1. Primary official source: regulator, public authority, manufacturer or operator, filing, technical publication, court or government record, or official dataset.
2. High-quality independent reporting or specialist source.
3. Secondary summaries for discovery and context, not as the sole support for consequential claims when primary evidence exists.
4. Social posts as primary evidence only for what that account actually announced or showed, not for unsupported broader conclusions.

## Verification workflow

- Record source URL or identifier, publisher, publication/update date, and access/retrieval date where practical.
- Separate event date from article or post publication date.
- Cross-check surprising, disputed, safety-relevant, or consequential claims.
- Preserve attribution and licensing/provenance for imported datasets and media.
- Label uncertainty rather than filling gaps with plausible guesses.
- Detect duplicate or syndicated records before treating them as independent corroboration.
- Before large-scale extraction, check for an official API, download, or feed; follow terms and rate limits; cache source identifiers/snapshots only where permitted; stage parsed data; preserve provenance; and deduplicate and validate before production ingestion.

## Claim states

Use one of `Verified`, `Partially Verified`, `Unverified`, or `Disputed` based on the available evidence. Keep the underlying source trail so a claim can be reevaluated. Social-only claims remain `Unverified` and `lead_only=true` until independently checked. Keep `lead_only` separate from the claim state.

The proposed read-only ledger shape is in `references/claim-ledger.md`; it is not a database schema and does not authorize writes or migrations.

## Completion

For each consequential claim, report what is verified, what remains uncertain, conflicting evidence, and the strongest supporting source. If using `social-research-reader`, keep content retrieval status separate from the truth status of claims.
