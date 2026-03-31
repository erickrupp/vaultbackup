---
type:
  - "[[project]]"
status: hold
date: 2025-01-06 10:25
aliases:
goal:
  - "[[Eigene Projekte]]"
area:
  - "[[Persönlich]]"
---


# Erste Schritte - Schreiben und Content Creation
## 2025-01-06 10:25

Aus dem ersten Projekt zum Ziel: [[Eigene Projekte]], nämlich [[Klarheit über Projekte, die in den nächsten Monaten gemacht werden, gewinnen]], habe ich mir im Dokument: [[Potenzielle Projekte - Brain Dump, Bewertung und what next]] entsprechende Gedanken über die möglichen Projekte und Inhalte gemacht. 
Hier kam es zu der Bewertung, dass das Schreiben und die Content Creation die oberste Priorität haben sollen und die anderen Dinge (Notizbücher binden, Arbeitsplatz einrichten und Computerspielereien) darauf einzahlen sollen und eben nicht selbstzweckhaft betrieben werden sollen.

Deswegen geht es nun um die nächsten Schritte, die ich wie folgt festgelegt habe:
![[Potenzielle Projekte - Brain Dump, Bewertung und what next#Nächste Schritte]]

Also geht es im nächsten Schritt um die Etablierung einer Liste möglicher Inhalte und die entsprechenden Aufhänger, mit denen man die Inhalte aufbereiten kann. Dies wird im Dokument [[MOC Schreiben - List of Contents]] geschehen. 
Außerdem wird es eine [[Liste guter Verweise (Geschichten etc) für Sachbücher]] geben in der ich die Geschichten sammeln werde, die mir bei der Lektüre von Büchern, Blogs u.ä. aufgefallen sind und die ich gerne vielleicht verwenden möchte. Hierbei ist eine Zuordnung von möglichen Kontexten relevant um einordnen zu können, wo und wann die Geschichten benutzt werden können.
Ich überlege gerade, ob es nicht cool wäre ein neues property: 'context' zu bauen, damit man alle entsprechenden Elemente per Dataview erfassen und sortieren kann. Dann wäre es möglich alle Elemente, bei denen das Property nicht leer ist zu sammeln und in einer Tabelle aufzulisten nach context und Typ, wobei Typ noch mindestens um 'geschichte' oder so ergänzt werden muss. 





**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]

---
# Project Informationen 

## Related to
### Goal 
```button
name New Goal
type command
action QuickAdd: New Goal
color green
```
^button-newgoal
### Area 
```button
name New Area
type command
action QuickAdd: New Area
color yellow
```
^button-newarea

### Project


```button
name New Project
type command
action QuickAdd: New Project
color blue
```
^button-newProject
#### Mit dem Project verlinkte Projekte 
```dataview
list status 
FROM [[Schreiben und Content Creation]]
WHERE contains(type, "project")
```


### Mit dem Project verlinkte Ressourcen
```dataview
list status 
WHERE contains(project, [[Schreiben und Content Creation]])
WHERE contains(type, "research") OR contains(type, "concept") OR contains(type, "evergreen") OR contains(type, "methode")
```


