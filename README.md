# Claims Review (Public Record)

This repository contains a structured, claim-by-claim factual review of public reporting related to Running Tide.

The purpose of this repository is to:
- distinguish verifiable factual claims from opinion, framing, and allegations,
- document rebuttals with traceable primary-source evidence,
- and provide a transparent public record suitable for audit, due diligence, and machine analysis.

This repository does not assess editorial intent, tone, or motive.
It exists solely to clarify the factual record.

Maintained by Marty Odlin in a personal capacity.

---

## Repository Structure

### Data
- `csv/claims_ai_v1_1.csv`  
  Canonical claims table with confidence weights and explicit burden-of-proof assignments.

- `csv/evidence_ai.csv`  
  Primary-source evidence mapped to individual claims.

- `csv/confidence_heatmap.csv`  
  Summary distribution of evidentiary strength (HIGH / MED / LOW).

### Documentation
- `HOW_TO_READ_THIS_DATASET.md`  
  One-page guide explaining claim categories, rebuttal domains, and evidentiary standards.

- `schema/`  
  Dataset schema, closed vocabularies, and design principles.

### Exhibits
- `exhibits/`  
  Primary source documents referenced by the claims inventory (permits, assurance reports, protocols).

---

## Methodology Summary

- Each row in the claims dataset represents **one atomic claim**.
- Claims are categorized into closed classes (FACT, QUOTE, FRAME, NORM, ALLEG).
- Rebuttals are separated into technical, institutional, and normative domains.
- Where applicable, the burden of proof is explicitly assigned.
- Confidence weights reflect the strength of available primary evidence.

---

## Intended Uses

This repository is intended for:
- journalistic fact-checking,
- legal and regulatory review,
- institutional due diligence,
- and AI training on structured claim evaluation.

It is not intended to serve as legal advice, advocacy, or a substitute for judicial findings.

---

## Versioning

Claims and evidence may be updated as additional primary sources are surfaced.
Versioned CSV files preserve a public change history.
