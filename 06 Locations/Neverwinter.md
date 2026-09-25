---
type: location
region: The North
chapter: "[[Ch 03 - The Savage Frontier]]"
kind: "city"
visited: false
first_visited:
map: ""
tts_url:
tags: [location]
---
# Neverwinter

**Book:** [[Storm Kings Thunder.pdf#page=102|p. 101]]
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
