# Data Types and Templates Library

A browser-based library for exploring reusable data types and templates. The current repository is centered on `index.html`, a self-contained interface titled **Template Library & Fillable Forms**.

## Contents

| Path | Purpose | Status |
|---|---|---|
| [index.html](index.html) | Browser UI for browsing templates, editing template fields, and working with entries | Existing interface; review behavior and persistence before relying on it for durable storage |

## Intended role in the wider repository portfolio

This repository should be the shared home for reusable data structures and template definitions that can be consumed by procedural playbooks, records libraries, cataloging systems, and search/ingestion tools.

It should complement rather than duplicate:
- [Forms-and-Templates-Library](https://github.com/bradgeigermanager-sketch/Forms-and-Templates-Library), which currently contains operational form templates and a JSON-schema directory.
- [Procedures-Playbooks-Library](https://github.com/bradgeigermanager-sketch/Procedures-Playbooks-Library), which defines decision-tree playbooks and library exports.
- [Records-Deduplication-Suite](https://github.com/bradgeigermanager-sketch/Records-Deduplication-Suite), which needs stable record, evidence, comparison, and audit structures.

These are candidate integration relationships, not established software dependencies. Agree on schema identifiers and versions before sharing structures across repositories.

## Recommended conventions

A reusable template should, where applicable, declare:
- stable machine-readable identifier and human-readable title;
- schema version and compatibility expectations;
- purpose, scope, owner/maintainer, and status;
- required and optional fields with types and validation constraints;
- controlled vocabularies and units where relevant;
- provenance, source, and change history;
- example valid data and invalid examples;
- privacy/sensitivity notes and retention expectations;
- validation tests and a migration note for breaking changes.

Keep the template definition separate from the data entered into a template. A UI preview or browser-local entry should not be represented as durable, centrally stored data unless a persistence mechanism is explicitly implemented and tested.

## Development roadmap

- [ ] Inventory the template model and all UI behaviors in `index.html`.
- [ ] Extract reusable template definitions into versioned JSON files or a documented registry format.
- [ ] Add JSON Schema validation and sample fixtures.
- [ ] Document whether data is stored locally, exported, or persisted remotely.
- [ ] Add automated validation for schema syntax, required fields, and stable IDs.
- [ ] Add a searchable catalog and clear categories/tags.
- [ ] Document import/export compatibility and error handling.
- [ ] Coordinate shared primitives with the Forms and Playbooks libraries.

## Current status

This README documents the repository's visible entry point and a proposed organization path. It does not claim that all templates are already normalized, schema-validated, or integrated with other repositories.