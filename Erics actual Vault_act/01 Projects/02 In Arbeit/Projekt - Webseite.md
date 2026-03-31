---
training:
tags:
type:
  - "[[project]]"
aliases:
status: ongoing
goal:
area:
context:
---
## Table of content
```dataview
TABLE type as "Dokumententyp", project as "Projekt", status as "Status"
WHERE contains(project, [[Webseite]])
AND !contains(type, "foldernote")
SORT file.ctime ASC
```




## Overhead Notes 

## Blogposts

```dataview
Table project, type
 From "02 Areas/Beruf und Finanzen/OrientierungSinn/Blog/Artikel"
```


```dataview
Table project as Project, file.folder as Folder 
where contains(type,"blogpost") AND contains(project,[[Webseite OrientierungSinn]])
```

## Reference

```dataview
Table project as Project, file.folder as Folder 
where contains(type,"blogpost")
```

**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]