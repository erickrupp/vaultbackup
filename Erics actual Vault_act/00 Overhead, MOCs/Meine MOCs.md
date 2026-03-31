## Notes with MOC as Type:
```dataview
List 
where contains(type,"MOC")
```

## Notes with MOC as Tag
```dataview
LIST 
FROM #MOC 
```
# Notes that contain MOC in the title
```dataview
LIST

WHERE contains(file.name,"MOC")
SORT file.name ASC
```
