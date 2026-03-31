---
type: review/annually
---

<% await tp.file.move("/00 MAPLE/03 Review/Perioden/04 annually/" + tp.file.title) %>

# <% tp.file.title %>
## <% tp.file.creation_date() %>
<< [[<% tp.date.now("YYYY", "P-1Y") %>]] | [[<% tp.date.now("YYYY", "P1Y") %>]]>>

---

# Planning 

## Nordstern Overview
![[Nordstern]]

- Check Purpose

## Areas Overview
```dataview
table status
FROM "02 Areas"
WHERE contains(type, "area")
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
Table status
FROM "00 MAPLE"
WHERE contains(type, "goal")
```

- add new goal if necessary

```button
name New Goal
type command
action QuickAdd: New Goal
color green
```
^button-newgoal



# Review
## Breakthroughs in the year
```dataview
TABLE breakthrough
FROM [[<% tp.file.title%>]]
where contains(type, "review/monthly")
```

## Discoveries in the year
```dataview
TABLE discoveries
FROM [[<% tp.file.title%>]]
where contains(type, "review/monthly")
```

## Achievements
```dataview
TABLE achievements
FROM [[<% tp.file.title%>]]
where contains(type, "review/monthly")
```

## Learnings
```dataview
TABLE learnings
FROM [[<% tp.file.title%>]]
where contains(type, "review/monthly")
```



