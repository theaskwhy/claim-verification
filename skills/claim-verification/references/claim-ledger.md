# Proposed claim ledger (read-only; mapping to current datastore NOT_VERIFIED)

```json
{"claim_id":"string", "exact_claim":"string", "source_urls":[], "publisher":"string|null", "event_date":null, "published_at":null, "retrieved_at":null, "locator":null, "independent_corroboration":[], "conflicts":[], "state":"Verified|Partially Verified|Unverified|Disputed", "lead_only":false}
```

Use v1 state names. `lead_only` is a separate proposed flag, not an accepted persistent enum. Preserve source timestamps and syndication origin. Do not write or migrate a database without finding its actual schema and owner approval.
