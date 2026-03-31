---
training:
tags:
  - [[MOC]]
  - weiterbildung/BTB/Coach
status: cancelled
project:
  - btb/pb
type:
  - [[project]]
  - [[MOC]]
area:
  - lernen
---

> [!info] BTB-Coach
> [[Notizen nach Studienbrief_Coach]]
> [[Fragen nach Studienbrief_Coach]]

**Inhalt**

- [[#Alle Notizen zu Studienbriefen|Alle Notizen zu Studienbriefen]]
- [[#Alle offenen Notizen|Alle offenen Notizen]]
- [[#Alle weitergehenden Infos|Alle weitergehenden Infos]]
- [[#Flashcard Plugin|Flashcard Plugin]]
- [[#Reference|Reference]]



### Alle Notizen zu Studienbriefen

```dataview
Table tags, status

WHERE contains(type, "studienbrief") AND contains(project, "btb/pb") AND !contains(file.name, "Vorlage")
sort status asc
```

### Alle offenen Notizen
```dataview
Table project as "Projekt", status as Status
From !"04 Ressourcen"
WHERE contains(type, "studienbrief") AND
!contains(status, "finalised") AND !contains(status, "hold") AND !contains(status, "upcoming")
```

### Alle weitergehenden Infos
```dataview
LIST status

WHERE contains(type, "concept") AND contains(project, "btb/pb") AND !contains(file.name, "Vorlage")
SORT file.mday DESC
SORT status Asc
```

### Flashcard Plugin
![[spaced repitition plugin]]

---
### Reference
[[000_Home_Dashboard|HomeNote]]
