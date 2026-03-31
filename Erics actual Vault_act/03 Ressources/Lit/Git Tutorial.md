---
note: tvz
training:
tags:
  - Training
title: Claude-Git Tutorial
author:
  - Claude AI
media: e-learning
type:
  - "[[litnote]]"
verlag: ""
veröffentlicht:
isbn:
status: ongoing
project:
area:
context:
---


# Git Tutorial
## 2026-03-10 14:28
___
# Note Section
## Notes
### Wichtige Schritte 
#### Git installieren
mit brew
#### Git Einrichten 
```bash
git config --global user.name "Dein Name"
git config --global user.email "Deine E-Mail"
```

#### Repo 
Ordner erstellen, der beobachtet werden soll. Dann
```bash
cd "erstellter Ordner"
git init
```

#### Statusabfrage
```bash
git status
```

### Das Konzept von git

#### Die Working Area
Dateien, die ins in einer allerersten Fassung ins Repo gelegt werden, wandern ersteinmal in die Working-Area. Das bedeutet, git erkennt die Datei, macht aber nichts mit ihr. Eine Statusabfrage mit
```bash
git status
```

wird deswegen die Datei nur als 'untracked ausgeben'. 
Wird eine Datei, zu der es bereits mind. einen Schnappschuss gibt verändert, wandert diese auch zunächst in die Working Area. Eine Statusabfrage erzeugt den Status 'Modified' 

#### Die Staging Area 
##### Hinzufügen
Dateien, die soweit fertig sind, können aus der Working-Area heraus nicht committed werden. Hierfür müssen sie erst aktiv in die Staging Area verschoben werden. Dies geschieht mit:

```bash
git add
```

Hier können einzelne Dateien mit
```bash
git add "Dateiname"
```
hinzugefügt werden. Dateien können auch durch Leerzeichen getrennt eingegeben werden, wenn mehrere geaddet werden sollen.

Command für: Füge alle zur Stage Area hinzu:
```bash
git add .
```

##### Entfernen
Sollten wir Dateien, die noch nicht fertig waren für den Commit fälschlicherweise in die Staging Area gelegt haben, dann können wir diese auch wieder zurückholen. Der Befehl hierzu lautet:

```bash
git restore --staged "Dateiname"
```

#### Repository (Snapshots)
Wenn git die Dateien als neue Versionen abspeichern soll, dann kann man mit 
```bash
git commit -m "Commit-Message"
```

einen neuen Schnappschuss aus den Dateien der Staging Area erzeugen. Der Befehl git commit nimmt immer **alle** Dateien aus der Staging Area. Einzelne daraus zu commiten ist nicht möglich. Die Auswahl des Schnappschusses erfolgt somit immer über

```bash
git add
```


#### Überblick des Konzepts

![[Pasted image 20260310143128.png]]

### Versionskontrolle
#### Status von Änderungen
Änderungen an den Dateien bekommt ein von git überwachter Ordner immer mit. Er gibt den Status der Änderungen immer über
```bash
git status
```
aus. 
Liegen Änderungen vor, gibt git ein 'modified' aus.

#### Inhaltliche Änderungen 
Wenn wir eine commitete Datei verändern, können wir die genauen Änderungen (sofern Textbasiert) mit:
```bash
git diff
```
ausgeben. 
So kann man genau nachvollziehen welche Änderungen die Datei im Working-Area gegenüber dem letzten Commit aufweist

#### Versionshistorie
Die Historie der commits kann mit 

```bash
git log
```

angezeigt werden. Die Änderungen werden angezeigt als ID des Commits, Author, Datum und das letzte Commit zeigt den Standort in der Versionshistorie an. Man kann in git verschiedene Äste erstellen und commits in diesen verschiedenen Ästen machen. Die 'Normale' Anzeige ist: HEAD->main. D.h. dass der Commit im Branch: main, also dem Hauptzweig erfolgt ist.

Für eine übersichtlichere Darstellung nutze die Option: --oneline.

### In Versionen springen 
#### Zurück in eine ältere Version 
Man kann in Git in einen älteren Schnappschuss springen und dort schauen, wie der Inhalt des Repos zu diesem Zeitpunkt war. Der Befehl dazu lautet:

```bash
git checkout "Name des Commits"
```
Vorsicht: hier ist der Alphanumerische Name des Commits gemeint und nicht die Commit-Message.

git beamt einen dann in einen anderen Status in der Zeit und gibt an, man sein in einem "detached HEAD state".

Zurück kommt man dann wieder mit:
```bash
git checkout main
```

#### Was wenn ich einen früheren Schnappschuss verändern will
##### Alten Commit verwerfen
Einen alten Commit kann ich entweder mit 

```bash
git reset
```
oder 
```bash
git revert
```

verwerfen. 
###### Git revert
Revert macht einen Commit rückgängig, löscht ihn aber nicht. Stattdessen nimmt "git revert" den Stand vor dem letzten Commit und committed ihn einfach nochmal hinter dem zu ändernden Commit. Dabei bleiben alle Daten erhalten und der Zustand wird zurückgesetzt.

###### Git reset
Reset gibt es in verschiedenen "Flavours".

```bash
git reset --soft HEAD~1
```
Löscht den letzten Commit (einen vor HEAD) und legt die dort commiteten Dateien zurück in die Staging Area.

```bash
git reset HEAD~1
```
Wie --soft, nur dass die Daten nicht in der Staging Area sind, sondern in der Working-Area.

```bash
git reset --hard HEAD~1
```
wie git reset (ohne flag) aber löscht auch die Dateien aus der Working-Area. Dann ist alles weg. Also Vorsicht hierbei.


##### Neuen Ast erstellen
Siehe zuerst [[# Branches]]
Hier können die Dateien angesehen werden. Verändert werden können sie auch, aber wenn man diese veränderten Dateien erneut commiten will, dann sollte man das am besten in einem neuen Ast (Branch) machen. So können beide Versionen behalten werden und parallel beobachtet werden. 

### Branches

Branches sind Verästelungen in der Versionshistorie. Diese können unabhängig voneinander angelegt werden.

Das ist ein normaler Zeitstrahl:
e360c3e → 156de4d
"erster    "README
Snapshot"   updated"

Ein Branch wäre sowas wie:
![[Pasted image 20260311174956.png]]

Typische Situationen für Branches:

- Du willst eine neue Idee ausprobieren, ohne das funktionierende Projekt zu gefährden
- Du arbeitest an Feature A, hast aber plötzlich eine Idee für Feature B
- Du willst etwas riskantes ausprobieren mit der Sicherheit, es wegwerfen zu können

Achte darauf, dass 'main' immer die stabile Basis bleibt.

#### Alle Branches anzeigen
Man kann sich alle Branches im Repo anzeigen lassen mit dem Befehl:
```bash
git branch
```

#### Neuen Branch anlegen 
```bash
git branch "Name des Branches"
git switch -c "Name des Branches"
```
Branch erzeugt einen neuen Branch, bleibt aber, wo er ist (HEAD->main)
switch -c erzeugt einen neuen Branch und springt gleich dortin.

#### Branches zusammenführen
Wenn die Änderungen im Branch OK sind, kann der Branch wieder ins main zusammengeführt werden. Hierzu stellen wir sicher, dass wir im Main sind mit:
```bash
git switch main
```
danach kann man die Ergebnisse des letzten commits aus dem Branch nach main mergen.
```bash
git merge "Name des Branches"
```

#### Konflikte 
Konflikte können entstehen, wenn in einer Datei auf beiden branches Änderungen vorgenommen wurden. nun muss man schauen, dass die 'Richtigen Änderungen mitgenommen werden'. In einer TEXT-Datei erstellt git eine genaue Analyse des Konfliktes 
```text
erickrupp@Mac git-tutorial % cat README.txt
Mein erstes Git-Projekt
Heute lerne ich git commit kennen
<<<<<<< HEAD
=======
Das ist ein Experiment
>>>>>>> mein-experiment
```

Der Konflikt muss dann mauell gelöst werden und dann kann die Datei neu geadded und auf main committet werden. 

#### Branch löschen
Gemergete Branches können dann gelöscht werden 
```bash
git branch -d "Name des Branches"
```

### Github
Mein Account heißt: erickrupp.
#### Arbeiten und an Github senden
Wenn ich alles erledigt habe, dann soll ich folgendes machen:
```bash
# Änderungen machen
git add .
git commit -m "Was ich gemacht habe"
git push
```

Hier gilt:
git add . - Fürs hinzufügen zur Staging Area 
git commit - für das Erstellen eines neuen Schnappschusses
git push - für das weiterleiten aller Änderungen an Github

#### Ein existierendes Repo von Github holen
```bash
git clone git@github.com:deinbenutzername/deinrepo.git
```

#### Aktuelle Änderungen von Github holen
Immer aus dem Ordner heraus, in dem das lokale Repo liegt.

```bash
git pull
```

### .gitignore - Dateien und Ordner, die ignoriert werden sollen
## 📝 Eine .gitignore erstellen



```bash
nano .gitignore

Dort trägst du einfach ein was ignoriert werden soll – eine Zeile pro Eintrag:

.DS_Store
*.log
geheime-passwoerter.txt
node_modules/
```


- **`.DS_Store`** – diese exakte Datei ignorieren
- **`*.log`** – alle Dateien die auf `.log` enden ignorieren (`*` ist ein Platzhalter)
- **`node_modules/`** – einen ganzen Ordner ignorieren

Speichern mit `Ctrl + O` → `Enter` → `Ctrl + X`

Dann wie gewohnt committen:

bash

```bash
git add .gitignore
git commit -m ".gitignore hinzugefügt"
git push
```

## 📋 Der komplette Ablauf einmalig auf CachyOS

**Schritt 1 – Git installieren** (falls noch nicht vorhanden):

bash

```bash
sudo pacman -S git
```

**Schritt 2 – Git konfigurieren** (erinnerst du dich aus Modul 2?):

bash

```bash
git config --global user.name "Dein Name"
git config --global user.email "deine@email.de"
```

Wichtig: dieselbe E-Mail wie auf GitHub!

**Schritt 3 – SSH-Schlüssel erstellen:**

bash

```bash
ssh-keygen -t ed25519 -C "deine@email.de"
```

**Schritt 4 – Schlüssel zu GitHub hinzufügen:**

bash

```bash
cat ~/.ssh/id_ed25519.pub
```

Den angezeigten Schlüssel kopieren und auf GitHub unter Settings → SSH keys → New SSH key einfügen – genau wie auf dem Mac. Aber diesmal mit einem anderen Namen, z.B. `Mein CachyOS`.

**Schritt 5 – Repo klonen:**



````bash
cd ~/Projekte
git clone git@github.com:deinbenutzername/git-tutorial.git
```

Ab jetzt funktioniert auf CachyOS alles genau wie auf dem Mac. 😊

---

## 🔄 Der Alltag mit zwei Rechnern

Das ist der Workflow den du verinnerlichen solltest:
```
Morgens am CachyOS anfangen:
git pull                    ← neuesten Stand von GitHub holen

...arbeiten...

git add .
git commit -m "Was ich gemacht habe"
git push                    ← zu GitHub hochladen

Abends am Mac weitermachen:
git pull                    ← neuesten Stand holen
...und so weiter
```

**Die goldene Regel:** Immer zuerst `git pull` bevor du anfängst zu arbeiten – so vermeidest du unnötige Konflikte zwischen den Rechnern.

---

## ⚠️ Was passiert wenn du `git pull` vergisst?

Stell dir vor du arbeitest auf beiden Rechnern ohne zu pullen:
```
GitHub:   A → B → C
Mac:      A → B → D        ← du hast D gemacht ohne C zu pullen
```

Git wird beim `git push` meckern:
```
! [rejected] main -> main (fetch first)
````

Die Lösung:

```bash
git pull
# Eventuellen Konflikt lösen
git push
```



## Key-Learnings


---
## Reference:



**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]