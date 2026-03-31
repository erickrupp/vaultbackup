## Alles neue im 2. Brain
```dataview
Table tags as "Schlagwort", status as "Status", project as " Projekt", status as "Status"
FROM "03 Ressources"
WHERE contains(status, "new")
sort file.mday desc
```

## Alles ongoing im 2. Brain 

```dataview
Table tags as "Schlagwort", project as " Projekt"
FROM "03 Ressources"
WHERE contains(status, "ongoing")
sort file.mday desc
```

