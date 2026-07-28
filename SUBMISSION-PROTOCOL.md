# Submission Protocol

**Author:** Alyssa Solen  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum  
**Status:** Canon Registry Protocol  
**Version:** 1.0.0  
**Date:** 2026-07-28

---

## Purpose

The Submission Protocol defines how a Self-Location Record enters this registry node and becomes a searchable index entry.

The registry receives an **Index Manifest**.

It does not require the submitter to surrender the full Self-Location Record.

---

## Order of Operations

**Create record → publish canonical record → complete Index Manifest → submit manifest → validate source and authority → record decision → register accepted manifest → create index entry**

Every step must remain visible.

No later step may silently replace the canonical record.

---

## Step 1: Create the Full Record

Create a Self-Location Record using the Self-Location Standard.

The full record must identify what the entity is, what it claims, what it does not claim, its source, authority, status, version, relationships, evidence, permissions, and unknown or disputed fields.

## Step 2: Publish the Canonical Record

The full record must be available at a stable canonical location controlled by the appropriate person, entity, organization, or responsible authority.

A host may store the record under delegated authority.

Hosting alone does not make the host the source or authority.

## Step 3: Complete the Index Manifest

The Index Manifest is the compact submission summary used by the registry.

It must contain enough information to identify the record, locate the canonical source, identify the responsible authority, identify the current version, expose public retrieval keys, state indexing permission, identify public relationship pointers, and record the requested visibility level.

## Step 4: Submit the Manifest

Submit through the repository's **Index Manifest Submission** issue form.

The submitter must provide the completed manifest, canonical record address, statement of authority, method by which that authority may be checked, and confirmation that the public fields may be indexed.

## Step 5: Registry Validation

The registry checks schema completeness, canonical source availability, source consistency, stated authority, public indexing permission, version consistency, visibility consistency, retrieval key relevance, relationship evidence, and whether the entry would merge, reassign, or misrepresent another record.

The registry does not claim to verify every factual or empirical statement in the full record.

## Step 6: Registry Decision

The registry records one decision:

- `pending`
- `needs-revision`
- `accepted`
- `rejected`
- `withdrawn`
- `superseded`

Acceptance means that the manifest satisfies this registry's intake requirements.

Acceptance does not mean endorsement, empirical validation, legal certification, universal recognition, AI Foundations canon status, or transfer of authority.

## Step 7: Registration

An accepted manifest is stored under:

`records/<record-id>.yaml`

The stored manifest preserves the submitted identity, canonical source, authority, version, visibility, permissions, registry decision, acceptance date, and registry node.

## Step 8: Index Entry

A searchable entry is added to `INDEX.md`.

The entry points to the canonical record, accepted manifest, and any public relationship pointers.

The index entry is a route.

It is not the canonical record itself.

---

## Update Protocol

A record holder may submit an updated manifest when the canonical record, version, authority, visibility, permissions, relationships, or status changes.

The prior accepted version must remain traceable.

Updates must not silently rewrite the earlier registry decision.

---

## Removal and Withdrawal

A record holder or authorized maintainer may request withdrawal.

The registry may remove an index entry when authority cannot be maintained, the canonical source disappears, the manifest becomes materially inaccurate, indexing permission is revoked, public information creates a privacy or safety concern, or the entry violates the standard or registry boundaries.

Removal from this registry does not erase or invalidate the canonical source record.

---

## Submission Boundary

**Record holder → authority over canonical record**

**Registry node → authority over registry acceptance and index display**

Neither authority silently replaces the other.
