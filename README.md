# VTMO20

## Vietnamese Traditional Medicinal Plant Ontology

**VTMO20 (Vietnamese Traditional Medicinal Plant Ontology)** is a competency-driven OWL ontology developed to support the structured representation and semantic retrieval of Vietnamese traditional medicinal plant knowledge.

VTMO20 provides a machine-readable semantic representation of medicinal plant knowledge, including medicinal substances, scientific names, plant families, medicinal parts, tastes, traditional properties, meridians, therapeutic functions, indications, dosage specifications, and administration methods.

## Ontology Information

- **Ontology name:** Vietnamese Traditional Medicinal Plant Ontology
- **Acronym:** VTMO20
- **Core version:** 1.0.0
- **Identifier:** VTMO20-Core-v1.0
- **Ontology IRI:** `https://w3id.org/vtmo/ontology`
- **Version IRI:** `https://w3id.org/vtmo/ontology/1.0.0`
- **Language:** English and Vietnamese
- **Creator:** Trần Phong Vũ
- **Format:** OWL / RDF/XML
- **Public ontology file:** `VTMO20_Core_v1.0_Public.rdf`

## Ontology Scope

VTMO20 represents structured knowledge concerning Vietnamese traditional medicinal plants and their principal semantic relationships.

The current core ontology includes concepts and relations concerning:

- Medicinal substances
- Scientific names
- Plant families
- Medicinal parts
- Tastes
- Traditional medicinal properties
- Meridians
- Therapeutic functions
- Diseases and indications
- Dosage specifications
- Administration methods

The ontology is designed as a foundation for semantic retrieval, knowledge graph construction, competency-question evaluation, and future ontology-based intelligent applications involving Vietnamese traditional medicinal plant knowledge.

## Current Core Statistics

VTMO20 Core v1.0.0 currently contains:

| Ontology component | Count |
|---|---:|
| RDF triples | 499 |
| OWL classes | 14 |
| Object properties | 10 |
| Datatype properties | 10 |
| Named individuals | 55 |

These statistics correspond to the validated public core release.

## Competency-Driven Development

VTMO20 was developed using a competency-driven ontology engineering workflow.

The development process includes:

1. Curated source knowledge
2. Competency-question definition
3. Ontology modelling
4. RDF/OWL implementation
5. SPARQL-based validation
6. Reproducibility checking
7. Provenance-aware evidence management

The ontology has been tested using competency questions and SPARQL queries in Apache Jena Fuseki.

## Example Knowledge Representation

The current public core contains a medicinal substance representing **Mentha arvensis L. (Bạc hà)** and semantic relations connecting it to knowledge entities such as:

- Plant family
- Scientific name
- Medicinal part
- Taste
- Traditional property
- Meridian
- Therapeutic function
- Indication
- Dosage specification
- Administration method

This provides a compact reference case for validating semantic retrieval across the ontology.

## Repository Contents

```text
VTMO20/
├── README.md
└── VTMO20_Core_v1.0_Public.rdf
