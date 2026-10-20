<!-- Kurze Praxisnotiz: wie ich einen fast vollen 8-GB-Mac wieder frei bekommen habe. -->
# Freeing up a full Mac: what actually took the space

Video work fills a laptop quickly. My M1 MacBook (8 GB RAM, 228 GB disk) was down to **4.2 GB free**. After cleaning up it has about **65 GB free**.

## Method

1. **Measure before deleting.** List the biggest folders first instead of guessing.
2. **Move to the Trash, not into the void.** Everything went to the Trash first, so I could undo it. I emptied it myself after looking once more.
3. **Leave app-internal data alone.** A large folder inside a chat app looked tempting but belongs to the app. I did not touch it.

## Where the space was

| What | Size |
|---|---|
| Intermediate video cuts from an older editing tool | ~35 GB |
| Raw footage folders no longer needed | ~16 GB |
| Caches (package managers, tools) | ~11 GB |
| Apps in total | only 14 GB |

Takeaway: **apps are rarely the problem, working files are.** Render intermediates and old footage were most of it.

## Decisions I made on the way

- Keep important files in two places (for example GitHub plus a drive) before deleting a local copy.
- For an external drive, compare real speeds, not the number on the box. My laptop cannot use the fastest USB standard, so paying extra for "2000 MB/s" drives gives about 1000 MB/s anyway.
- Cheap flash sticks are fine for storing and carrying files, but too slow to edit video from.
- Buy from the manufacturer or a known shop. Fake drives are common on marketplaces.

## A habit that stuck

Render outputs are now excluded from Git, so a 200 MB render or a virtual environment can no longer clog a backup.

Back to the [overview](../README.md).
