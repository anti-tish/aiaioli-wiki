---
id: P.sliver-is-a-fact
title: "The Sliver Is a Fact, Not an Error"
type: Pattern
domain: geography_cartography
epistemic_status: hypothesis
visibility: publishable
extraction: auto
source_ref: "live code session (2026-06-15)"
confidence: high
claude_terms: []
schema: v3.1
tags:
  - graph-v3
  - type/pattern
---

# The Sliver Is a Fact, Not an Error

`Pattern` · `geography_cartography` · *hypothesis* · visibility: **publishable**

In clean cartographic topology, overlaps and slivers are errors — coverage rules, snapping, cluster
tolerance and validity checks all exist to enforce a planar partition where every point belongs to
exactly one polygon and edges meet without overlap. That rule bakes in a metaphysics: that space is
cleanly divisible, that every place has a single answer to 'what region is this.' But the overlap is
often the truth, not the error — contested territory, a block that is genuinely both Harlem and
Morningside Heights, ecotones, bilingual zones, the gentrification frontier that is two places at
once. Clean topology forbids exactly the realities that matter most; the no-overlap rule is
[[C.borders-make-irreal-real]] hiding inside a validation check. A relational model does what planar
geometry structurally cannot: a point can be 'within' multiple regions as multiple triples, each with
its own provenance, coexisting without contradiction. The sliver that is a validation *failure* in GIS
is a sourced *fact* in a triple store — multi-valued and contradiction-tolerant. Against a GeoJSON
stack (which can *show* an overlap but treats it as a mute visual coincidence — flat properties, no
relations between features, no model of who-claims-what), the advantage is not display but meaning: the
contested zone becomes a class you can query — 'show me everywhere two authorities both assert
jurisdiction' — sourced and reasoned, not eyeballed. Don't clean the slivers; attribute them. And the
honest map that shows 'here be contested' instead of a false crisp line is *more* intuitable for it,
because people already know borders are fuzzy — the clean map gaslights lived experience. The error
message is the feature.

## Connections
- → [[C.borders-make-irreal-real]] · is_instance_of
- → [[P.sanctioned-topology]] · extends
- → [[C.critical-cartography]] · is_instance_of
- → [[C.relational-ontology]] · rests_on
- → [[C.semantic-tile]] · queried_via

> source: live code session (2026-06-15) · extraction: auto (schema v3.1)
