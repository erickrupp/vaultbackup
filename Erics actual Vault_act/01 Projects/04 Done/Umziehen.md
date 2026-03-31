---
type:
  - "[[project]]"
status: finalised
date: 2025-01-02 20:16
aliases:
goal:
  - "[[Umzug Gettorf]]"
area:
  - "[[Familie]]"
---


# Umziehen
## 2025-01-02 20:16

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
[[Haus GWS herrichten und verkaufen]]
[[Haus in Gettorf kaufen und einrichten]]

```button
name New Project
type command
action QuickAdd: New Project
color blue
```
^button-newProject
#### Mit dem Projekt verlinkte Projekte 
```dataview
list status 
FROM [[Umziehen]]
WHERE contains(type, "project")
```
### Mit dem Project verlinkte Ressourcen
```dataview
list status 
WHERE contains(project, [[Umziehen]])
WHERE contains(type, "research") OR contains(type, "concept") OR contains(type, "evergreen") OR contains(type, "methode")
```



**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]