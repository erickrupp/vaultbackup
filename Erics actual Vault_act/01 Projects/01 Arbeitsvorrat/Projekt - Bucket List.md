---
type:
  - "[[project]]"
status: new
date: 2026-01-19 14:23
aliases:
goal:
area:
context:
---


# Bucket List
## 2026-01-19 14:23

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
FROM [[Bucket List]]
WHERE contains(type, "project")
```


### Mit dem Project verlinkte Ressourcen
```dataview
list status 
WHERE contains(project, [[Bucket List]])
WHERE contains(type, "research") OR contains(type, "concept") OR contains(type, "evergreen") OR contains(type, "methode") OR contains(type, "litnote")
```

| Name der Aktivität                | Mit wie vielen Menschen kann ich das machen | Nötige Ressourcen                  | Schlagwort |
| --------------------------------- | ------------------------------------------- | ---------------------------------- | ---------- |
| Geocaching                        | 1-5                                         | Smartphone, Geocaching-App         | Abenteuer  |
| Nachtwanderung                    | 1-10                                        | Taschenlampe, festes Schuhwerk     | Abenteuer  |
| Floßbau am See                    | 2-6                                         | Holz, Seil, Werkzeug               | Abenteuer  |
| Escape Room                       | 2-6                                         | Buchung im Escape Room             | Abenteuer  |
| Kletterpark besuchen              | 1-10                                        | Eintritt, festes Schuhwerk         | Abenteuer  |
| Schnitzeljagd im Wald             | 2-10                                        | Karte, Hinweise                    | Abenteuer  |
| Wildcampen im Garten              | 1-5                                         | Zelt, Schlafsack                   | Abenteuer  |
| Kajakfahren auf einem Fluss       | 1-4                                         | Kajak, Paddel, Schwimmweste        | Abenteuer  |
| Höhlenwanderung                   | 1-10                                        | Helm, Taschenlampe                 | Abenteuer  |
| Bogenschießen                     | 1-5                                         | Bogen, Pfeile, Zielscheibe         | Abenteuer  |
| Besuch eines Trampolinparks       | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Freizeitparks        | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Tierparks            | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Science Centers      | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Planetariums         | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Aquariums            | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Museums              | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines botanischen Gartens  | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines historischen Ortes   | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Kunstgalerie         | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Bauernhofs           | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Schmetterlingshauses | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Vogelparks           | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Reptilienhauses      | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Puppentheaters       | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Zirkus               | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Freizeitbades        | 1-10                                        | Eintritt, Badebekleidung           | Abenteuer  |
| Besuch eines Kletterzentrums      | 1-10                                        | Eintritt, Kletterausrüstung        | Abenteuer  |
| Besuch eines Minigolfplatzes      | 1-10                                        | Eintritt, Golfschläger             | Abenteuer  |
| Besuch eines Bowlingcenters       | 1-10                                        | Eintritt, Bowlingschuhe            | Abenteuer  |
| Besuch eines Skateparks           | 1-10                                        | Skateboard, Schutzkleidung         | Abenteuer  |
| Besuch eines BMX-Parks            | 1-10                                        | BMX-Rad, Schutzkleidung            | Abenteuer  |
| Besuch eines Wassersportzentrums  | 1-10                                        | Eintritt, Wassersportausrüstung    | Abenteuer  |
| Besuch eines Segelclubs           | 1-10                                        | Segelboot, Schwimmweste            | Abenteuer  |
| Besuch eines Reitstalls           | 1-10                                        | Eintritt, Reitausrüstung           | Abenteuer  |
| Besuch eines Golfplatzes          | 1-10                                        | Eintritt, Golfausrüstung           | Abenteuer  |
| Besuch eines Tennisclubs          | 1-10                                        | Eintritt, Tennisausrüstung         | Abenteuer  |
| Besuch eines Fußballstadions      | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Basketballspiels     | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Eishockeyspiels      | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Baseballspiels       | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Rugbyspiels          | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Volleyballspiels     | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Handballspiels       | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Badmintonspiels      | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Tischtennisspiels    | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Squashspiels         | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Boxkampfs            | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Wrestlingmatches     | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Kampfsportturniers   | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Tanzwettbewerbs      | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Musikfestivals       | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Filmfestivals        | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Theaterstücks        | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Musicals             | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Konzerts             | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Opernhauses          | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Balletts             | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Jazzclubs            | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Comedyclubs          | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Varietés             | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Kabaretts            | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Poetry Slams         | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Literaturfestivals   | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Kunsthandwerksmarkts | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Flohmarkts           | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Weihnachtsmarkts     | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Ostermarkts          | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Bauernmarkts         | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Wochenmarkts         | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Antikmarkts          | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Trödelmarkts         | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Kunstmarkts          | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Designmarkts         | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Handwerksmarkts      | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Gartenmarkts         | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Pflanzenmarkts       | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Blumenmarkts         | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Fischmarkts          | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Käsemarkts           | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Weinmarkts           | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Biermarkts           | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Schokoladenmarkts    | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Kaffeemarkts         | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Teemarkts            | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Gewürzmarkts         | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Kräutermarkts        | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Honigmarkts          | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Olivenölmarkts       | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Brotmarkts           | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Backwarenmarkts      | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Konditoreimarkts     | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Patisseriemarkts     | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Eismarkts            | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Süßwarenmarkts       | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Spielzeugmarkts      | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Modellbaumarkts      | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Sammlermarkts        | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Antiquitätenmarkts   | 1-10                                        | Eintritt                           | Abenteuer  |
| Besuch eines Kunsthandwerksmarkts | 1-10                                        | Eintritt                           | Abenteuer  |
| Kochkurs                          | 1-10                                        | Kochzutaten, Kochutensilien        | Lernen     |
| Töpferkurs                        | 1-10                                        | Ton, Töpferwerkzeug                | Lernen     |
| Malworkshop                       | 1-10                                        | Farben, Pinsel, Leinwand           | Lernen     |
| Fotografie-Workshop               | 1-10                                        | Kamera, Fotobearbeitungssoftware   | Lernen     |
| Sprachkurs                        | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Tanzkurs                          | 1-10                                        | Tanzkleidung, Musik                | Lernen     |
| Yoga-Kurs                         | 1-10                                        | Yogamatte, bequeme Kleidung        | Lernen     |
| Meditationstraining               | 1-10                                        | Ruhiger Raum, Meditationsmusik     | Lernen     |
| Schreibworkshop                   | 1-10                                        | Papier, Stift, Laptop              | Lernen     |
| Schauspielkurs                    | 1-10                                        | Skripte, Bühne                     | Lernen     |
| Musikunterricht                   | 1-10                                        | Musikinstrument, Noten             | Lernen     |
| Gartenbaukurs                     | 1-10                                        | Pflanzen, Gartenwerkzeug           | Lernen     |
| Imkerkurs                         | 1-10                                        | Bienenstock, Schutzkleidung        | Lernen     |
| Nähkurs                           | 1-10                                        | Stoff, Nähmaschine, Faden          | Lernen     |
| Strickkurs                        | 1-10                                        | Wolle, Stricknadeln                | Lernen     |
| Häkelkurs                         | 1-10                                        | Garn, Häkelnadel                   | Lernen     |
| Schmuckherstellungskurs           | 1-10                                        | Perlen, Draht, Werkzeug            | Lernen     |
| Holzschnitzkurs                   | 1-10                                        | Holz, Schnitzwerkzeug              | Lernen     |
| Schweißkurs                       | 1-10                                        | Schweißgerät, Schutzkleidung       | Lernen     |
| Elektronikkurs                    | 1-10                                        | Elektronische Bauteile, Lötkolben  | Lernen     |
| Programmierkurs                   | 1-10                                        | Computer, Software                 | Lernen     |
| Webdesignkurs                     | 1-10                                        | Computer, Software                 | Lernen     |
| Grafikdesignkurs                  | 1-10                                        | Computer, Software                 | Lernen     |
| Videobearbeitungskurs             | 1-10                                        | Computer, Software                 | Lernen     |
| Fotobearbeitungskurs              | 1-10                                        | Computer, Software                 | Lernen     |
| Social Media Marketing Kurs       | 1-10                                        | Computer, Internetzugang           | Lernen     |
| SEO-Kurs                          | 1-10                                        | Computer, Internetzugang           | Lernen     |
| Online-Marketing-Kurs             | 1-10                                        | Computer, Internetzugang           | Lernen     |
| Finanzmanagementkurs              | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Aktienhandel-Kurs                 | 1-10                                        | Computer, Internetzugang           | Lernen     |
| Immobilienkurs                    | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Fotografie-Workshop               | 1-10                                        | Kamera, Fotobearbeitungssoftware   | Lernen     |
| Erste-Hilfe-Kurs                  | 1-10                                        | Lehrmaterialien, Erste-Hilfe-Set   | Lernen     |
| Selbstverteidigungskurs           | 1-10                                        | Schutzkleidung, Trainingsraum      | Lernen     |
| Pilates-Kurs                      | 1-10                                        | Pilatesmatte, bequeme Kleidung     | Lernen     |
| Tai Chi-Kurs                      | 1-10                                        | Bequeme Kleidung, ruhiger Raum     | Lernen     |
| Achtsamkeitstraining              | 1-10                                        | Lehrmaterialien, ruhiger Raum      | Lernen     |
| Ernährungsberatung                | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Kräuterkunde-Kurs                 | 1-10                                        | Kräuter, Lehrmaterialien           | Lernen     |
| Aromatherapie-Kurs                | 1-10                                        | Ätherische Öle, Lehrmaterialien    | Lernen     |
| Massagekurs                       | 1-10                                        | Massageöl, Lehrmaterialien         | Lernen     |
| Feng Shui-Kurs                    | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Astrologie-Kurs                   | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Tarotkarten-Lesen-Kurs            | 1-10                                        | Tarotkarten, Lehrmaterialien       | Lernen     |
| Numerologie-Kurs                  | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Hypnosekurs                       | 1-10                                        | Lehrmaterialien, ruhiger Raum      | Lernen     |
| NLP-Kurs                          | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Coaching-Ausbildung               | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Persönlichkeitsentwicklungskurs   | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Leadership-Training               | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Kommunikationstraining            | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Konfliktmanagementkurs            | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Zeitmanagementkurs                | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Projektmanagementkurs             | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Teamführungskurs                  | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Präsentationstraining             | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Verhandlungstraining              | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Verkaufstraining                  | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Kundenservice-Training            | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Stressmanagementkurs              | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Burnout-Präventionskurs           | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Resilienztraining                 | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Kreativitätstraining              | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Innovationsworkshop               | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Design Thinking Workshop          | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Agile Methoden Kurs               | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Scrum Master Kurs                 | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Kanban Kurs                       | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Lean Management Kurs              | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Six Sigma Kurs                    | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Qualitätsmanagementkurs           | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Umweltmanagementkurs              | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Nachhaltigkeitskurs               | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| CSR-Kurs                          | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Ethikkurs                         | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Philosophie-Kurs                  | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Geschichte-Kurs                   | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Kunstgeschichte-Kurs              | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Literaturkurs                     | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Musikgeschichte-Kurs              | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Filmgeschichte-Kurs               | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Theatergeschichte-Kurs            | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Architekturgeschichte-Kurs        | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Archäologiekurs                   | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Anthropologiekurs                 | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Soziologiekurs                    | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Psychologiekurs                   | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Politikwissenschaftskurs          | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Wirtschaftskurs                   | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Rechtskurs                        | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |
| Medizinischer Grundkurs           | 1-10                                        | Lehrmaterialien, Online-Ressourcen | Lernen     |


## Reference
**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]