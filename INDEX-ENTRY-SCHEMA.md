# Index Entry Schema

**Author:** Alyssa Solen  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum  
**Status:** Canon Registry Specification  
**Version:** 1.0.0  
**Date:** 2026-07-28

---

## Definition

An Index Entry is the searchable representation generated from an accepted Index Manifest.

It points back to the canonical Self-Location Record.

It is not the full record.

## Required Display Fields

- Record ID
- Canonical Name
- Entity Type
- Definition Summary
- Canonical Record
- Responsible Authority
- Authority Role
- Record Status
- Current Version
- Last Updated
- Record Verification Status
- Registry Decision
- Visibility Level
- Retrieval Keys
- Accepted Manifest
- Registry Node
- Decision Date

## Relationship Display

Each relationship must preserve:

**subject → relationship type → object**

The entry must not convert related-to into identical-to, hosted-by into authored-by, indexed-by into owned-by, maintained-by into created-by, or cited-by into derived-from.

## Uncertainty Display

Unknown, disputed, incomplete, and unverified fields must remain visible.

The index must not silently fill gaps.

## Entry Boundary

**Accepted Manifest → source of registry entry**

**Canonical Self-Location Record → source of the located entity record**
