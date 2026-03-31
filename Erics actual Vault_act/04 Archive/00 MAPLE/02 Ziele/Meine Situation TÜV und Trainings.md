---
type:
  - "[[goal]]"
status: finalised
date: 2025-01-02 21:05
aliases:
area:
  - "[[02 Areas/TÜV|TÜV]]"
---


#  Trainings
## 2025-01-02 21:05

---
# Goal info
## Related to
### Area 


```button
name New Area
type command
action QuickAdd: New Area
color yellow
```
^button-newarea

### Goal 


```button
name New Goal
type command
action QuickAdd: New Goal
color green
```
^button-newgoal


# Projekte 

```dataview
LIST status 
where contains(type, "project") AND contains(goal, [[ Trainings]])
```


```button
name New Project
type command
action QuickAdd: New Project
color blue
```
^button-newproject

# Action Items
> [!INFO] Beachte:
> hier nur, sofern sie nicht in Projekten abgebildet werden. Dies dient dazu Action Items schnell zu verfassen ohne Projektbezug und stellt die Ausnahme dar.


