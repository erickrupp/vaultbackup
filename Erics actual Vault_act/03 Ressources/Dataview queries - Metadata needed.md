---
status: ongoing
training:
tags:
  - obsidian/dataview
  - pkm
type:
  - "[[concept]]"
---



# **Dataview queries - Metadata needed**
## **2022-07-12 13:06**
___
# Dataview
## Allgemeines
### Die 4 Dataview Ausgabeelemente
- Liste (LIST)
- Tabelle (TABLE)
	- Syntax: TABLE gefolgt von den Metadaten, die in der Tabelle aufgelistet werden sollen. Dann FROM, dann WHERE und SORT
- Aufgaben (TASK)
- Kalender / Datum (CALENDAR)

## FROM
### Basic Features
Der FROM-Filter ist der erste Schritt, Ausgabedateien bzw. Informationen zu filtern. Es können gefiltert werden:
- TAGS (FROM #)
- FILES (FROM PATH/TO/FILE)
- FOLDERS (FROM "PATH/TO/FOLDER")
- LINKS In (FROM '[[]]') Alle Dateien, die auf den Link verweisen
- LINKS Out (FROM outgoing([[]])) Alle Dateien, auf die von der verlinkten Datei verwiesen wird. 

### Expension AND - OR - NOT Matching
Queries can be combined:
- AND (Both have to be true)
	- FROM `#Testtag` AND "Second Brain" = All files with this TAG AND which are in Folder: Second Brain
	- FROM `[[]]` AND `[[]]` = All Fils in the vault which have to have **BOTH** incoming LINKS.
- OR (either of them have to be true)
	- FROM "Folder 1" OR "Folder 2" = All files from both, Folder 1 and 2
	- FROM `#Testtag` or "Folder Test" = All files in the entire vault with the Testtag and all files in the Folder Test no matter what TAG
- NOT Matching (this parameter must be excluded in the result)
	- FROM "Folder 1" AND -#Testtag = All files from Folder 1 but without those having Testtag tagged.

## WHERE
Verfeinert die Ausgabe aus den FROM-Abfragen. Kann hierzu alle möglichen Metadaten nutzen.

Nur WAHRE Aussagen werden zurückgegeben
Möglich sind 
- =; != (Ungleich); <=; >=; <; >
- contains(`wo gesucht wird`, "was gesucht wird") => Bsp. WHERE contains(file.name, "? - ") gibt die Fragen aus dem BTB vault zurück
- !completed = gibt nur offene Tasks zurück (nicht completed)
- completed = gibt nur geschlossene Tasks zurück (completed)

>[!Attention]+ Bei eigenen Metadaten mit mehreren Werten
>Die Werte werden als AND Verknüpfung interpretiert. Deshalb funktioniert bei Abfragen einzelner WERTE: type = VALUE nicht, da beide VALUES da sein müssen.
>Stattdessen: contains(METADATA, "VALUE")!



### automatisch verwaltete Metadaten
- file.ctime = Time file created
- file.mtime = Time file modified
- file.name: The file title (a string).
- file.folder: The path of the folder this file belongs to.
- file.path: The full file path (a string).
- file.ext: The extension of the file type; generally '.md' (a string).
- file.link: A link to the file (a link).
- file.size: The size (in bytes) of the file (a number).
- file.cday: The date that the file was created (just a date).
- file.mday: The date that the file was last modified (just a date).
- file.status:
training:
tags: An array of all unique tags in the note. Subtags are broken down by each level, so `#Tag/1/A` will be stored in the array as `[#Tag, #Tag/1, #Tag/1/A]`.
- file.etraining:
tags: An array of all explicit tags in the note; unlike file.tags, does not include subtags.
- file.inlinks: An array of all incoming links to this file.
- file.outlinks: An array of all outgoing links from this file.
- file.aliases: An array of all aliases for the note.
- file.tasks: An array of all tasks (I.e., `- [ ] blah blah blah`) in this file.
- file.lists: An array of all list elements in the file (including tasks); these elements are effectively tasks and can be rendered in task views.
- file.frontmatter: Contains the raw values of all frontmatter; mainly useful for checking raw frontmatter values or for dynamically listing frontmatter keys.

### Metadaten aus Frontmatter
Alle im YAML-Frontmatter hinterlegte individuelle Metadaten. Für dieses Vault siehe [[#Metadata needed]].
Kann alle möglichen Elemente beinhalten und ist individuell einrichtbar.

Die Metadaten können auch inline vergeben werden. 

> [!INFO] Anwendung von Metadaten
> - Im YAML mit einem Doppelpunkt (Bsp. author:)
> - Inline mit zwei Doppelpunkten (Bsp `author::`)

### SORT
sortiert die Ausgabedaten nach den spezifizierten Kriterien

Bsp. 
SORT file.name asc = nach Dateiname aufsteigend
SORT file.ctime desc = nach creation time absteigend

# Metadata needed
## Literatur:
author:
title:
isbn:
zitiert:
media:

## BTB

## pkm

## Content

## Personen

## JOB
### Training

# meine Abfragen:
## Fragen aus BTB:
LIST
FROM `#BTB`
WHERE contains(file.name, "? - ")

Wenn unterschieden werden muss zwischen Studienbriefen dann WHERE erweitern: AND studienbrief = xxxx
Zwischen Coach und HP-Psych unterschieden werden kann indem der Tag ergänzt wird `#BTB/HP-Psych` oder `#BTB/Coach`
Zwischen den einzelnen Fächern kann unterschieden werden indem die WHERE Abfrage erweitert wird:
WHERE slipbox = "fach_1, fach_2 oder fach_3"

Vereinfacht:
FROM `#BTB/HP-Psych (oder Coach)/Fragen`


Studienbriefe
FROM `#BTB/HP-Psych (oder Coach)/studienbrief`
WHERE studienbrief = xxxx

Ohne Where alle Studienbriefe

Alternative:
FROM `#BTB`
WHERE studienbrief = xxxx AND slipbox = "fach_0"


## TASKS
FROM `was auch immer sinnvoll ist (bspw Projekte)`
WHERE !completed


---
Reference:
**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]