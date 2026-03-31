---
type:
  - "[[project]]"
status: finalised
date: 2025-01-02 19:12
aliases:
goal:
  - "[[Eigene Projekte]]"
area:
  - "[[Persönlich]]"
---
---



# Klarheit über Projekte, die in den nächsten Monaten gemacht werden, gewinnen
## 2025-01-02 19:12

Ich muss mir zunächst einmal klar darüber werden, was ich mit meiner Zeit anfangen will und wie ich die verschiedenen Themen, die mir andauernd neu und nicht immer hierzu einfallen, unter einen Hut bekomme.

Hierzu erstelle ich ein Dokument über [[Potenzielle Projekte - Brain Dump, Bewertung und what next]].

---
# Project Informationen 

## Related to
### Goal 
[[Projekt - Dinge, die mir guttun]]

```button
name New Goal
type command
action QuickAdd: New Goal
color green
```
^button-newgoal

### Area 
[[Persönlich]]

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


# Mit dem Project verlinkte Ressourcen
```dataview
list status 
WHERE contains(project, [[Klarheit über Projekte, die in den nächsten Monaten gemacht werden, gewinnen]])
WHERE contains(type, "research") OR contains(type, "concept") OR contains(type, "evergreen") OR contains(type, "methode")
```

# Mit dem Project verlinkte Projekte 
```dataview
list status 
FROM [[Liste von potenziellen Projekten]]
WHERE contains(type, "project")
```



**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]