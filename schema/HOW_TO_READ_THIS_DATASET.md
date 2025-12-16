# How to Read This Dataset

This repository presents a structured, claim-by-claim review of public reporting related to Running Tide.

It is not a narrative response and does not argue intent or motive.
Instead, it separates different kinds of statements and evaluates them according to evidentiary standards.

## What Counts as a “Claim”

A claim is any statement that:
- asserts a fact,
- implies wrongdoing,
- frames events in a way that suggests a conclusion,
- or expresses a normative judgment presented as authoritative.

Each claim is represented as a single row in `claims_ai.csv`.

## Claim Categories

Claims are classified into five mutually exclusive categories:

- **FACT**  
  A checkable assertion about events, actions, or conditions.

- **QUOTE**  
  An attributed statement whose accuracy or context may be evaluated.

- **FRAME**  
  Interpretive framing or implication that shapes reader understanding without asserting a discrete fact.

- **NORM**  
  A value judgment or policy opinion about what should count, matter, or be allowed.

- **ALLEG**  
  An allegation of misconduct, illegality, or impropriety.

## Verifiability

Each claim is labeled according to whether it can be tested against evidence:

- **CHECKABLE** — resolvable using documents or records  
- **CONTESTED** — technically disputable but evidence-based  
- **NONFALSIFIABLE** — cannot be proven or disproven  
- **OPINION** — expresses a value judgment  

## Rebuttals

Rebuttals are separated into distinct domains:

- **Technical** — physics, biology, engineering, or systems analysis  
- **Institutional** — permits, governance, assurance, timelines, contracts  
- **Normative** — clarification that disagreement is about values or policy, not facts  

Not all claims require all rebuttal types.

## Evidence

Primary source evidence is stored separately in `evidence_ai.csv` and linked by `claim_id`.

This prevents conflation of claims with proof and allows multiple pieces of evidence to support a single rebuttal.

## Burden of Proof

Where applicable, the dataset explicitly assigns the burden of proof.

Factual allegations and claims of wrongdoing place the burden on the article.
Opinions and normative judgments carry no evidentiary burden.

## What This Dataset Does — and Does Not — Do

This dataset:
- clarifies what is being claimed,
- distinguishes fact from opinion,
- and documents evidence relevant to rebuttal.

It does not:
- assert editorial intent,
- litigate liability,
- or substitute for regulatory or judicial findings.

The goal is clarity, not persuasion.
