---
type:
  - "[[project]]"
status: finalised
date: 2025-01-02 21:44
aliases:
goal:
  - "[[Meine Situation TÜV und Trainings]]"
area:
  - "[[02 Areas/TÜV|TÜV]]"
---


# Meine Rolle im TÜV in der HR neu finden
## 2025-01-02 21:44

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

[[Projekt - Trainings an Benjamin verkaufen]]
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
FROM [[Meine Rolle im TÜV in der HR neu finden]]
WHERE contains(type, "project")
```


### Mit dem Project verlinkte Ressourcen
```dataview
list status 
WHERE contains(project, [[Meine Rolle im TÜV in der HR neu finden]])
WHERE contains(type, "research") OR contains(type, "concept") OR contains(type, "evergreen") OR contains(type, "methode")
```



**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]