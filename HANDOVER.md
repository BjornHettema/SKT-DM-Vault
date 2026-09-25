# Handover: Storm King's Thunder DM setup

**For any new Claude session working on this campaign.** Read this file first, then follow the `skt-live-session` skill during play.
Keep the **Current state** section up to date at the end of every session (the skill's `end` step does this).

## Starting a fresh session (for Jeroen)

1. In the Claude desktop app, start a new task **on this PC (gram-bjorn)** and connect the folder `C:\Users\bjorn\Desktop\Dndpdfs`.
2. Type: **`Read SKT-DM-Vault/HANDOVER.md, then start 1`** (use the session number you're running).
3. That's it. Claude reads this file, loads the notes it needs, and replies "ready". Then type updates as described in [[Live Session with Claude]].

If Claude can't see the folder, the folder isn't connected to that task. Add it with **Add folder** in the app.

## Current state

*Last updated: 2026-09-25 (setup day, before session 1).*

| | |
|---|---|
| Sessions played | Session 0 (session zero) |
| Next session | Session 1 - [[Ch 01 - A Great Upheaval]], arriving at [[Nightstone]] |
| Party level | 1 |
| Party | [[B'Leep]] (Max), [[Shay Rajul-Aegis]] (Oxymoronic), [[Sylvaris]] (Niels), [[Wolfram Erenwald]] (player name unknown - "Player One") |
| Live logs so far | none |

**Open to-dos before or around session 1**
- [ ] Settle the sheet checks in each PC note (B'Leep INT 18; Shay reflavour + custom background; Sylvaris ideal vs alignment; Wolfram's player name).
- [ ] Talk to each player about character context and backgrounds (promised at session 0).
- [ ] Discord server channels (see the guide) and Avrae (optional).
- [ ] Tabletop Simulator: D&D table mod + Nightstone map.
- [ ] Optional: publish the player wiki as a website with Quartz.
- [ ] Book text copy for fast lookups: `_Sources/Storm Kings Thunder - text.txt` - check whether it exists (see *Book text* below).

**Decisions made**
- Rules: D&D 5e **2014, rules as written, no homebrew**. Full table rules: [[Table Rules (Session 0)]].
- Monsters: use **2014** stat blocks (Fantasy Statblocks' built-in SRD), not the 2024 Monster Manual Jeroen owns.
- Both GitHub repos are **public by Jeroen's choice** (DM vault included, so players could read spoilers and live logs). Switching to private is fine at any time: repo → Settings → Change visibility.
- Levelling: XP or milestones as written; level up only on a short or long rest.

## Environment facts (so you don't rediscover them)

| Thing | Fact |
|---|---|
| PC | Windows, device name `gram-bjorn`, user folder `C:\Users\bjorn` |
| DM vault | `C:\Users\bjorn\Desktop\Dndpdfs\SKT-DM-Vault` → [github.com/BjornHettema/SKT-DM-Vault](https://github.com/BjornHettema/SKT-DM-Vault) (public) |
| Player wiki | `C:\Users\bjorn\Desktop\Dndpdfs\SKT-Player-Wiki` → [github.com/BjornHettema/SKT-Player-Wiki](https://github.com/BjornHettema/SKT-Player-Wiki) (public) |
| Sync | Obsidian **Git** plugin, pre-configured: commit-and-sync every 10 min, pull on startup. Git for Windows is installed; GitHub sign-in via Git Credential Manager is done. |
| Plugins (DM vault) | Git, Dataview, Fantasy Statblocks, Initiative Tracker, Dice Roller, Homepage (opens `00 Home`), Calendarium. Player wiki: Git only. |
| Claude file access | `device_bash` **fails** on this PC ("A Windows update released September 8 prevents Claude's workspace from reaching your files"). Use `device_list_dir`, `device_stage_files` (read) and `device_commit_files` (write) instead. Retry `device_bash` once per session; it may work after a Windows update. |
| Blocked | Writing inside any `.git` folder is not allowed via Claude's tools. Git operations that need the terminal must be done by Jeroen in **Git Bash**. |
| Browser | Claude's in-app browser has github.com allowed; Jeroen signs in himself (Claude never types passwords). |
| Timezone | Asia/Bangkok (UTC+7) |

## Vault conventions

- **Book page links:** `[[Storm Kings Thunder.pdf#page=N|p. M]]` where **PDF page N = book page M + 1**. Inside tables, escape the pipe: `\|`. The PDF is `_Sources/Storm Kings Thunder.pdf` (local only).
- **`_Sources/` is gitignored** (PDFs, character sheets, book text). Never put book text anywhere else, and never commit PDFs.
- **Folders:** `00 Inbox`, `01 Campaign`, `02 Sessions`, `03 Party`, `04 Chapters`, `05 NPCs`, `06 Locations`, `07 Factions`, `08 Encounters`, `09 Handouts`, `_Templates`, `_Attachments`, `_Sources`.
- **Frontmatter used by the dashboards:** sessions `type: session`, `session_number`; live logs `type: livelog`; NPCs `type: npc`, `met`, `location`, `faction`, `status`, `attitude`; PCs `type: pc`, `absences`, `inspiration`; chapters `type: chapter`, `status`.
- **Session notes:** Jeroen's prep note `02 Sessions/Session NNN - <name>.md` (Session template) is his. Claude writes the separate `02 Sessions/Session NNN - Live Log.md` (Live Log template) during play.
- **PC notes** contain DM-only secrets and hooks. They never go to the Player Wiki. Player Wiki PC pages hold appearance only; the players write the rest.
- **Player Wiki:** only what players may know. `draft: true` hides a note from a future Quartz site. Claude writes there only with Jeroen's explicit OK.
- **Safe writes:** stage the file, keep a working copy, commit with `expectedMtimeMs`. If a commit is rejected, re-stage and merge (Jeroen's text wins). Never `force`.

## Book text (for fast lookups)

The PDF is a scan (no text layer). A searchable text copy speeds up lookups a lot. If `_Sources/Storm Kings Thunder - text.txt` is missing, make it in the cloud workspace (about 1 hour, runs in the background):

```bash
# after staging _Sources/Storm Kings Thunder.pdf into the cloud workspace
for p in $(seq 1 258); do
  pdftoppm -r 110 -gray -f $p -l $p -png "Storm Kings Thunder.pdf" img
  echo "=== PDF page $p (book p. $((p-1))) ===" >> text.txt
  tesseract img-*.png - --psm 1 2>/dev/null >> text.txt; rm -f img-*.png
done
```

Then save it as `_Sources/Storm Kings Thunder - text.txt` with `device_commit_files`. It is gitignored, so it stays on Jeroen's PC. Use it only for lookups, and answer in summaries with page numbers, never long quotes.

## Session history

| Session | Date | Chapter | Summary | Live log |
|---|---|---|---|---|
| 0 | 2026-09-25 (approx.) | - | Session zero: table rules agreed, four PCs created | - |
