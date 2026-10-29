# AITECHIS Asset Naming Rules — November 2026

## Folder Structure

Feed:
`2026-11/assets/feed/<POST_ID>/`

Stories:
`2026-11/assets/stories/<STORY_ID>/`

## Feed IDs
N01 → N12

Examples:
- Single image: `N05_01.png`
- Carousel:
  - `N04_01.png`
  - `N04_02.png`
  - `N04_03.png`

Carousel numbering is the exact publication order.

## Story IDs
NS01 → NS21

Examples:
- One frame: `NS07_01.png`
- Three frames:
  - `NS07_01.png`
  - `NS07_02.png`
  - `NS07_03.png`

Story numbering is the exact frame order.

## Critical Rules
- Feed and Story assets must NEVER be mixed.
- Claude must identify asset type from both folder path and ID prefix.
- `N##` means Feed post.
- `NS##` means Story set.
- Never infer order from file modification date.
- Always sort by numeric suffix.
- If expected asset count does not match the calendar, BLOCK.
- If a Story requires an interactive element unsupported by Buffer, report it instead of silently changing the Story.
