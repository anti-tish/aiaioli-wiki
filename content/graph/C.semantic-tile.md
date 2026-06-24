---
id: C.semantic-tile
title: "The Semantic Tile"
type: Concept
domain: geography_cartography
epistemic_status: hypothesis
visibility: publishable
extraction: auto
source_ref: "live code session (2026-06-15)"
confidence: medium
claude_terms: ["semantic tile"]
schema: v3.1
tags:
  - graph-v3
  - type/concept
---

# The Semantic Tile

`Concept` · `geography_cartography` · *hypothesis* · visibility: **publishable**

A vector tile is pre-baked geometry plus attributes for one styling at one zoom — optimized for fast
display (binary-packed, generalized per zoom, CDN-cached) but dumb: its meaning is frozen at
tile-generation time, it cannot infer or recombine, and to change what it shows you re-tile. A
*semantic tile* inverts the priority: the tile's contents are defined by a query over a triple store,
so the map is a query *result*, not a product. 'Administrative boundaries' vs 'vernacular boundaries'
vs 'figure-ground' become different maps from the same substrate — 'visualize space, not make a map'
made literal: the tile is a question. Figure-ground is the purest case, because the figure/ground
decision is itself a semantic class query (a region typed water becomes black, its complement white) —
the most semantic cartographic style there is, Stamen Toner as one SELECT.

The honest architecture, no hype: RDF is verbose and slow to render raw; vector tiles win the
*painting* race by design and always will. So the win is not 'semantics renders faster' — it is that
semantics is *queryable and inferential* where a tile is inert. The real lightness is not bytes
(triples are heavy); it is *inference*: a triple store derives transitive containment (A in B, B in C,
therefore A in C) without storing it, so you need not bake every derivable relation. A vector tile can
infer nothing. The buildable form is therefore not semantics-instead-of-tiles but semantics as
source-of-truth with a derived, cached render layer — materialised semantic tiles: tile-speed display,
query-defined contents.

## Connections
- → [[P.sanctioned-topology]] · rests_on
- → [[Q.even-more-open-osm]] · serves
- → [[C.relational-ontology]] · is_instance_of
- → [[A.wikidata-atlas]] · conceptually_related_to
- → [[C.critical-cartography]] · conceptually_related_to

> source: live code session (2026-06-15) · extraction: auto (schema v3.1)
