---
id: C.nyc-map-vs-idea-space
title: "New York on the Map vs in Idea Space"
type: Concept
domain: vector_semantics
epistemic_status: hypothesis
visibility: publishable
extraction: auto
source_ref: "live code session (2026-06-17)"
confidence: high
claude_terms: ["t-SNE", "UMAP"]
schema: v3.1
tags:
  - graph-v3
  - type/concept
---

# New York on the Map vs in Idea Space

`Concept` · `vector_semantics` · *hypothesis* · visibility: **working**

The cleanest single illustration of the whole thesis — and the thing she named as 'the real thing to
illustrate.' On a **map**, New York City is a *point at coordinates* (~40.7°N, 74.0°W): position fixed,
handed over by the rock, measured from Greenwich, neighbors decided by physical adjacency — Newark,
Yonkers, the Atlantic. One position, one neighborhood, imposed. In **idea / latent space**, New York is
a *vector* learned from everything ever said about it: neighbors are whatever it is *related* to —
Tokyo, London, Paris (peer world-cities), Gotham, Wall Street, hip-hop, 'the city that never sleeps.'
Position isn't given, it's learned from relations, and it can sit in *many* neighborhoods at once
(financial-NYC near Hong Kong; cultural-NYC near LA; the-idea-of-NYC near 'ambition'). The map says NYC
is near Newark; idea space says NYC is near Tokyo. Both true — only one is interesting for most
questions. **The map's neighbors are decided by a rock; idea space's neighbors are decided by meaning.**

Bridge: the `P31/P279*` query (NYC → city → settlement → geographic location) is idea-space showing
through the graph — Wikidata is a *discrete, hand-built* approximation (named edges) of what an
embedding holds *continuously* (learned coordinates). Same intuition, two implementations. And a rhyme
worth keeping: even *visualizing* latent space means projecting it down to 2D (t-SNE / UMAP), which
distorts — the Theorema Egregium lie repeats in ML. You cannot flatten the idea-manifold honestly
either.

Context: arose 2026-06-17; likely the first explorable interaction to build (NYC's two neighborhoods,
side by side).

## Connections
- → [[A.geography-fails-at-both]] · illustrates
- → [[C.welded-to-one-shape]] · contrasts_with
- → [[C.latent-space]] · rests_on
- → [[P.sanctioned-topology]] · conceptually_related_to

> source: live code session (2026-06-17) · extraction: auto (schema v3.1)
