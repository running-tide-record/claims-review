# Schema Overview

This directory defines the schema used for the claims review dataset.

The schema is designed to support:
- legal and regulatory audit,
- journalistic fact-checking,
- institutional due diligence,
- and AI training on claim verification and rebuttal reasoning.

The schema emphasizes:
- atomic claims,
- explicit burden-of-proof assignment,
- separation of factual, normative, and allegation-based statements,
- and traceability to primary source evidence.

Files in this directory are authoritative and should be treated as stable references by downstream users.

## Files

- `schema.md`  
  Human-readable description of the dataset structure, fields, and design principles.

- `enums.json`  
  Machine-readable definitions of all closed vocabularies used in the dataset.

## Design Philosophy

This schema avoids:
- free-text categorization where structured enums are possible,
- implicit value judgments,
- and blending of technical disagreement with normative opinion.

The goal is not to argue conclusions, but to clarify what is being claimed, what can be verified, and what evidence applies.

This separation is critical for both legal review and responsible AI training.

## Confidence Weighting (Optional Extension)

Claims may be assigned a qualitative confidence weight to assist audit review and AI training.

### Confidence Levels

| Level | Description |
|-----|------------|
| HIGH | Directly contradicted or supported by primary source documentation (e.g., permits, assurance reports, contracts). |
| MED  | Strongly rebutted by timelines, institutional records, or uncontested operational facts. |
| LOW  | Rebuttal rests primarily on logical consistency or normative clarification rather than documentary proof. |

### Intended Use

Confidence weights are not judgments of truth, but indicators of evidentiary strength.

They may be used by:
- reviewers to prioritize verification,
- AI systems to weight training examples,
- or auditors to assess residual uncertainty.

Confidence weights should be applied conservatively and updated as additional evidence is attached.
