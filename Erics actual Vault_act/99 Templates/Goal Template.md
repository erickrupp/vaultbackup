---
type:
  - "[[goal]]"
status: new
date: <% tp.file.creation_date() %>
aliases:
area:
context:
---

<% await tp.file.move("/00 MAPLE/02 Ziele/" + tp.file.title) %>
# <% tp.file.title %>
## <% tp.file.creation_date() %>

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
where contains(type, "project") AND contains(goal, [[<% tp.file.title %>]])
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


## Reference
**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]