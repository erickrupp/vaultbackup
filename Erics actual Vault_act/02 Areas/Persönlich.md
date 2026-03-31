---
type: area
status: ongoing
date: 2025-01-02 20:44
---


# Persönlich
## 2025-01-02 20:44

---
# Area info


## Welche Projekte sind hier verankert

```dataview
LIST status 
WHERE contains(type, "project") AND contains(area, [[Persönlich]])
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
WHERE contains(type, "goal") AND contains(area, [[Persönlich]])
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
WHERE !contains(type, "project") AND !contains(type, "goal") AND !contains(type, "foldernote") AND contains(area, [[Persönlich]])
```

## ToDos

