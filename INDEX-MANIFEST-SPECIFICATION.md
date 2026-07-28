# Index Manifest Specification

**Author:** Alyssa Solen  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum  
**Status:** Canon Registry Specification  
**Version:** 1.0.0  
**Date:** 2026-07-28

---

## Definition

An **Index Manifest** is the compact, structured summary submitted to a Self-Location Registry.

It contains enough public information to identify, validate, register, and retrieve a canonical Self-Location Record.

It is not a replacement for the full record.

---

## Required Fields

- Manifest Version
- Record ID
- Canonical Name
- Entity Type
- Definition Summary
- Canonical Record URL
- Responsible Authority
- Authority Role
- Authority Basis
- Proof of Control or Authority
- Record Status
- Current Version
- Last Updated
- Verification Status
- Visibility Level
- Retrieval Keys
- Claims Summary
- Does Not Claim Summary
- Relationship Pointers
- Indexing Permission
- Display Permission
- Cache Permission
- Record License or Permission URL
- Submission Contact

---

## Recommended Fields

- Integrity Hash
- Hash Algorithm
- Former Names
- Aliases
- Supersedes
- Superseded By
- Unknown or Disputed Fields

---

## Registry-Assigned Fields

The registry assigns:

- registry node,
- submission issue,
- submitted date,
- registry decision,
- decision date,
- decision reason,
- accepted manifest path,
- and index entry path.

Submitters must not preassign a registry decision.

---

## Field Separation Rules

**record verification status ≠ registry decision**

**record authority ≠ registry authority**

**canonical record ≠ stored manifest**

**submission contact ≠ ownership**

**relationship pointer ≠ identity**

**acceptance ≠ endorsement**

**public visibility ≠ unrestricted reuse**
