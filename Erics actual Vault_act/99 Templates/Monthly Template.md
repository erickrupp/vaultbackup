---
type: review/monthly
breakthrough: []
discoveries: []
achievements: []
learnings: []
review:
---

<% await tp.file.move("/00 MAPLE/03 Review/Perioden/03 Monthly/" + tp.file.title) %>

# <% tp.file.title %>
## <% tp.file.creation_date() %>


<< [[<% tp.date.now("YYYY-MM", "P-1M", tp.file.title, "YYYY-MM") %>]] | [[<% tp.date.now("YYYY", 0, tp.file.title, "YYYY-[MM") %>]] | [[<% tp.date.now("YYYY-MM", "P1M", tp.file.title, "YYYY-MM") %>]]>>

---

# Planning 
## What would make this month awesome 

## Setting Weeks
In Calendar View
CHECK:

```dataview
LIST 
FROM [[<% tp.file.title %>]]
WHERE contains(type, "review/weekly")
```


## Nordstern Overview
![[Nordstern]]


## Areas Overview
```dataview
LIST status
FROM "02 Areas"
WHERE contains(type, "area") AND !contains(status, "finalised")
```

```button
name New Area
type command
action QuickAdd: New Area
color yellow
```
^button-newarea


## Goal Overview
```dataview
List status
FROM "00 MAPLE"
WHERE contains(type, "goal") AND !contains(status, "finalised")
```
- Status update
- Check for new projects in goal note
- add new goal if necessary


```button
name New Goal
type command
action QuickAdd: New Goal
color green
```
^button-newgoal

## Project Overview
### Overview
```dataview
Table status as "Status", goal as "Ziel"
FROM "01 Projects"
WHERE contains(type, "project") AND !contains(status, "finalised")
sort goal asc 
sort status asc
```

- Add new projects if nessecary
- Set new goals in the Project Notes
- Set new set of tasks in the project notes

```button
name New Project
type command
action QuickAdd: New Project
color blue
```
^button-newproject

## Overview where this month is referenced
```dataview
list from [[<% tp.file.title %>]]
where !contains(type, "review")
```

## Tasks to be scheduled
### Inbox => Schedule these
```tasks
description includes #inbox 
```

### New Tasks 
>[!INFO] If scheduled, set due date, If not, set hashtag inbox 




# Review
## Focus
![[#What would make this month awesome]]
Did you met the monthly focus?
- Did you learn something 
- Change / Calibrate something
- Think of the Assessment im YAML


## Weekly Assessments:
## Breakthroughs 
```dataview
TABLE breakthrough
FROM [[<% tp.file.title%>]]
where contains(type, "review/weekly")
```

## Discoveries
```dataview
TABLE discoveries
FROM [[<% tp.file.title%>]]
where contains(type, "review/weekly")
```

## Achievements
```dataview
TABLE achievements
FROM [[<% tp.file.title%>]]
where contains(type, "review/weekly")
```

## Learnings
```dataview
TABLE learnings
FROM [[<% tp.file.title%>]]
where contains(type, "review/weekly")
```

## Reviews 
```dataview
TABLE review
FROM [[<% tp.file.title%>]]
where contains(type, "review/weekly")
```
## Assessment
In YAML-Frontmatter
Details here


> [!INFO] 
> if there is something to learn, is there a doing?

## Weeks of the last Month:
```dataview
List
from [[<% tp.date.now("YYYY-MM", "P-1M") %>]] AND !"00 MAPLE/03 Review/Perioden/03 Monthly" AND !"99 Templates"
```

## Projects worked on last month
```dataview
List status
FROM !"99 Templates"
where contains(type, "project") AND file.mtime >= date(today) - dur(31 day)
sort file.mtime asc
```
- Status Update
- What is to do to bring Projects forward

## Set-up new Month and plan there 


```button
name New Month
type command
action QuickAdd: New Month
color purple
```
^button-newmonth



<< [[<% tp.date.now("YYYY-MM", "P-1M", tp.file.title, "YYYY-MM") %>]] | [[<% tp.date.now("YYYY", 0, tp.file.title, "YYYY-[MM") %>]] | [[<% tp.date.now("YYYY-MM", "P1M", tp.file.title, "YYYY-MM") %>]]>>
