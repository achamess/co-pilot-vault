# Co-Pilot Vault — Claude Instructions

## Inbox Processing Workflow
1. Read all unprocessed notes in `00 Inbox/`
2. Fix trailing-space filenames (rename `"file .md"` → `"file.md"`)
3. Distill into permanent notes (`02 Notes/`) with footnoted quotes from source captures
4. Create source notes (`04 Sources/`) for papers, meetings, or other reference material
5. Update existing permanent notes when new captures relate to existing topics (don't duplicate)
6. Cross-link notes with `[[wikilinks]]`
7. Mark inbox notes as `processed: true` and move to `07 Archive/`
8. Commit and push to GitHub

## Paper Lookup
- **Always query Zotero first** via Better BibTeX JSON-RPC at `http://localhost:23119/better-bibtex/json-rpc`
- Use method `item.search` with search terms: `{"jsonrpc":"2.0","method":"item.search","params":["search terms"],"id":1}`
- Only fall back to PubMed/web search if the paper is not in Zotero
- Pull full metadata (authors, DOI, journal, volume, issue, citekey) from Zotero into source notes

## Vault Structure
- `00 Inbox/` — Raw captures (single capture point, voice or typed)
- `01 Daily/` — Daily notes (tasks + log only, no capture section)
- `02 Notes/` — Permanent notes (your thinking, distilled, footnoted)
- `03 MOCs/` — Maps of Content
- `04 Sources/` — Preserved reference material (papers, meetings, articles)
- `05 Projects/` — Project folders
- `06 Templates/` — Note templates
- `07 Archive/` — Processed inbox notes

## Note Types
- **Permanent notes** use `type: permanent` — your interpretation/synthesis
- **Source notes** use `type: source` with `source_type:` (paper, meeting, article, etc.) — preserved records of external material
- **Inbox notes** use `type: inbox` — raw unprocessed capture
