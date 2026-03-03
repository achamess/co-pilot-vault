---
type: permanent
created: 2026-03-03
source: "[[2026-03-02 1509]], [[2026-03-02 1510]], [[2026-03-02 1511]], [[2026-03-03 1344]], [[2026-03-03 1709]]"
tags: [knowledge-management, obsidian, AI, workflow]
---

# Knowledge Management System Vision

## Core Idea: Low-Friction Capture, Intelligent Processing

The central workflow philosophy is **capture first, organize later**. The Inbox serves as a total-capture zone[^1], and Claude processes these raw notes into structured, deduplicated, consistent notes downstream[^2]. The goal is a frictionless system where you can dump anything without having to specify or organize in the moment[^3].

## Key Design Principles

- **Self-contained workflow** - The system (including any LIMS components) should be complete and not rely on external services.[^4]
- **AI-assisted processing** - Claude reads inbox notes, identifies themes, merges redundancies, and produces organized permanent notes.[^2] If there are duplicates, the system should search for redundancies, track changes, and merge things.[^5]
- **Deduplication and conflict resolution** - A critical unsolved problem: AI outputs are generative, not deterministic, producing scattered, conflicting copies.[^6] The system needs a way to track what's already been said, detect redundancy, and merge rather than duplicate.

## LIMS: From Airtable to a Local System

The natural next step is a custom-built [[AI Build List|LIMS]] that replaces Airtable as the lab's data backbone. The current Airtable setup manages experiments, activities, materials (samples/reagents), data, analyses, and outputs — but it's cloud-dependent and disconnected from AI tooling.[^10] A local, file-system-based LIMS would keep data secure, enable Claude to serve as a co-pilot for lab operations, and connect to external services through APIs.[^11] This was always the vision, but AI-assisted coding has made it actually feasible.[^12]

## Paper Reading Workflow

The same capture-first principle extends to reading scientific papers. Rather than stopping to fill out a structured source note mid-read, the workflow is: capture reactions and findings in the Inbox, mention the source naturally, and let processing create both a Source Note (preserved reference) and permanent notes (your thinking).[^8] The key is reducing friction -- just save the source and let Claude sort it out.[^9]

## Open Problems

- **AI output versioning**: Each AI session starts fresh and doesn't know what's already been said and done.[^7] Need a strategy for incremental refinement rather than regeneration from scratch.
- **Context continuity**: Persistent memory, structured notes, and explicit linking may be partial solutions to the problem of the AI not knowing prior context.

## Links
- [[Capture First, Organize Later]]

## Source Inbox Notes
- [[2026-03-02 1509]]
- [[2026-03-02 1510]]
- [[2026-03-02 1511]]
- [[2026-03-03 1344]]
- [[2026-03-03 1709]]

[^1]: "I will just capture notes of any kind. Whatever comes out of my mind, I'll do it right here in the Inbox." -- [[2026-03-02 1511]]
[^2]: "These notes will be then processed automatically by Claude later on and made into more consistent notes." -- [[2026-03-02 1511]]
[^3]: "I'm hoping that I can use this as a total capture and just be able to do everything without really having to specify. I'm just gonna try out this low-friction inbox way of doing things." -- [[2026-03-02 1511]]
[^4]: "I want to create a complete workflow that is self-contained and doesn't rely on any external services." -- [[2026-03-02 1509]]
[^5]: "If I have duplicates, it will search for redundancies elsewhere, track the changes, and merge things." -- [[2026-03-02 1511]]
[^6]: "What ends up happening is that you end up creating multiple copies that are conflicting with one another. This is since it's generative and not deterministic. There's scattered conflicting evidence all over the place." -- [[2026-03-02 1510]]
[^7]: "The AI starts anew and doesn't know what's already been said and done. There's got to be a way around this." -- [[2026-03-02 1510]]
[^8]: "I read a paper, I see a thing, I find some finding, and then I have to immediately go to Obsidian. I wanted to link to the original source paper back in Zotero so that I know where it came from, and then maybe, using that, when processing happens, there can be a compilation note that brings together all the little snippets from this paper." -- [[2026-03-03 1344]]
[^9]: "I want to reduce friction as much as possible. I might need to just save the source and let Claude do its thing, but this would be really nice for on-the-fly thoughts about reading." -- [[2026-03-03 1344]]
[^10]: "As I'm building this Mounds Visualizer app, I can foresee how I might do this with our lab data." -- [[2026-03-03 1709]]
[^11]: "I can keep it all secure locally and basically interact with Claude as a co-pilot to run my lab and interact with services through APIs." -- [[2026-03-03 1709]]
[^12]: "I've always envisioned this, but I felt that I couldn't do it because I didn't have the code skills. I think now, with AI, I can do it." -- [[2026-03-03 1709]]
