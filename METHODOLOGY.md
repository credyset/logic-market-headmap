# Methodology and Governance

## Scope boundary

- External corpus only.
- Logic-authored or Logic-participant material is excluded from corpus statistics, discovered taxonomy, buyer language, trends, and quotations.
- Logic context and website content are comparison targets used for Phase 0 and Phase 7.

## Reproduced method

The research reuses the prior exercise’s method, not its conclusions:

1. Preserve canonical source provenance and transcript metadata.
2. Normalize speaker turns and timestamps.
3. Group turns into approximately 150–250-word chunks.
4. Discover semantic clusters from external text before locking a taxonomy.
5. Review representative examples from every cluster and identify noise.
6. Collapse near-duplicates into plain-language topics.
7. Run multi-label classification across all chunks.
8. Compare normalized shares across time, industry, role, source type, and host/guest status.
9. Extract sentence-level pains, questions, objections, triggers, alternatives, tools, numbers, and claims with exact provenance.
10. Compare the resulting market map with Logic’s current site and positioning.

## Prior-art firewall

- Existing `taxonomy.json`, classified outputs, and EasyOps findings are preserved only as a reproducibility record.
- They will not seed or constrain the Logic taxonomy.
- The Logic analysis will begin from raw external episode records and normalized chunks.
- After the Logic taxonomy is reviewed and locked, it may be compared with the prior taxonomy to document agreement and contradiction.

## Source inclusion

Include canonical transcripts, recordings, articles, talks, and current competitor or industry resources with traceable provenance. Exclude:

- Logic first-party transcripts and recordings.
- Reposts when the canonical source is available.
- Scraped summaries lacking original-source links.
- Sources that prohibit automated access.
- Quote records whose exact wording and location cannot be recovered.
- Promotional introductions, sponsor reads, and unrelated biography from high-signal analysis.

## Retrieval accounting

- Authorized external retrieval budget: 300 calls.
- Local reuse of already-collected external files: 0 calls.
- Each new retrieval is recorded in `retrieval-ledger.csv` with date, URL/domain, purpose, outcome, cache path, and cumulative count.
- Search-result discovery and source-page retrieval are tracked separately.

## Opportunity scoring

Each content opportunity will retain raw 1–5 scores for:

1. Audience relevance — 18%
2. Pain intensity — 16%
3. Search/discovery intent — 12%
4. Evidence strength — 14%
5. Differentiation potential — 12%
6. Timeliness — 7%
7. Commercial relevance — 13%
8. Claims risk — 4% (reverse-scored)
9. Production effort — 4% (reverse-scored)

Weighted score = sum of weighted normalized dimensions. Search intent cannot contribute more than 12%, preventing volume from overwhelming audience and pain relevance. All raw inputs and notes remain visible.

## Evidence classes

- First-party evidence from the external speaker’s own company or experience
- Customer-reported
- Expert opinion
- Third-party research
- Unverified or conflicting

Frequency is reported separately from commercial importance.
