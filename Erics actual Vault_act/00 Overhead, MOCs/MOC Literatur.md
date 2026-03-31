---
status: ongoing 
training:
tags: Literatur, 
type: MOC
---
# MOC Literatur
### 2022-11-13 16:27

# NOTES

# Tables
## ebook
```dataview
TABLE author, title, media
from #literatur 
where media = "ebook"
```


## buch
```dataview
TABLE author, title, media
FROM #literatur 
WHERE media = "buch" OR media2 = "buch"
```


## Artikel
```dataview
TABLE author, title, media
FROM #literatur 
WHERE media = "artikel" OR media2 = "artikel"
```


## video
```dataview
TABLE author, title, media
FROM #literatur 
WHERE media = "video" OR media2 = "video"
```

## Blog
```dataview
TABLE author, title, media
FROM #literatur 
WHERE media = "blog" OR media2 = "blog"
```

## Blinks
```dataview
TABLE author, title, media
FROM #literatur 
WHERE media = "blinkist" OR media2 = "blinkist"
```




---

# Lists
## Alle
```dataview
LIST
FROM #literatur 
```

## Buch
```dataview
LIST
FROM #literatur 
WHERE media = "buch" OR media2 = "buch"
```

## E-Book
```dataview
LIST
FROM #literatur 
WHERE media = "ebook" OR media2 = "ebook"
```

## Artikel
```dataview
LIST
FROM #literatur 
WHERE media = "artikel" OR media2 = "artikel"
```

## Video
```dataview
LIST
FROM #literatur 
WHERE media = "video" OR media2 = "video"
```


## Blog
```dataview
LIST
FROM #literatur 
WHERE media = "blog" OR media2 = "blog"
```
## Blinks
```dataview
LIST
FROM #literatur 
WHERE media = "blinkist" OR media2 = "blinkist"
```
## Normen
```dataview
LIST
FROM #literatur 
WHERE media = "norm" OR media2 = "norm"
```


---
# Reference
