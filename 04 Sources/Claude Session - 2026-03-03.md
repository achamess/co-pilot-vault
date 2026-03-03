---
type: source
source_type: claude-session
date: 2026-03-03
created: 2026-03-03
tags: [claude-session]
---

# Claude Session - 2026-03-03

## Decisions Made
- **Single capture point**: Inbox is the only capture zone; removed Capture section from [[Daily Note]] template
- **Capture first, organize later**: Voice-dump thoughts into Inbox, Claude processes into structured notes
- **Source notes vs permanent notes**: Sources preserve external material as-is; permanent notes are your thinking/synthesis
- **Meeting notes live in `04 Sources/`** with `source_type: meeting` — fewer folders, let metadata organize
- **Paper reading workflow**: Capture reactions in Inbox mentioning the paper; Claude creates Source Note (via Zotero) + permanent notes during processing
- **Zotero-first paper lookup**: Always query local Zotero via Better BibTeX before falling back to PubMed/web
- **Entity notes**: Hub notes for proteins, compounds, techniques — created when 2+ mentions, no people-entities for lab members
- **Liberal inline wikilinks**: Link entities and notes throughout body text, not just in Links sections
- **Session summaries**: Auto-create at end of every Claude Code session
- **dTAG-13 vs dTAG-V1**: dTAG-13 recruits CRBN; dTAG-V1 recruits [[VHL]] — corrected an error

## Notes Created
- [[Knowledge Management System Vision]] — vision for the vault as a capture-then-process system
- [[Capture First, Organize Later]] — typing vs speaking, first-draft principle, distraction trap
- [[NIH PTDP Grant - NaV1.8 Covalent Degrader]] — grant planning with Rob Gereau
- [[Documentation as Lab Infrastructure]] — SOPs as safety nets, personnel expectations, leadership tension
- [[VHL in DRG Neurons and the dTAG System]] — key insight from HIF-1/SARM1 paper
- [[dTAG-13 Capsaicin Experiment Plan]] — in vivo experiment discussed with Rich
- [[VHL]] — entity note
- [[NaV1.8]] — entity note
- [[dTAG]] — entity note
- [[HIF-1 Protects Neurons from SARM1 Neurodegeneration - 2026]] — source note, paper metadata from Zotero
- [[Chamessian NIH PTDP Brainstorming with Rob Gereau - 2026-03-02]] — source note, meeting template applied

## Notes Updated
- [[Capture First, Organize Later]] — added voice capture speed data (~180 wpm), recurring distraction pattern, new "Maker Upside" section
- [[Knowledge Management System Vision]] — added paper reading workflow section
- [[dTAG]] — added dTAG-13 alias, CRBN distinction, in vivo experiment info

## Vault Changes
- Initialized git repo, pushed to `github.com/achamess/co-pilot-vault` (private)
- Created `CLAUDE.md` with persistent workflow instructions
- Created templates: Meeting Note, Entity Note, Zotero Source, Claude Session
- Removed Capture section from Daily Note template
- Installed Zotero Integration plugin (obsidian-zotero-desktop-connector)
- Fixed trailing-space filenames across all inbox notes
- Processed and archived 12 inbox notes total (1 journal entry archived without distillation)

## Open Questions
- Zotero Integration plugin needs GUI configuration in Obsidian (import format, output path, bibliography style)
- Should MOCs be created now that there are enough entity/permanent notes to organize?
- DeepLabCut setup details for the capsaicin experiment
- PTDP action items still open (Simone Haroutounian, Mohamed Hachicha, collaborator, innovation criteria)
