---
type:
  - "[[project]]"
status: new
date: <% tp.file.creation_date() %>
aliases:
goal:
area:
context:
---

<% await tp.file.move("/01 Projects/01 Arbeitsvorrat/" + tp.file.title) %>
# <% tp.file.title %>
## <% tp.file.creation_date() %>

---
# Project Informationen 

## Related to
### Goal 
```button
name New Goal
type command
action QuickAdd: New Goal
color green
```
^button-newgoal
### Area 
```button
name New Area
type command
action QuickAdd: New Area
color yellow
```
^button-newarea

### Project


```button
name New Project
type command
action QuickAdd: New Project
color blue
```
^button-newProject
#### Mit dem Project verlinkte Projekte 
```dataview
list status 
FROM [[<% tp.file.title %>]]
WHERE contains(type, "project")
```


### Mit dem Project verlinkte Ressourcen
```dataview
list status 
WHERE contains(project, [[<% tp.file.title %>]])
WHERE contains(type, "research") OR contains(type, "concept") OR contains(type, "evergreen") OR contains(type, "methode") OR contains(type, "litnote")
```


## Reference
**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]