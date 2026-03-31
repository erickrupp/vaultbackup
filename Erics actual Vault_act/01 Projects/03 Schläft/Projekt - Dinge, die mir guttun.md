---
training:
tags:
type:
  - foldernote
aliases:
status: hold
goal:
  - "[[Eigene Projekte]]"
area:
  - "[[Persönlich]]"
---
## Table of content
```dataview
TABLE type as "Dokumententyp", project as "Projekt"
WHERE contains(file.folder, this.file.folder) 
AND !contains(type, "foldernote")
SORT file.ctime ASC
```

## Overhead Notes 

![[Preview.jpg]]

## Reference


## Table of content
```dataview
TABLE
WHERE contains(file.folder, this.file.folder) 
AND !contains(type, "foldernote")
```

## Overhead Notes 



## Reference


