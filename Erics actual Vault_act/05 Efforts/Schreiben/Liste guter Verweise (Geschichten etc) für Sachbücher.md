---
training:
tags:
  - schreiben
type:
status: ongoing
project:
  - "[[Projekt - Erste Schritte - Schreiben und Content Creation]]"
area:
  - "[[Persönlich]]"
context:
---


# Liste guter Verweise (Geschichten etc) für Sachbücher
## 2025-01-06 11:42
___
Hier sollen alle Geschichten oder sonstige Dokumente hin, die von Belang für das Schreibprojekt sind. Also:
- Geschichten um zu belegen oder Aufmerksamkeit zu generieren genauso wie 
- Forschungsstudien, die bestimmte Ergebnisse nahelegen oder 
- andere Bücher, die auf ähnliche Themen verweisen.

## Alle Files

```dataview
TABLE context as "Kontext" , type as "Dokumententyp", project as "Projekt"
WHERE context
```


## Geschichten 
```dataview
TABLE context as "Kontext" , type as "Dokumententyp", project as "Projekt"
WHERE context AND contains(type, "geschichte")
```

## Zitate
```dataview
TABLE context as "Kontext" , type as "Dokumententyp", project as "Projekt"
WHERE context AND contains(type, "quote")
```
## Alles andere
```dataview
TABLE context as "Kontext" , type as "Dokumententyp", project as "Projekt"
WHERE context
WHERE !contains(type, "geschichte") AND !contains(type, "quote")
```



---
# Reference:
**ÜBERGEORDNETE NOTIZ** 
[[Projekt - Erste Schritte - Schreiben und Content Creation]]

**LITERATURNOTIZ**
