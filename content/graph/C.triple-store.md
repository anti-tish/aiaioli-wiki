---
unlisted: true
id: C.triple-store
title: "Triple Store"
type: Concept
domain: knowledge_systems
epistemic_status: verified_fact
visibility: publishable
extraction: hand
source_ref: "v2.1 knowledge-graph concept (technical reference) — systems-architecture thread, 2026-01"
confidence: high
claude_terms: []
wikidata_id: Q1265
canonical_source: "RDF/SPARQL W3C standards"
schema: v3.1
tags:
  - graph-v3
  - type/concept
---

# Triple Store

`Concept` · `knowledge_systems` · *verified_fact* · visibility: **publishable**

A database that stores knowledge as subject-predicate-object triples. Every fact is a relationship between two things. Contrast with relational databases (tables/rows) and document databases (nested JSON). The key property: graph traversal is native — you can follow relationships across the entire dataset in a single SPARQL query. Reasoning is also native: if X is in Y and Y is in Z, the store can infer X is in Z without you stating it explicitly. Federation is native: you can query your personal triple store and Wikidata in the same query using SERVICE. This is the architecture that makes "personal knowledge layer on top of Wikidata" actually implementable.

## Connections
- → [[O.intuited-triple-stores]] · demonstrated_by
- → [[A.wikidata-atlas]] · makes_possible
- → [[C.non-hierarchical-brain]] · conceptually_related_to

> source: v2.1 knowledge-graph concept (technical reference) · extraction: hand (schema v3.1)
