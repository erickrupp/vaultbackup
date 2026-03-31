---
training:
tags:
type:
  - foldernote
aliases:
status: new
goal:
area:
context:
---
## Table of content
```dataview
TABLE type as "Dokumententyp", project as "Projekt", status as "Status"
WHERE contains(file.folder, this.file.folder) 
AND !contains(type, "foldernote")
SORT file.ctime ASC
```

## Overhead Notes 



## Reference


**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]