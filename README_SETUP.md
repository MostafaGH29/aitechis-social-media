# AITECHIS Claude Code + Buffer Setup

## 1. Add final assets
Place approved media in:
`2026-11/assets/feed/<POST_ID>/` for Feed posts and `2026-11/assets/stories/<STORY_ID>/` for Stories

Example:
`2026-11/assets/N04/N04_01.png`
`2026-11/assets/N04/N04_02.png`

## 2. Open this package root in your terminal
Start Claude Code from this folder so it reads `CLAUDE.md`.

## 3. Connect Buffer
Run:

`claude mcp add --transport http buffer https://mcp.buffer.com/mcp`

Then start Claude Code and run:

`/mcp`

Select Buffer and complete OAuth.

## 4. Use the master prompt
Paste `MASTER_EXECUTION_PROMPT.txt` into Claude Code.

The first pass is read-only and should produce a preflight report.

## 5. Approval gates
After reviewing the preflight:

`APPROVE BUFFER DRAFT CREATION`

After reviewing Buffer drafts:

`APPROVE SCHEDULING`

Do not use immediate publishing during the first month.

## Recommended workflow
ChatGPT → strategy, calendar, captions
You / Designer → final media
Claude Code → validation, asset matching, Buffer execution
Buffer → review, scheduling, publishing


## Feed vs Stories

Feed:
- IDs: N01–N12
- Folder: `2026-11/assets/feed/`

Stories:
- IDs: NS01–NS21
- Folder: `2026-11/assets/stories/`

Examples:

Feed carousel:
`2026-11/assets/feed/N04/N04_01.png`

Story frames:
`2026-11/assets/stories/NS07/NS07_01.png`
`2026-11/assets/stories/NS07/NS07_02.png`

Claude must never mix Feed and Story assets.

Some native Story interactions may require manual completion depending on Buffer support. Claude must flag these instead of inventing or removing them.
