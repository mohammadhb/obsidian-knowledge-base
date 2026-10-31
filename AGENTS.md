# LLM Wiki

Based on [Karpathy’s LLM Wiki](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f).

## Structure

- `raw/`: curated original sources. Read them; never modify them.
- `wiki/`: agent-maintained Markdown knowledge pages. Create summaries, entity pages, concept pages, comparisons, and syntheses as material calls for them. Connect pages with Obsidian wikilinks and cite their sources.
- `wiki/index.md`: catalog of pages, each with a link and one-line summary. Organize by category as the wiki grows.
- `wiki/log.md`: append-only chronological record of ingests, queries, and lint passes. Use headings like `## [YYYY-MM-DD] ingest | Source title`.
- `AGENTS.md`: the schema and operating instructions; evolve with the user as needed.

## Ingest

Read the new source. Summarize it in the wiki, integrate its information into relevant existing pages, and create new pages where useful. Maintain cross-references and explicitly note contradictions with prior sources. Update the index and append a log entry. Prefer processing one source at a time with user involvement.

## Query

Read the index first, then relevant pages and sources. Answer with citations. File useful new analyses and connections back into the wiki so the knowledge accumulates; update the index and log when doing so.

## Lint

Check for contradictions, stale claims, orphan pages, missing concept pages, missing cross-references, and gaps in the evidence. Repair the wiki where supported and suggest questions or sources for unresolved gaps. Append the results to the log.
