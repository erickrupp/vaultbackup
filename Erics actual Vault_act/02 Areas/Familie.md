---
type: area
status: ongoing
date: 2025-01-02 19:52
---


# Familie
## 2025-01-02 19:52

---
# Area info


## Welche Projekte sind hier verankert

```dataview
TABLE goal as "Ziel" 
WHERE contains(type, "project") AND contains(area, [[Familie]])
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
WHERE contains(type, "goal") AND contains(area, [[Familie]])
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
WHERE !contains(type, "project") AND !contains(type, "goal") AND contains(area, [[Familie]])
```

## ToDos

