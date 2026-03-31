---
type:
  - "[[project]]"
status: ongoing
date: 2025-07-28 08:08
aliases:
goal:
area:
context:
---


# Themen
## 2025-07-28 08:08

---
# Themen 
- [[Angst frisst Verantwortung spaltet die Gesellschaft]]
- [[Gewohnheiten aus meiner Sicht]]
- [[Projekt - Konzept Entwicklung TNCERT]]
	- Konzept Nachwuchszentrum [[2026 Strategie Nachwuchszentrum BU-C]]
	- Resilienz gegen und mit KI
	- KI verändert alles, auch die Veränderung



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
FROM [[Themen]]
WHERE contains(type, "project")
```


### Mit dem Project verlinkte Ressourcen
```dataview
list status 
WHERE contains(project, [[Themen]])
WHERE contains(type, "research") OR contains(type, "concept") OR contains(type, "evergreen") OR contains(type, "methode") OR contains(type, "litnote")
```




**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]