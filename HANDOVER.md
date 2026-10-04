# Handover: Storm King's Thunder DM setup

**For any new Claude session working on this campaign.** Read this file first, then follow the `skt-live-session` skill during play.
Keep the **Current state** section up to date at the end of every session (the skill's `end` step does this).

## Starting a fresh session (for Jeroen)

1. In the Claude desktop app, start a new task **on the PC you're playing on** and connect the folder that holds the vaults:
    - **Main PC (desktop-bjorn, since 2026-10-04):** `C:\Users\31646\Documents\DnD`
    - Old laptop (gram-bjorn): `C:\Users\bjorn\Desktop\Dndpdfs`
2. Type: **`Read SKT-DM-Vault/HANDOVER.md, then start 2`** (use the session number you're running).
3. That's it. Claude reads this file, loads the notes it needs, and replies "ready". Then type updates as described in [[Live Session with Claude]].

If Claude can't see the folder, the folder isn't connected to that task. Add it with **Add folder** in the app.

## Current state

*Last updated: 2026-10-04 (after session 1).*

| | |
|---|---|
| Sessions played | Session 0 (session zero), Session 1 (2026-10-04) |
| Next session | Session 2 - still in [[Nightstone]], 03:00 in-game, party split. See *Where we stopped* below and [[Session 001 - Live Log]]. |
| Party level | 1 (level 2 milestone pending: one goblin is still asleep in the village) |
| Party | [[B'Leep]] (Max), [[Shay Rajul-Aegis]] (Oxymoronic), [[Sylvaris]] (Niels), [[Wolfram Erenwald]] (player name unknown - "Player One") |
| Live logs so far | [[Session 001 - Live Log]] |

**Where we stopped (end of session 1, 03:00 in-game)**
- Worgs killed. The goblins fled the village, except **one asleep in a house** (the players don't know; the DM picks the house).
- After a long rest the party found [[Kella Darkhope]] at the inn. [[B'Leep]] showed his Zhentarim tattoo; she asked to talk with him alone. The party half-trusts her.
- [[B'Leep]]: at the inn with Kella. [[Wolfram Erenwald]]: in the keep with one guard, at Lady Nandar's body. [[Shay Rajul-Aegis]] and [[Sylvaris]]: on the drawbridge gate tower with two guards.
- The party knows: giants came on clouds, dropped rocks, stole the stone; a giant shouted about "Ostoria" (an ancient giant empire that fell in a war with dragons). They know the villagers fled north to some caves, but not that goblins hold them prisoner.
- Loot: silver necklace (20 sp), 1 gp, small dagger. No Inspiration recorded.
- The **Seven Snakes have not arrived** (they are overdue: the party already had its long rest).

**Open to-dos before session 2**
- [x] Session 1 recap posted to the Player Wiki.
- [ ] Between sessions: play B'Leep's private talk with Kella (Max) and Wolfram's scene with Lady Nandar's body (Player One). Tell Claude the outcome so the notes can be updated.
- [ ] Decide: which house the last goblin sleeps in; whether the fourth guard (Kaelen Zam) is inside the keep; whether the guards raised the drawbridge.
- [ ] Session 2 opening: the Seven Snakes ride up (if the drawbridge is raised, they call for it to be lowered). Then the Ear Seekers orc siege (p. 28), very dangerous at level 1-2.
- [ ] 13 goblins fled, most likely back to Hark: the Dripping Caves will be on alert in session 3.
- [ ] Confirm which version of the giant's words was used ("Careful! Ostoria's stone. The Countess waits." or "... Bring it home.").

**Open to-dos carried over from session 1 prep**
- [ ] Settle the sheet checks. Suggested fixes are in each PC note under *Session 1* (B'Leep INT 18 → 17; Shay: official Clan Crafter feature; Sylvaris: a Good ideal; Wolfram: player name).
- [ ] Send the handouts: everyone gets `Welcome to Storm King's Thunder.pdf`, and each player only their own letter (all in `_Sources/Player Handouts/`, local only). The same welcome text is on the player wiki as *Welcome*, plus a *Leads* page.
- [ ] Session 2 prep: the Seven Snakes, then the orc siege ("Ear Seekers", p. 28), which is very dangerous at level 2. See [[Nightstone - Kella and the Seven Snakes]].
- [ ] Discord server channels (see the guide) and Avrae (optional).
- [ ] Tabletop Simulator: D&D table mod + Nightstone map (player version ready: `_Sources/Maps/Nightstone - player map.png`, local only). Optional: share `_Sources/Maps/The North - player map.jpg` with the players so they see where Nightstone is.
- [ ] Before session 2-3: magic item wish lists from the players, pre-rolled giant loot, start foreshadowing, and pick the chapter 2 town (recommended: Bryn Shander). See [[Guide to the Guide - Takeaways]].
- [ ] Optional: publish the player wiki as a website with Quartz.
- [x] Book text copy for fast lookups: `_Sources/Storm Kings Thunder - text.txt` (added on the new PC 2026-10-04; on the old laptop it may be missing).

**Decisions made**
- Rules: D&D 5e **2014, rules as written, no homebrew**. Full table rules: [[Table Rules (Session 0)]].
- Monsters: use **2014** stat blocks (Fantasy Statblocks' built-in SRD), not the 2024 Monster Manual Jeroen owns.
- Both GitHub repos are **public by Jeroen's choice** (DM vault included, so players could read spoilers and live logs). Switching to private is fine at any time: repo → Settings → Change visibility.
- Levelling: XP or milestones as written; level up only on a short or long rest.
- **How the party met:** all four answered Lady Nandar's notice in Waterdeep and travelled the High Road together. Session 1 opens with a 15-minute campfire scene: in-character introductions plus one question per player (questions in [[Session 001 - Nightstone]]).
- **Personal hooks are kept simple** (Jeroen is a new DM, the players are new): Wolfram - sent by Helm's priests; Sylvaris - peacemaker for the elf quarrel; Shay - the glyph stone rumour; B'Leep - the reward, plus he can recognise Kella's Zhentarim snake. The bigger backstory threads (B'Leep's storm and mentor, Shay's Ostorian shard, Wolfram's memory and Helm's Hold) are parked for later; see each PC note.
- **Players are new to D&D and to sandbox play.** Keep the player wiki's *Leads* page current, and end each session by asking what they want to do next.

## Environment facts (so you don't rediscover them)

| Thing | Fact |
|---|---|
| PCs | **Main: `desktop-bjorn`** (Windows, user folder `C:\Users\31646`), vaults in `C:\Users\31646\Documents\DnD\` (cloned from GitHub 2026-10-04). Old laptop: `gram-bjorn`, vaults in `C:\Users\bjorn\Desktop\Dndpdfs\`. Both sync through GitHub. |
| DM vault | `...\SKT-DM-Vault` → [github.com/BjornHettema/SKT-DM-Vault](https://github.com/BjornHettema/SKT-DM-Vault) (public) |
| Player wiki | `...\SKT-Player-Wiki` → [github.com/BjornHettema/SKT-Player-Wiki](https://github.com/BjornHettema/SKT-Player-Wiki) (public) |
| Sync | Obsidian **Git** plugin (its settings live in the repo): commit-and-sync every 10 min, pull on startup. Each PC needs Git for Windows installed and a one-time GitHub sign-in (Git Credential Manager pops up on the first push). |
| Plugins (DM vault) | Git, Dataview, Fantasy Statblocks, Initiative Tracker, Dice Roller, Homepage (opens `00 Home`), Calendarium. Player wiki: Git only. |
| Claude file access | `device_bash` **fails on both PCs** (laptop: a Windows update blocks it; desktop: "Workspace unavailable"). Use `device_list_dir`, `device_stage_files` (read) and `device_commit_files` (write) instead. Retry `device_bash` once per session; it may work after a Windows update. |
| Blocked | Writing inside any `.git` folder is not allowed via Claude's tools. Git operations that need the terminal must be done by Jeroen in **Git Bash**. |
| Browser | Claude's in-app browser has github.com allowed; Jeroen signs in himself (Claude never types passwords). |
| Timezone | Jeroen lives in **UTC+7** (Bangkok). Sessions are scheduled in **Amsterdam time** (the players' time): 12:00-17:00 Amsterdam = **17:00-22:00 for Jeroen**. Use the local time from his start message for live-log timestamps, and say "AMS" when you mean the players' clock. |
| Table setup | **PC:** Tabletop Simulator (with a Steam Workshop D&D table mod; its initiative and HP tracking are used for combat), Obsidian for reading, Claude desktop app running so the vault stays linked. **Laptop:** the same Claude chat, used for questions and updates. **Phone:** Discord voice. Sessions run about 12:00-17:00 Amsterdam time (17:00-22:00 Jeroen's time) with a break around 14:15 AMS. Full procedure: [[Session Day Runbook]]. |
| DM style | New DM, new to the campaign. He mostly asks "the party does X, what happens?". Treat questions as updates (log what they reveal), answer with what to say or roll plus the page, and give a status plus "likely next" on `break`. He does **not** want to report every event. |

## Vault conventions

- **Book page links:** `[[Storm Kings Thunder.pdf#page=N|p. M]]` where **PDF page N = book page M + 1**. Inside tables, escape the pipe: `\|`. The PDF is `_Sources/Storm Kings Thunder.pdf` (local only).
- **Other sources in `_Sources/`:** `Guide to the guide.pdf` (Sean McGovern's community *A Guide to Storm King's Thunder*: chapter-by-chapter running notes, Monster Manual page refs, a sample campaign outline); `Character Sheets/`; `Session 001 - DM Briefing.pdf` (21-page DM briefing for session 1: scenes, NPCs, foreshadowing seeds, map); `Maps/`: `Nightstone - player map.png`, the full high-res Sword Coast map (`HighRes (without Saltmarsh) (1) (1).jpg`), `The North - DM map.jpg` (campaign places 1-10) and `The North - player map.jpg` (player-safe). All listed in [[Maps Index]].
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
| 1 | 2026-10-04 | [[Ch 01 - A Great Upheaval]] | Arrived at Nightstone; killed the worgs, goblins fled. Found Kella (B'Leep showed his Zhentarim tattoo) and three keep guards; learned about the giants and "Ostoria". Ended 03:00 in-game, party split. | [[Session 001 - Live Log]] |
