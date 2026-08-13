# VTMO20 Core v1.0.0 — Reproducibility Verification Protocol

## 1. Purpose

This protocol defines a reproducible procedure for independently verifying the public release of the Vietnamese Traditional Medicinal Plant Ontology (VTMO20) Core v1.0.0.

The protocol is intended to allow an independent researcher to:

1. locate the public ontology release;
2. download the RDF/XML artifact independently;
3. verify artifact integrity using SHA-256;
4. parse and inspect the ontology;
5. verify ontology identification metadata;
6. verify core ontology statistics;
7. inspect the ontology independently in Protégé;
8. verify the status of the persistent identifier when available.

---

## 2. Target Release

- **Ontology:** Vietnamese Traditional Medicinal Plant Ontology
- **Acronym:** VTMO20
- **Release:** Core v1.0.0
- **Version:** 1.0.0
- **Release tag:** v1.0.0
- **Serialization:** RDF/XML
- **Artifact:** `VTMO20_Core_v1.0_Public.rdf`

### Canonical identifiers

- **Ontology IRI:** `https://w3id.org/vtmo/ontology`
- **Version IRI:** `https://w3id.org/vtmo/ontology/1.0.0`

---

## 3. Public Sources

### Source repository

`https://github.com/phongvutayninh/VTMO20`

### Public release

`https://github.com/phongvutayninh/VTMO20/releases/tag/v1.0.0`

### Direct release artifact

`https://github.com/phongvutayninh/VTMO20/releases/download/v1.0.0/VTMO20_Core_v1.0_Public.rdf`

### Public checksum manifest

`reproducibility/CHECKSUMS.sha256`

### Release metadata record

`reproducibility/RELEASE_METADATA_v1.0.0.md`

---

## 4. Expected SHA-256

The expected SHA-256 checksum for the public RDF/XML artifact is:

`B7B699FA8077C8695E376D5E4017D5F2A824D33CE9920EE12AAA6A8EB485A4A5`

Expected artifact:

`VTMO20_Core_v1.0_Public.rdf`

The verification succeeds only when the independently calculated SHA-256 checksum exactly matches the value recorded above and in `CHECKSUMS.sha256`.

---

## 5. Step 1 — Independent Artifact Download

Download:

`VTMO20_Core_v1.0_Public.rdf`

from the public GitHub Release rather than relying on a local development copy.

### Expected result

The RDF/XML artifact is publicly downloadable without requiring access to the ontology development environment.

### Verification criterion

**PASS** if the artifact can be downloaded independently from the public release.

---

## 6. Step 2 — SHA-256 Integrity Verification

### Windows PowerShell

Run:

    Get-FileHash ".\VTMO20_Core_v1.0_Public.rdf" -Algorithm SHA256

If the browser or operating system automatically renames a duplicate download, use the actual downloaded filename, for example:

    Get-FileHash ".\VTMO20_Core_v1.0_Public (1).rdf" -Algorithm SHA256

### Expected SHA-256

    B7B699FA8077C8695E376D5E4017D5F2A824D33CE9920EE12AAA6A8EB485A4A5

### Verification criterion

**PASS** only if the calculated SHA-256 exactly matches the expected SHA-256.

A filename change introduced by the local operating system does not affect the verification result; the checksum is calculated from the file content.

---

## 7. Step 3 — RDF/XML Parsing Verification

Parse the downloaded ontology artifact using an RDF/OWL-compatible parser or ontology tool.

A suitable validation environment may include Apache Jena/Fuseki or another standards-compatible RDF parser.

### Expected result

The artifact is successfully parsed as RDF/XML without a syntax failure that prevents ontology loading.

### Verification criterion

**PASS** if the public artifact can be parsed successfully as RDF/XML.

---

## 8. Step 4 — Ontology Identification Verification

Inspect the ontology header.

The following identifiers are expected:

- **Ontology IRI:** `https://w3id.org/vtmo/ontology`
- **Version IRI:** `https://w3id.org/vtmo/ontology/1.0.0`

Expected descriptive metadata includes:

- Vietnamese Traditional Medicinal Plant Ontology;
- VTMO20 Core release identification;
- creator information;
- English and Vietnamese language metadata.

### Verification criterion

**PASS** if the ontology and version identifiers match the release metadata record.

---

## 9. Step 5 — Core Statistics Verification

The validated VTMO20 Core v1.0.0 release records the following RDF/OWL statistics:

- **RDF triples:** 499
- **OWL classes:** 14
- **Object properties:** 10
- **Datatype properties:** 10
- **Named individuals:** 55

### Important note

RDF triple counts and OWL axiom counts are different metrics and must not be treated as interchangeable.

For example, an ontology editor may report an OWL axiom count that differs from the RDF triple count while still representing the same RDF/XML artifact.

### Verification criterion

**PASS** if the ontology structural counts relevant to the selected inspection tool are consistent with the validated release record.

---

## 10. Step 6 — Independent Protégé Inspection

Open the independently downloaded RDF/XML artifact in Protégé.

Inspect:

1. ontology header;
2. ontology IRI;
3. version IRI;
4. class count;
5. object property count;
6. data property count;
7. individual count;
8. ontology annotations.

### Expected Protégé observations

- **Class count:** 14
- **Object property count:** 10
- **Data property count:** 10
- **Individual count:** 55

### Verification criterion

**PASS** if Protégé successfully opens the downloaded artifact and the ontology identification and structural statistics are consistent with the validated release.

---

## 11. Step 7 — Public Release Stability Verification

Confirm that:

- release tag `v1.0.0` exists;
- release title identifies `VTMO20 Core v1.0.0`;
- `VTMO20_Core_v1.0_Public.rdf` remains attached to the release;
- the independently downloaded artifact continues to produce the expected SHA-256 checksum.

### Verification criterion

**PASS** if the release artifact remains publicly retrievable and checksum-stable.

The released v1.0.0 artifact should not be silently replaced. Ontology changes should be published under a new version.

---

## 12. Step 8 — Persistent Identifier Verification

The intended persistent identifiers are:

- `https://w3id.org/vtmo/ontology`
- `https://w3id.org/vtmo/ontology/1.0.0`

At the time this protocol was created, the W3ID configuration had been submitted upstream and final redirect verification was pending merge.

Therefore, persistent-identifier resolution is treated separately from artifact-integrity verification.

### Verification after W3ID activation

After the W3ID configuration is merged upstream:

1. open the canonical ontology IRI;
2. confirm successful HTTP resolution;
3. verify that the canonical identifier resolves to the intended VTMO20 public ontology artifact;
4. repeat the procedure for the version-specific IRI;
5. download the resolved artifact if applicable;
6. calculate SHA-256;
7. compare it with the release checksum.

### Verification criterion

**PENDING** until the W3ID pull request is merged and redirect resolution is independently verified.

---

## 13. Verification Matrix

| Verification Item | Expected Result | Status at Protocol Creation |
|---|---|---|
| Public GitHub Release | Accessible | VERIFIED |
| Independent RDF/XML download | Successful | VERIFIED |
| SHA-256 integrity | Exact match | VERIFIED |
| RDF/XML parsing | Successful | VERIFIED |
| Ontology metadata inspection | Successful | VERIFIED |
| Core ontology statistics | Consistent | VERIFIED |
| Protégé independent opening | Successful | VERIFIED |
| Release stability | Artifact identified and checksum recorded | VERIFIED |
| W3ID canonical redirect | Correct resolution | PENDING |
| W3ID version redirect | Correct resolution | PENDING |

---

## 14. Reproducibility Decision Rule

The VTMO20 Core v1.0.0 release is considered reproducible at the public-artifact level when all of the following conditions are satisfied:

1. the release can be located publicly;
2. the RDF/XML artifact can be independently downloaded;
3. the SHA-256 checksum matches the public manifest;
4. the RDF/XML artifact can be parsed;
5. ontology identification metadata can be independently inspected;
6. core structural statistics are consistent with the release record;
7. the ontology can be independently opened in Protégé.

Persistent identifier resolution is an additional verification layer and does not replace artifact-level integrity verification.

---

## 15. Current Verification Status

Based on the public release verification performed for VTMO20 Core v1.0.0:

**Public Artifact Reproducibility: VERIFIED**

**Artifact Integrity: VERIFIED**

**Independent Protégé Inspection: VERIFIED**

**W3ID Persistent Resolution: PENDING UPSTREAM MERGE**

The final W3ID verification should be recorded after upstream activation without altering the historical integrity evidence of the v1.0.0 release.

---

## 16. Protocol Provenance

- **Protocol:** VTMO20 Reproducibility Verification Protocol
- **Protocol version:** 1.0
- **Created:** 2026-08-13
- **Associated ontology:** VTMO20 Core v1.0.0
- **Creator:** Trần Phong Vũ
- **Repository:** `phongvutayninh/VTMO20`
- **Purpose:** Independent verification of accessibility, integrity, inspectability, release stability, and reproducibility of the public VTMO20 ontology artifact.
