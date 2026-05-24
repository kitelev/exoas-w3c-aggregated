# exoas-w3c-aggregated

W3C foundational TBox assets (RDF, RDFS, OWL, XSD, SHACL) — aggregated representation.

This repository is the AGGREGATED variant — all W3C foundational terms collected under one assetspace root. Parallel to [exoas-w3c](https://github.com/kitelev/exoas-w3c) (non-aggregated representation).

## Provenance

Created 2026-05-24 per [RFC 107818a0](https://github.com/kitelev/vault-exodev/blob/main/inbox/107818a0-fc21-47ad-a79b-c28cb6b6eb32.md): TBox re-home from `shared-identities` (which was misclassified as Ontology container).

## Contents

14 W3C/RDF/RDFS/OWL/XSD/SHACL foundational class + property assets:
- rdf__Statement, rdf__subject, rdf__predicate
- rdfs__Class, rdfs__Resource, rdfs__subClassOf, rdfs__subPropertyOf, rdfs__range, rdfs__domain, rdfs__isDefinedBy
- owl__NamedIndividual, owl__ObjectProperty
- xsd__Date
- sh__severity

## Usage

Add as git submodule in your Exocortex vault under `assetspaces/w3c-aggregated/`.
