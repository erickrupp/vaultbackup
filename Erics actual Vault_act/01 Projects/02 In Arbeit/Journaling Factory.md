---
type:
  - "[[project]]"
status: new
date: 2026-03-19 07:58
aliases:
goal:
area:
  - "[[OrientierungSinn]]"
context:
---


# Journaling Factory
## 2026-03-19 07:58

---
# Project Informationen 
## Warum mache ich das hier eigentlich?



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
FROM [[Journaling Factory]]
WHERE contains(type, "project")
```


### Mit dem Project verlinkte Ressourcen
```dataview
list status 
WHERE contains(project, [[Journaling Factory]])
WHERE contains(type, "research") OR contains(type, "concept") OR contains(type, "evergreen") OR contains(type, "methode") OR contains(type, "litnote")
```

![[Backlinks.base#Journalfactory]]


## Reference
**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]