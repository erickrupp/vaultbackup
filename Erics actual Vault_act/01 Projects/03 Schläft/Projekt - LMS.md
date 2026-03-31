---
training:
tags:
type:
  - "[[project]]"
aliases:
status: hold
goal:
area:
context:
---
## Table of content
```dataview
TABLE type as "Dokumententyp", project as "Projekt", status as "Status", file.folder as "Ordner"
WHERE contains(project, [[LMS]]) 
AND !contains(type, "foldernote")
SORT file.ctime ASC
```

## Overhead Notes 



## Reference



**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]