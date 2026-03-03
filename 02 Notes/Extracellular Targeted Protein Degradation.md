---
type: permanent
created: 2026-03-03
source: "[[2026-03-03 1711]]"
tags: [targeted-protein-degradation, protein-design, pain, ion-channel]
---

# Extracellular Targeted Protein Degradation

## The Idea

An extracellular [[targeted protein degradation]] strategy for [[NaV1.8]] and [[NaV1.9]] — ion channels that sit on the cell surface. The concept is a HiBiT-like effector: a designed protein binder that engages the extracellular domain of the target and triggers its degradation, potentially through lysosomal pathways or receptor-mediated internalization.[^1]

## How It Relates to Other Degrader Work

This is **related but distinct** from the [[NIH PTDP Grant - NaV1.8 Covalent Degrader|intracellular covalent degrader]] approach being developed under the NIH PTDP grant with Rob Gereau. Both target NaV channels, but the modalities differ:

| Approach | Target access | Mechanism | Stage |
|----------|--------------|-----------|-------|
| **Covalent degrader** (PTDP grant) | Intracellular | Small-molecule PROTAC/molecular glue | Grant planning |
| **Extracellular TPD** (this) | Extracellular domain | Designed protein binder | Early concept |
| **[[dTAG]] system** | Intracellular (requires genetic tag) | Bifunctional degrader | Active experiments |

## Enabling Technologies

The protein binder design relies on computational tools ([[BindCraft]], [[BoltzGen]], [[Rosetta]]) and services like [[AdaptyvBio]] that can take designs from in silico to wet bench.[^2] Currently collaborating with a group at Washington University on the computational design side.

## Open Questions
- Which extracellular epitopes on [[NaV1.8]]/[[NaV1.9]] are accessible and druggable?
- What degradation mechanism would be engaged — lysosomal targeting, crosslinking to endocytic machinery?
- What is the pharmacokinetic profile of a protein binder vs. a small molecule for peripheral nerve targets?
- How does this compare to antibody-based approaches?

## Links
- [[NaV1.8]]
- [[NaV1.9]]
- [[AdaptyvBio]]
- [[dTAG]]
- [[NIH PTDP Grant - NaV1.8 Covalent Degrader]]

## Source Inbox Notes
- [[2026-03-03 1711]]

[^1]: "I want to make an extracellular TPD effector, like a HiBiT, but for NaV1.8/NaV1.9." -- conversation, 2026-03-03
[^2]: "I definitely think we'll be using it for our express protein binders." -- [[2026-03-03 1711]]
