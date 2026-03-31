---
type:
  - area
status: new
date: <% tp.file.creation_date() %>
context:
---

<% await tp.file.move("/02 Areas/" + tp.file.title) %>
# <% tp.file.title %>
## <% tp.file.creation_date() %>

---
# Area info


## Welche Projekte sind hier verankert

```dataview
TABLE goal as "Ziel" 
WHERE contains(type, "project") AND contains(area, [[<% tp.file.title %>]])
```

```button
name New Project
type command
action QuickAdd: New Project
color blue
```
^button-newProject

## Welche Ziele sind hier verankert
```dataview
LIST status 
WHERE contains(type, "goal") AND contains(area, [[<% tp.file.title %>]])
```
```button
name New Goal
type command
action QuickAdd: New Goal
color green
```
^button-newgoal


## Weitere Ressourcen
```dataview
List 
WHERE !contains(type, "project") AND !contains(type, "goal") AND !contains(type, "foldernote") AND contains(area, [[<% tp.file.title %>]])
```

## ToDos


## Reference
**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]