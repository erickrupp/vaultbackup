---
training:
tags:
type:
  - foldernote
aliases:
status: ongoing
goal:
area:
context:
---
## Table of content
```dataview
TABLE type as "Dokumententyp", project as "Projekt"
WHERE contains(file.folder, this.file.folder) 
AND !contains(type, "foldernote")
SORT file.ctime ASC
```

## Overhead Notes 



## Reference


## Table of content
```dataview
TABLE type as "Dokumententyp", project as "Projekt"
WHERE contains(file.folder, this.file.folder) 
AND !contains(type, "foldernote")
SORT file.ctime ASC
```

## Overhead Notes 



## Reference


