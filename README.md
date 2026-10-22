# AI-Readiness Index

**An open, vendor-neutral research prototype for evaluating whether a dataset is fit for a specific AI use case.**

A dataset can be discoverable, documented, and accompanied by valid metadata without necessarily being suitable for a particular AI application. The AI-Readiness Index explores how to evaluate that suitability using measurable dataset properties, documented evidence, and intended-use-specific requirements.

## What does it assess?

Five dimensions:

1. **Data quality:** completeness, validity, accuracy, timeliness.
2. **Governance and provenance:** source, lineage, ownership, stewardship, policy.
3. **Privacy:** sensitive information, purpose, minimization, consent and masking evidence.
4. **Security and integrity:** access, encryption, integrity, exposure evidence.
5. **Operational and economic sustainability:** duplication, efficiency and illustrative cost signals.

An assessment combines the **dataset**, an **intended-use profile** (use case, risk tier, rules, weights, required conditions), and **supplied metadata**. It produces rule findings, a composite score, evidence provenance, and a disposition subject to mandatory conditions.

## Two motivating use cases

- **One dataset, different decisions.** In a synthetic prototype using 204 records, the same dataset met an illustrative aggregate reporting profile (99.67/100) but was blocked under an illustrative individual lending-decision profile (82.60/100; six unmet required conditions). These numbers demonstrate the method, not measured real-world safety or regulatory suitability.
- 
- **Readiness before AI pipeline adoption.** Detect missing evidence, data-quality problems, or failed required controls before relying on data for an AI workflow. A strong aggregate score cannot override an unmet mandatory condition.

## Relation to existing efforts

This project is intended to **complement**, not replace, ISO/IEC 5259, the NIST AI Risk Management Framework, metadata/catalog systems, and dataset publication and provenance initiatives such as **SetGo**. The research emphasis is direct observations about dataset contents, evidence qualified by origin (computed, declared, or estimated), and assessments relative to intended use. The precise division of responsibilities and potential interoperability with other projects should be validated collaboratively.

## Project status

**Early-stage research demonstrator; independent validation pending.** Existing prototype observations use synthetic data and illustrative, uncalibrated profiles. This public repository contains a conceptual overview only; it does not publish the prototype source or claim certification, safety, or legal compliance.

## Learn more

- [Public overview webpage](docs/index.html) (also deployable with GitHub Pages)
- [Research questions](docs/RESEARCH_QUESTIONS.md)

## Collaboration

Feedback from contributors and other research communities is welcome, particularly around intended-use profiles, measurable dataset criteria, evidence provenance, evaluation protocols, and alignment with existing efforts.

## Licensing and provenance

This is an independently prepared public-facing description of an early research concept. No code or confidential material from the private implementation repository is included. Licensing for future software or datasets will be designated separately.
