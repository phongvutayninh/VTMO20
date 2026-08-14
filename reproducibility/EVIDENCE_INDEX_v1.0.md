# VTMO20 Core v1.0.0 — Reproducibility Evidence Index

## 1. Index Identification

- **Ontology:** Vietnamese Traditional Medicinal Plant Ontology (VTMO20)
- **Release:** Core v1.0.0
- **Index:** Reproducibility Evidence Index
- **Index version:** 1.0
- **Created:** 2026-08-14
- **Repository:** https://github.com/phongvutayninh/VTMO20
- **Release tag:** v1.0.0
- **Maintainer:** Trần Phong Vũ

---

## 2. Purpose

This document provides a single audit entry point for the reproducibility
evidence associated with VTMO20 Core v1.0.0.

It connects the public ontology artifact, integrity evidence, release
metadata, verification protocol, and executed verification record into a
traceable evidence chain.

The index does not replace the individual evidence records. Its purpose is
to identify, organize, and connect them for independent inspection,
verification, and future scholarly reuse.

---

## 3. Public Ontology Artifact

### Primary release artifact

`VTMO20_Core_v1.0_Public.rdf`

- **Serialization:** RDF/XML
- **Release:** VTMO20 Core v1.0.0
- **Tag:** `v1.0.0`
- **Release page:**  
  https://github.com/phongvutayninh/VTMO20/releases/tag/v1.0.0
- **Direct artifact:**  
  https://github.com/phongvutayninh/VTMO20/releases/download/v1.0.0/VTMO20_Core_v1.0_Public.rdf

### Role in the evidence package

This file is the versioned public ontology artifact to which the
reproducibility evidence refers.

---

## 4. Evidence Components

| ID | Evidence component | File | Function | Status |
|---|---|---|---|---|
| EV-01 | Public ontology artifact | `VTMO20_Core_v1.0_Public.rdf` | Versioned RDF/XML ontology artifact | VERIFIED |
| EV-02 | Integrity manifest | `CHECKSUMS.sha256` | Records the reference SHA-256 checksum | VERIFIED |
| EV-03 | Release metadata record | `RELEASE_METADATA_v1.0.0.md` | Records release identity, metadata, statistics, provenance, and reproducibility status | VERIFIED |
| EV-04 | Reproducibility protocol | `REPRODUCIBILITY_PROTOCOL_v1.0.md` | Defines the reproducibility verification procedure | VERIFIED |
| EV-05 | Verification record | `REPRODUCIBILITY_VERIFICATION_RECORD_v1.0.md` | Records execution and results of reproducibility verification | VERIFIED |
| EV-06 | Persistent identifier configuration | W3ID `/vtmo/` configuration | Provides persistent ontology and version IRI resolution | PENDING FINAL REDIRECT VERIFICATION |

---

## 5. Integrity Evidence

### SHA-256 algorithm

`SHA-256`

### Verified checksum

`B7B699FA8077C8695E376D5E4017D5F2A824D33CE9920EE12AAA6A8EB485A4A5`

### Checksum manifest

`reproducibility/CHECKSUMS.sha256`

The checksum was independently calculated from the ontology artifact
downloaded from the public GitHub Release and matched against the checksum
recorded in the repository.

### Status

**VERIFIED**

---

## 6. Evidence Chain

The reproducibility evidence chain for VTMO20 Core v1.0.0 is:

`Public Release Artifact`

↓

`SHA-256 Integrity Manifest`

↓

`Release Metadata Record`

↓

`Reproducibility Verification Protocol`

↓

`Reproducibility Verification Record`

↓

`Reproducibility Evidence Index`

This chain separates:

- the object being verified;
- integrity evidence;
- descriptive release metadata;
- the verification method;
- the execution record;
- the audit entry point.

This separation supports transparent inspection and reduces ambiguity
between specification, execution, and evidence.

---

## 7. Verification Coverage

| Verification dimension | Evidence | Status |
|---|---|---|
| Public accessibility | GitHub Release + EV-05 | VERIFIED |
| Independent download | EV-05 | VERIFIED |
| RDF/XML availability | EV-01 + EV-05 | VERIFIED |
| SHA-256 integrity | EV-02 + EV-05 | VERIFIED |
| Ontology loading in Protégé | EV-05 | VERIFIED |
| Ontology IRI inspection | EV-03 + EV-05 | VERIFIED |
| Version IRI inspection | EV-03 + EV-05 | VERIFIED |
| Structural statistics inspection | EV-03 + EV-05 | VERIFIED |
| Release identification | EV-03 | VERIFIED |
| Verification procedure | EV-04 | VERIFIED |
| Verification execution | EV-05 | VERIFIED |
| Persistent W3ID resolution | EV-06 | PENDING |

---

## 8. Persistent Identifier Status

### Persistent namespace

`https://w3id.org/vtmo/`

### Canonical ontology IRI

`https://w3id.org/vtmo/ontology`

### Version-specific IRI

`https://w3id.org/vtmo/ontology/1.0.0`

### Current status

**PENDING FINAL REDIRECT VERIFICATION**

The W3ID configuration has been submitted upstream.

Final persistent-identifier resolution must be tested only after the
corresponding W3ID pull request has been merged and the configuration has
become active.

Until that event occurs, this evidence package does not claim successful
W3ID resolution.

---

## 9. Audit Procedure

An independent reviewer can inspect the reproducibility package using the
following sequence:

1. access the VTMO20 Core v1.0.0 GitHub Release;
2. independently download `VTMO20_Core_v1.0_Public.rdf`;
3. compute its SHA-256 checksum;
4. compare the result with `CHECKSUMS.sha256`;
5. inspect `RELEASE_METADATA_v1.0.0.md`;
6. inspect `REPRODUCIBILITY_PROTOCOL_v1.0.md`;
7. inspect `REPRODUCIBILITY_VERIFICATION_RECORD_v1.0.md`;
8. independently open the RDF/XML artifact in an ontology editor such as
   Protégé;
9. inspect the ontology identifiers and structural components;
10. after W3ID activation, independently test the canonical and
    version-specific persistent identifiers.

---

## 10. Package Status

### Current reproducibility package status

**VERIFIED — W3ID FINAL REDIRECT CHECK PENDING**

The VTMO20 Core v1.0.0 reproducibility evidence package currently provides:

- a publicly accessible versioned ontology artifact;
- an independently verified SHA-256 checksum;
- a public checksum manifest;
- release metadata;
- a documented reproducibility protocol;
- an executed verification record;
- a centralized evidence index.

The remaining external dependency is final W3ID redirect activation and
verification.

---

## 11. Freeze Policy

The evidence records associated with VTMO20 Core v1.0.0 represent the
verification state of this specific ontology release.

After final review, the package should be treated as a frozen
release-specific reproducibility record.

Substantive changes to the ontology artifact require a new ontology
release and corresponding reproducibility evidence.

Final W3ID activation may be documented as an additional verification
event without altering the historical integrity-verification results for
the released artifact.

---

## 12. Provenance

- **Record:** VTMO20 Reproducibility Evidence Index
- **Version:** 1.0
- **Created:** 2026-08-14
- **Associated ontology release:** VTMO20 Core v1.0.0
- **Creator:** Trần Phong Vũ
- **Maintainer:** Trần Phong Vũ
- **Purpose:** To provide a centralized, auditable index of the
  reproducibility evidence associated with VTMO20 Core v1.0.0.
