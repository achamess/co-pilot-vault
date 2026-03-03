# Co-Pilot Vault — Claude Instructions

## Inbox Processing Workflow
1. Read all unprocessed notes in `00 Inbox/`
2. Fix trailing-space filenames (rename `"file .md"` → `"file.md"`)
3. Distill into permanent notes (`02 Notes/`) with footnoted quotes from source captures
4. Create source notes (`04 Sources/`) for papers, meetings, or other reference material
5. Update existing permanent notes when new captures relate to existing topics (don't duplicate)
6. Create or update entity notes when an entity appears in 2+ notes, or when explicitly requested
7. Cross-link notes with `[[wikilinks]]`
8. Mark inbox notes as `processed: true` and move to `07 Archive/`
9. Commit and push to GitHub

## Paper Lookup
- **Always query Zotero first** via Better BibTeX JSON-RPC at `http://localhost:23119/better-bibtex/json-rpc`
- Use method `item.search` with search terms: `{"jsonrpc":"2.0","method":"item.search","params":["search terms"],"id":1}`
- Only fall back to PubMed/web search if the paper is not in Zotero
- Pull full metadata (authors, DOI, journal, volume, issue, citekey) from Zotero into source notes

## Vault Structure
- `00 Inbox/` — Raw captures (single capture point, voice or typed)
- `01 Daily/` — Daily notes (tasks + log only, no capture section)
- `02 Notes/` — Permanent notes and entity notes (see Note Types)
- `03 MOCs/` — Maps of Content (high-level topic hubs linking to notes and entities)
- `04 Sources/` — Preserved reference material (papers, meetings, articles)
- `05 Projects/` — Project folders
- `06 Templates/` — Note templates
- `07 Archive/` — Processed inbox notes

## Note Types
- **Permanent notes** use `type: permanent` — your interpretation/synthesis/arguments
- **Entity notes** use `type: entity` with `entity_type:` (protein, compound, person, technique, etc.) — accumulated facts about a specific thing, linking out to permanent and source notes. Lives in `02 Notes/`.
- **Source notes** use `type: source` with `source_type:` (paper, meeting, article, etc.) — preserved records of external material
- **Inbox notes** use `type: inbox` — raw unprocessed capture
- **MOCs** use `type: moc` — high-level topic maps linking to entities, notes, and sources

## Entity Notes
- **What they are**: Hub notes for specific things (proteins, compounds, people, techniques) that compile what you know from across the vault
- **Division of labor**: Entity = what is known about X; Permanent note = what you think/argue about X
- **Creation threshold**: Create when an entity appears in 2+ other notes, or when explicitly requested
- **People**: Use for collaborators and field figures, not for direct reports/lab members
- **Template**: Entity Note template in `06 Templates/`
