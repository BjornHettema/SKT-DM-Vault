---
type: guide
---
# Live Session with Claude

During play, keep the Claude chat open on your second screen and type short updates. Claude keeps the vault up to date, answers lookups and gives improv help, so you can keep your eyes on the table.

**Claude writes to:** `02 Sessions/Session NNN - Live Log.md` (one per session, Claude's own note), plus NPC notes and [[Open Threads]].
**Claude never touches:** your prep note for the session, unless you say `end` (see below).

> [!tip] Start of the session
> Type `start 1` (or whichever session number it is). Claude creates the live log and loads the chapter, NPCs and PCs for that session.

## Shorthand

Type naturally - the prefixes just make it faster. Several updates in one message is fine.

| You type | Claude does |
|---|---|
| `start 1` | Creates the live log for session 1, notes the attendees |
| *anything plain* | Logs it with a timestamp, e.g. `party reaches Nightstone, bell ringing` |
| `npc Morak - met him at the inn, grumpy, wants the villagers back` | Logs it, sets `met: true` on the NPC and adds to *What the party knows* |
| `new npc Hark - goblin boss, Dripping Caves` | Creates the NPC note (NPC template) and links it |
| `loot Wolfram - +1 shield` | Logs loot on the session and the PC note |
| `xp 450` / `milestone` | Logs the award |
| `insp Sylvaris - talked the goblins down` | Logs Inspiration in the tracker |
| `align B'Leep - left the goblin prisoners to die` | Logs it in the Alignment watch |
| `rule grappling a flying creature - allowed, disadv` | Logs a ruling to check against the rules later |
| `thread who sent the goblins?` | Adds it to [[Open Threads]] |
| `? how does the tower of Zephyros land` | **Lookup** - answers from the book, citing the page |
| `? rules: two-weapon fighting with a dagger` | **Rules lookup** (2014 rules as written) |
| `! innkeeper voice` / `! what does Kella do now` | **Improv** - 2-3 quick options that fit the notes |
| `pause` / `resume` | Marks a break in the log |
| `end` | Wraps up: tidies the log, drafts the **spoiler-free player recap**, updates the session prep note's *After the session* section, lists anything to copy to the Player Wiki |

## How fast is it?
- Lookups and improv: an answer in chat, usually within seconds.
- Vault writes happen in the background. A note can take up to a minute to appear in Obsidian, and the Git plugin uploads it within 10 minutes.
- If you edit the live log yourself, Claude notices and keeps your changes.

## Ground rules
- Lookups are **summaries with page numbers**, not quotes from the book. Click the page link to read it yourself.
- Rules answers follow **2014, rules as written** (see [[Table Rules (Session 0)]]). Claude flags anything it isn't sure about instead of guessing.
- Nothing from the DM vault goes into the Player Wiki without your OK.
