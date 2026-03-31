---
type:
  - "[[project]]"
status: hold
date: 2025-01-02 21:06
aliases:
goal:
  - "[[Meine Situation TÜV und Trainings]]"
area:
  - "[[02 Areas/TÜV|TÜV]]"
project:
---


# Trainings an Benjamin verkaufen
## 2025-01-02 21:06

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
[[Projekt - Meine Rolle im TÜV in der HR neu finden]]

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
FROM [[Trainings an Benjamin verkaufen]]
WHERE contains(type, "project")
```


### Mit dem Project verlinkte Ressourcen
```dataview
list status 
WHERE contains(project, [[Trainings an Benjamin verkaufen]])
WHERE contains(type, "research") OR contains(type, "concept") OR contains(type, "evergreen") OR contains(type, "methode")
```



**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]