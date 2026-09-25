---
type: location
region:
chapter:
kind:
visited: false
first_visited:
map:
tts_url:
tags: [location]
---
# {{title}}

**Book page:**
**First impression (read-aloud idea, in your own words):**

## Notable features
-

## People here
```dataview
LIST FROM "05 NPCs" WHERE contains(string(location), this.file.name)
```

## What happened here
```dataview
LIST FROM "02 Sessions" WHERE contains(file.outlinks, this.file.link)
```
