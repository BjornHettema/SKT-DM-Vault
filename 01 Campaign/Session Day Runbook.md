---
type: guide
---
# Session Day Runbook

Everything **around** the table, step by step. Tabletop Simulator handles the map, minis, initiative and monster HP. This note covers Obsidian, Claude and Discord.

## Your setup

| Device | What's on it | What you use it for |
|---|---|---|
| **PC** | Tabletop Simulator (front), Obsidian (behind it, `Alt+Tab`), **Claude desktop app running** (minimised) | Running the game. Obsidian is only for **reading** the session note. |
| **Laptop** | **Claude**: the same chat, opened in the Claude app or at claude.ai | Your DM assistant: questions, lookups and updates. |
| **Phone** | Discord voice (with headphones) | Talking to the players. |

> [!important] Two rules that keep this working
> 1. **Start the Claude chat on the PC** (that links it to your vault), then open the **same chat** on the laptop. On the laptop, **don't** click "Link to this computer".
> 2. **Don't edit notes in Obsidian on the laptop.** One vault, on the PC. Claude writes to it; you read it.

## How you talk to Claude during play (the key idea)

You do **not** have to report every event. Two kinds of message are enough:

**1. Questions, whenever you need them.** Ask in a way that also says where the party is, and Claude logs it from your question. No separate update needed.
- "They're at the inn and Wolfram goes upstairs. What does he find?"
- "Sylvaris asks the guards what happened. What do they say?"
- "B'Leep noticed Kella's snake. How does she react?"
- "They want to jump the broken bridge. What do they roll?"
- "They killed the goblins in the windmill. What's next nearby?"
- "Player wants to steal Lady Nandar's ring. What happens?"

Asking a lot is fine; that's what Claude is for. Answers come back in a few lines, telling you **what to say or what to roll**, with the book page.

**2. A short checkpoint at natural pauses:** after a fight, when the party moves somewhere new, at the break. One or two lines, for example:
- "Checkpoint: worgs dead, Shay down to 3 HP, Sylvaris healed him. Party heading to the temple."
- "Checkpoint: found Kella, they believe her story. Wolfram is leading the guards now."
- "Loot: Pojo's gold ring to B'Leep. Inspiration to Sylvaris for calming the guards."

**Busy at the table?** Type nothing. Catch up at the break with one message covering what happened.

## The timeline (12:00-17:00)

> [!note] Times are Amsterdam time (the players' clock)
> For you that's **5 hours later**: 11:00 → 16:00, 12:00 → **17:00**, 14:15 → 19:15, 17:00 → **22:00**. Give Claude your own local time in the start message.

### 11:00 - Preparation (60 min)
- [ ] Read [[Session 001 - Nightstone]] sections 0-4 once (about 20 min), or pages 1-2 of `_Sources/Session 001 - DM Briefing.pdf`. You don't need the whole book.
- [ ] Open the book PDF at page 19 and glance at the map on page 21 (5 min).
- [ ] TTS: load your table and the map, place the minis, check that the players can join.
- [ ] Have the players received the welcome guide and their letters? Has everyone made their sheet fix?

### 11:40 - Start Claude (5 min)
1. **On the PC**, open the Claude desktop app and start a **new task** with the folder `Documents\DnD` connected.
2. Paste the **start message** below and send it.
3. Wait for Claude's "ready" reply.
4. **On the laptop**, open the same chat (Claude app or claude.ai, it appears in your recent tasks). Keep the PC's Claude app running.

**Start message (copy this):**
```
Session 1 of Storm King's Thunder starts at 12:00. My local time now is [HH:MM]. Players present: [all four / names].
Read SKT-DM-Vault/HANDOVER.md and Session 001 - Nightstone, use the skt-live-session skill, and start the live log.
I'm a new DM and new to this campaign: I'll mostly ask questions in the form "the party does X, what happens?". Log what you learn from my questions, keep answers short (what to say or roll + page), and give me a quick status and "what's likely next" whenever I write "break".
```

### 11:50 - Players join
- [ ] Discord voice on the phone, everyone in TTS.
- [ ] Quick tech check: can everyone see the map and roll dice?

### 12:00 - Opening (about 30 min)
Follow section 1 of [[Session 001 - Nightstone]]: rules check, then the **campfire**: introductions and the four questions. Read the strong start, then ask **"What do you do?"**
*Claude:* nothing needed. Optionally afterwards: "Campfire done, everyone introduced."

### 12:30 - Nightstone, part 1 (about 1 h 45)
Exploring, goblins, maybe the worgs.
*Claude:* questions whenever you need them, plus checkpoints after fights.

### 14:15 - Break (15 min)
- Type **`break`**. Claude replies with where the party is, what's still left in the village, and what's likely next.
- Add anything you didn't mention (loot, Inspiration, who's hurt).
- Glance at the session note for the next part.

### 14:30 - Nightstone, part 2 (about 2 h)
The keep and the guards, Kella, the remaining goblins.
**Aim to stop at the cliffhanger:** goblins cleared, the party rests, hoofbeats: seven riders. Note: the milestone (level 2) happens when the goblins are cleared, and they level up at the rest.

### 16:40 - Wrap-up with the players (20 min)
1. End on the cliffhanger.
2. Ask the table: **"What did you enjoy? What do you want more of?"**
3. Ask: **"What do you want to do next session?"** (the sandbox habit)
4. Remind them: the recap will be on the player wiki.

### After 17:00 - With Claude (15 min, can be later the same day)
1. Type **`end`**. Claude tidies the log, fills in the *After the session* part of the session note, updates the NPCs and the handover, and writes a **spoiler-free recap**.
2. Read the recap. If it's OK, say **"post it"** and Claude adds it to the Player Wiki.
3. Let Obsidian sync (or `Ctrl+P` → *Git: Commit-and-sync*).

## When you're stuck at the table
- Saying **"Give me a second, let me check my notes"** is completely normal. Players don't mind 30 seconds.
- Ask Claude: "They do X. What happens?" If it's not in the book, Claude gives you 2-3 options and **you pick**.
- No answer in sight? **Make something up that feels fair, say it confidently, and write it down.** Consistency later matters more than being right now.
- Rules argument? **You decide on the spot** (your table rules allow it). Note it, check it after the session.
- Someone not having fun or the energy dropping? Call a **5-minute break**.

## Don'ts
- Don't try to log everything. Questions and a few checkpoints are plenty.
- Don't read long passages from the book aloud. Summarise in your own words.
- Don't edit the vault on the laptop.
- Don't worry if you only get halfway through Nightstone. Chapter 1 is meant to take a few sessions.
