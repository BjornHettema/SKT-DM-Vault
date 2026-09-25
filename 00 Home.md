# Storm King's Thunder

> [!tip] Before you start the session
> - Start the live log: in the Claude chat, type `start <session number>`.
> - Open the current session note (the newest one under *Latest sessions* below).
> - **Inspiration:** the players asked you to remember to hand it out. Check the tracker in the session note.
> - Check absences: only 1 absence is allowed, and it needs your approval. See [[Party Overview]].

## Quick links
[[Live Session with Claude]] · [[HANDOVER|Handover for Claude]] · [[Campaign Overview]] · [[Table Rules (Session 0)]] · [[Adventure Flow]] · [[Party Overview]] · [[Gazetteer of the North]] · [[Maps Index]] · [[Bestiary Index]] · [[Campaign Calendar]] · [[Open Threads]]

## Latest sessions
```dataview
TABLE WITHOUT ID file.link AS Session, date AS "Real date", chapter AS Chapter, level AS Level, ingame_date AS "In-game"
FROM "02 Sessions"
WHERE type = "session"
SORT session_number DESC
LIMIT 5
```

## Where we are in the book
```dataview
TABLE WITHOUT ID file.link AS Chapter, status AS Status, levels AS Levels
FROM "04 Chapters"
SORT file.name ASC
```

## NPCs the party has met
```dataview
TABLE WITHOUT ID file.link AS NPC, location AS Location, faction AS Faction, attitude AS Attitude, status AS Status
FROM "05 NPCs"
WHERE met = true
SORT file.mtime DESC
```

## Open to-dos from session notes
```dataview
TASK
FROM "02 Sessions" OR "04 Chapters"
WHERE !completed
GROUP BY file.link
```
