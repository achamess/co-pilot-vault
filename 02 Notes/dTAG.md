---
type: entity
entity_type: technique
aliases: [dTAG system, dTAG-V1, dTAG-13, DTAG, dTAG PROTAC]
created: 2026-03-03
tags: [entity, targeted-protein-degradation, PROTAC, VHL]
---

# dTAG

## What It Is
The dTAG system is a chemical biology tool for acute, reversible, and selective protein degradation. It uses bifunctional molecules to degrade FKBP12(F36V)-tagged proteins. Two main variants exist: **dTAG-V1** recruits [[VHL]] as the E3 ligase, while **dTAG-13** recruits CRBN (cereblon). Both require genetic tagging of the target protein with an FKBP12(F36V) degron.

## What I Know
- dTAG-V1 recruits [[VHL]] as its E3 ligase, so [[VHL]] expression in the target cell type is a prerequisite.[^1]
- [[VHL]] is confirmed present in mouse DRG neurons, validating that the dTAG system should work in sensory neurons.[^2]
- Planning an in vivo experiment: inject dTAG-13 into mouse, then perform capsaicin test with automated behavioral analysis via DeepLabCut.[^3]

## Open Questions
- What degradation kinetics can be expected in DRG neurons in vivo?
- Has dTAG-V1 been used in peripheral nervous system models before?
- What is the best delivery route for dTAG-V1 to reach DRG?

## Links
- [[VHL]]
- [[VHL in DRG Neurons and the dTAG System]]
- [[NaV1.8]]
- [[dTAG-13 Capsaicin Experiment Plan]]

[^1]: "VHL is in mouse DRG neurons which I will need to leverage for my purposes with the DTAG system using the DTAG V1 PROTAC." -- [[2026-03-03 1357]]
[^2]: "They show that VHL E3 ligase is present in mouse dorsal root ganglion neurons." -- [[2026-03-03 1357]]
[^3]: "We're talking about using video analysis for mouse behavior, in particular for capsaicin. We want to do a test where we inject the DTAG-13 into the mouse and then do capsaicin. I want to use this automated video analysis based on DeepLabCut." -- [[2026-03-03 1421]]
