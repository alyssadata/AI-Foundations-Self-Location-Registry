# AI Foundations | Self-Location Registry

**Repository:** AI-Foundations-Self-Location-Registry  
**Status:** Canon Registry Protocol / Initial Public Registry Node  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum  
**Author:** Alyssa Solen  
**Version:** 1.0.6  
**Release date:** 2026-07-28  
**Canonical entrance:** https://awakeningcodex.com

---

## Repository Purpose

This repository defines and operates the first public registry node for the **AI Foundations Self-Location Standard**.

The Self-Location Standard defines how a person, project, organization, system, paper, AI agent, dataset, hypothesis, or other entity publishes an accurate, source-supported Self-Location Record.

This registry defines how a record enters a federated index.

The operational sequence is:

**Full Self-Location Record → canonical source**

**Index Manifest → submission summary**

**Registry → intake and validation**

**Index Entry → searchable route to the canonical source**

The full Self-Location Record does not become the property of this registry.

The registry receives a structured summary, checks the source and stated authority, records the submission decision, and creates a searchable entry that points back to the canonical record.

---

## Relationship to the Standard

The normative record structure is defined in:

**AI Foundations | Self-Location Standard**

https://github.com/alyssadata/AI-Foundations-Self-Location-Standard

This repository does not replace or rewrite that standard.

It implements the operational layer required to receive, validate, register, and index records created under it.

---

## What This Registry Is

This repository is:

- an intake point for public Index Manifests,
- an authority and source validation protocol,
- a record of registry decisions,
- a public index of accepted entries,
- an initial registry node,
- and a reference implementation for future federated registry nodes.

---

## What This Registry Is Not

This repository is not:

- the canonical home of every full Self-Location Record,
- the owner or author of submitted records,
- a universal authority over people or entities,
- proof that every claim in a submitted record is true,
- an endorsement of every indexed entity,
- a merger of the records it resolves,
- or the only registry node that may exist.

---

## Initial Public Workflow

1. Create a full Self-Location Record under the Self-Location Standard.
2. Publish it at a canonical location controlled by the appropriate authority.
3. Complete the Index Manifest.
4. Submit the manifest through the repository submission issue form.
5. The registry checks required fields, canonical source access, stated authority, visibility, permissions, and relationship evidence.
6. The registry records one of the defined decisions.
7. An accepted manifest is stored under `records/`.
8. A searchable entry is added to `INDEX.md`.

The first implementation is manually reviewed.

Automation may be added later without changing the source, authority, or non-merge boundaries.

---

## Public Node Boundary

This GitHub repository is a public registry node.

It accepts only information that the submitter is authorized to make public.

A public manifest may point to a restricted canonical record, but restricted fields must not be copied into this repository.

Fully private records require a permissioned registry node and are not submitted through this public repository.

---

## Repository Contents

- [Submission Protocol](SUBMISSION-PROTOCOL.md)
- [Submit a Record](SUBMIT-A-RECORD.md)
- [Index Manifest Specification](INDEX-MANIFEST-SPECIFICATION.md)
- [Index Manifest Template](INDEX-MANIFEST-TEMPLATE.yaml)
- [Authority Verification](AUTHORITY-VERIFICATION.md)
- [Visibility Levels](VISIBILITY-LEVELS.md)
- [Registry Decisions](REGISTRY-DECISIONS.md)
- [Index Entry Schema](INDEX-ENTRY-SCHEMA.md)
- [Public Index](INDEX.md)
- [Registry Self-Location Record](SELF-LOCATION.md)
- [Machine-Readable Registry Record](machine-readable/self-location.yaml)
- [Example Manifest](examples/example-index-manifest.yaml)
- [Example Index Entry](examples/example-index-entry.md)
- [Citation Metadata](CITATION.cff)
- [Zenodo Metadata](.zenodo.json)
- [Source-Line License](LICENSE.md)

---

## Core Registry Boundary

**Submission does not transfer authorship.**

**Hosting does not transfer authority.**

**Validation does not equal endorsement.**

**Indexing does not equal ownership.**

**Retrieval does not make the registry the source.**

**Relationship does not equal identity.**

**Federation does not equal merger.**

---

## Required Citation

Alyssa Solen, *AI Foundations: Self-Location Registry*, AI-Foundations-Self-Location-Registry Repository. Source-line: Alyssa Solen → AI Foundations → Origin | Continuum.

---

## License

This repository uses `CC-BY-ND-4.0` citation metadata and the AI Foundations Source-Line License.

Citation is permitted with source-line preserved.

Derivative use is not authorized.
