# Taggle NOAM_CENTRIC_GRAPH_V1 — Recommendation Explanation Viewer

This is an internal Taggle recommendation-explanation **prototype**: an interactive
"why did Taggle recommend this restaurant?" viewer for Noam's frozen top-10 restaurant
recommendations from the `NOAM_CENTRIC_GRAPH_V1` experiment.

It is a single self-contained static HTML page (`index.html`) with no backend and no
external dependencies — all data is inlined and the page runs entirely in the browser.

## What this is

- A read-only visualization of an already-frozen, already-computed recommendation
  experiment. No live recommender runs here; nothing on this page recalculates,
  reranks, or tunes anything.
- Two views: an overview of all 10 recommendations sized by network support, and a
  per-restaurant "why this?" detail view showing the actual one-hop/two-hop evidence
  paths behind each recommendation.
- A **Simple** vs **Detailed** toggle, and a clear visual/label distinction between
  *network (structural) support* and *actual taste-alignment evidence* — the two are
  not the same thing, and the page never implies more taste-match evidence than the
  underlying experiment actually found.

## Privacy note

This published copy has been sanitized for public sharing: every real reviewer name
and Google Maps contributor ID from the source data has been replaced with a
deterministic `Reviewer N` label. No personally identifying information, API keys, or
internal file paths are present in this page. Restaurant names/addresses (public
business information), ranks, scores, ratings, and evidence counts are unchanged from
the original frozen experiment output.

## Status

Internal prototype — not a finished product, not a recommendation sent to any end user.
