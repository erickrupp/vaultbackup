---
type:
  - "[[project]]"
status: hold
date: 2025-12-02 13:10
aliases:
goal:
area:
context:
---


# TÜV Seminarkatalog
## 2025-12-02 13:10

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
FROM [[TÜV Seminarkatalog]]
WHERE contains(type, "project")
```


### Mit dem Project verlinkte Ressourcen
```dataview
list status 
WHERE contains(project, [[TÜV Seminarkatalog]])
WHERE contains(type, "research") OR contains(type, "concept") OR contains(type, "evergreen") OR contains(type, "methode") OR contains(type, "litnote")
```



**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]