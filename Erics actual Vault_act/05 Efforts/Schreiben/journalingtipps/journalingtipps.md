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
TABLE type as "Dokumententyp", project as "Projekt", status as "Status"
WHERE contains(file.folder, this.file.folder) 
AND !contains(type, "foldernote")
SORT file.ctime ASC
```

## Overhead Notes 
In diesem Projekt habe ich in einem Sprint Journalingmethoden entwickelt, die oben im TOC verlinkt sind



## Texte 
hier sind die Texte, die zu diesem Projekt entstanden sind.
```dataview
LIST 
FROM [[Journaling Tipps]]
WHERE contains(tags,"schreiben")
```


## Reference

![[journalingDB.base]]
