---
type:
  - "[[project]]"
status: finalised
date: 2025-01-02 21:37
aliases:
goal:
  - "[[Umzug Gettorf]]"
area:
  - "[[Familie]]"
---


# Einleben in Gettorf
## 2025-01-02 21:37

---
Wenn wir als Familie in Gettorf angekommen sind, geht es auch darum dort anzukommen. Im Einzelnen:
- Beim TÜV in Kiel und HH
- Bei Beate und Herby
- in der Gemeinde mit gemeinsamen Aktivitäten
- Bei der Suche nach alten Freunden in Kiel 
- Neue Aktivitäten
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
FROM [[Einleben in Gettorf]]
WHERE contains(type, "project")
```


### Mit dem Project verlinkte Ressourcen
```dataview
list status 
WHERE contains(project, [[Einleben in Gettorf]])
WHERE contains(type, "research") OR contains(type, "concept") OR contains(type, "evergreen") OR contains(type, "methode")
```



**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]