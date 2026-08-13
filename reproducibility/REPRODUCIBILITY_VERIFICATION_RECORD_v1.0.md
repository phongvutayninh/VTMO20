# VTMO20 Core v1.0.0 — Reproducibility Verification Record

## 1. Record Identification

- **Ontology:** Vietnamese Traditional Medicinal Plant Ontology (VTMO20)
- **Release:** Core v1.0.0
- **Record:** Reproducibility Verification Record
- **Record version:** 1.0
- **Verification date:** 2026-08-13
- **Verifier:** Trần Phong Vũ
- **Repository:** https://github.com/phongvutayninh/VTMO20
- **Release tag:** v1.0.0

---

## 2. Verification Scope

This record documents the execution and results of reproducibility
verification for the public release of VTMO20 Core v1.0.0.

The verification covers:

1. public release accessibility;
2. independent RDF/XML artifact download;
3. SHA-256 integrity verification;
4. independent ontology opening and inspection in Protégé;
5. ontology identifier verification;
6. version identifier verification;
7. structural ontology statistics;
8. public release stability;
9. reproducibility evidence availability.

Persistent W3ID resolution is excluded from the completed checks in this
record because the corresponding W3ID pull request is awaiting upstream
merge. Final redirect verification will be recorded separately after the
W3ID configuration becomes active.

---

## 3. Public Artifact

- **Artifact:** `VTMO20_Core_v1.0_Public.rdf`
- **Serialization:** RDF/XML
- **Release:** VTMO20 Core v1.0.0
- **Release tag:** `v1.0.0`
- **Release URL:** https://github.com/phongvutayninh/VTMO20/releases/tag/v1.0.0
- **Artifact URL:** https://github.com/phongvutayninh/VTMO20/releases/download/v1.0.0/VTMO20_Core_v1.0_Public.rdf

### Result

**PASS**

The ontology artifact was independently downloaded from the public GitHub
Release without relying on the local development copy.

---

## 4. SHA-256 Integrity Verification

### Algorithm

`SHA-256`

### Expected checksum

`B7B699FA8077C8695E376D5E4017D5F2A824D33CE9920EE12AAA6A8EB485A4A5`

### Observed checksum

`B7B699FA8077C8695E376D5E4017D5F2A824D33CE9920EE12AAA6A8EB485A4A5`

### Checksum manifest

`reproducibility/CHECKSUMS.sha256`

### Result

**PASS**

The independently calculated SHA-256 checksum exactly matched the checksum
recorded in the public reproducibility package.

---

## 5. RDF/XML and Protégé Verification

The independently downloaded ontology artifact was opened successfully in
Protégé.

Protégé recognized the ontology and exposed its ontology metadata,
entities, properties, individuals, and ontology metrics.

### Result

**PASS**

No RDF/XML loading failure was observed during the independent inspection.

---

## 6. Ontology Identifier Verification

### Ontology IRI

`https://w3id.org/vtmo/ontology`

### Version IRI

`https://w3id.org/vtmo/ontology/1.0.0`

The identifiers displayed by Protégé matched the identifiers declared for
VTMO20 Core v1.0.0.

### Result

**PASS**

---

## 7. Structural Verification

The independently opened ontology reported the following core structural
statistics:

| Metric | Verified value |
|---|---:|
| Axioms | 479 |
| Logical axioms | 122 |
| Declaration axioms | 95 |
| Classes | 14 |
| Object properties | 10 |
| Data properties | 10 |
| Named individuals | 55 |
| Annotation properties | 12 |

These values correspond to the ontology artifact independently downloaded
from the public release and inspected in Protégé.

### Result

**PASS**

---

## 8. Public Release Verification

The ontology is associated with the public GitHub Release:

- **Release title:** VTMO20 Core v1.0.0
- **Tag:** `v1.0.0`
- **Release date:** 2026-08-13
- **Public artifact:** `VTMO20_Core_v1.0_Public.rdf`

The release provides a version-specific public distribution point for the
ontology artifact.

### Result

**PASS**

---

## 9. Reproducibility Evidence Package

The following reproducibility resources are maintained in the repository:

- `CHECKSUMS.sha256`
- `RELEASE_METADATA_v1.0.0.md`
- `REPRODUCIBILITY_PROTOCOL_v1.0.md`
- `REPRODUCIBILITY_VERIFICATION_RECORD_v1.0.md`

Together, these resources document:

- artifact identity;
- release identity;
- integrity verification;
- verification procedure;
- verification execution;
- reproducibility status.

### Result

**PASS**

---

## 10. Persistent Identifier Verification

### Namespace

`https://w3id.org/vtmo/`

### Canonical ontology IRI

`https://w3id.org/vtmo/ontology`

### Version-specific IRI

`https://w3id.org/vtmo/ontology/1.0.0`

### Current status

**PENDING FINAL REDIRECT VERIFICATION**

The W3ID configuration has been submitted through an upstream pull request.
Final resolution testing must be performed after the pull request is merged
and the namespace becomes active.

This pending external infrastructure step does not alter the verified
integrity of the VTMO20 Core v1.0.0 release artifact.

---

## 11. Verification Summary

| Verification item | Status |
|---|---|
| Public GitHub Release accessible | PASS |
| RDF/XML artifact independently downloadable | PASS |
| SHA-256 checksum independently calculated | PASS |
| SHA-256 checksum matches manifest | PASS |
| RDF/XML opens successfully in Protégé | PASS |
| Ontology IRI verified | PASS |
| Version IRI verified | PASS |
| Core structural statistics inspected | PASS |
| Release tag identified | PASS |
| Reproducibility documentation available | PASS |
| Final W3ID redirect verification | PENDING |

---

## 12. Overall Reproducibility Status

**VERIFIED — W3ID FINAL REDIRECT CHECK PENDING**

VTMO20 Core v1.0.0 is publicly accessible, independently downloadable,
integrity-verifiable, RDF/XML parseable, independently inspectable, and
associated with a versioned public release and reproducibility evidence
package.

The remaining external verification concerns only final W3ID persistent
identifier resolution after upstream activation.

---

## 13. Record Provenance

- **Record:** VTMO20 Reproducibility Verification Record
- **Record version:** 1.0
- **Created:** 2026-08-13
- **Associated release:** VTMO20 Core v1.0.0
- **Creator:** Trần Phong Vũ
- **Maintainer:** Trần Phong Vũ
- **Purpose:** To preserve an auditable execution record of independent
  reproducibility verification for the VTMO20 Core v1.0.0 public release.
