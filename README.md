# Zitation nach FOM

Dieser Zitationsstil richtet sich nach dem "Leitfaden zur formalen Gestaltung von Seminar- und Abschlussarbeiten" der FOM Hochschule mit dem Stand aus dem Januar 2024.
**das ganze ist WIP, nicht alles funktioniert und ich übernehme keine Garantie auf die Ergebnisse**

## Installation 

Dieser Zitationsstil kann in jeder üblichen Zitationssoftware verwendet werden. Eine Option ist die open-source Software Zotero.

### Zotero installieren

- Zotero installieren
- falls benötigt das Plugin für den verwendeten Textprozessor installieren

### Stil installieren

- Doppelklick auf `fom-zitation-nach-leitfaden-2024 (xx).csl` und installieren

oder:

- in Zotero: Bearbeiten>Einstellungen>Zitieren>+ <img width="797" height="356" alt="image" src="https://github.com/user-attachments/assets/cd2faa21-11ce-4339-b5dd-c283fcdad62d" />
- `fom-zitation-nach-leitfaden-2024 (xx).csl` Datei auswählen
- fertig

## FOM 2024 verwenden

### Funktionen

Momentan sind die Medientypen Buch, Website und Zeitschriftenartikel voll unterstützt.
Zusätzlich können selbst geführte Interviews mit aufgenommen werden. Siehe hierzu das Kapitel [Interview](#interview).
Der Medientyp Buchteil ist mit zusätzlichen Schritten unterstützt, dazu bei [Aufsatz aus Sammelwerk bzw. Buchteil](#aufsatz-aus-sammelwerk-bzw-buchteil) mehr 

Der Stil verwendet den Eintrag Kurztitel (title-short) für das von der FOM geforderte Stichwort.
Folgende Felder müssen für eine korrekte Zitation nach dem Leitfaden gefüllt sein:

#### benötigte Angaben

| Medientyp                     | benötigte Felder                                                                                                                                                                                                                                                                                                                                                           |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <h5>Buch</h5>                 | Autor (author) <br>Kurztitel (title-short) <br>Datum / Erscheinungsjahr (issued) <br>Titel (title) <br>Auflage (edition) <br>Ort (publisher-place) <br>Verlag (publisher)                                                                                                                                                                                                  |
| <h5>Zeitschriftenartikel</h5> | Autor (author) <br>Kurztitel (title-short) <br>Datum / Erscheinungsjahr (issued) <br>Titel (title) <br>Zeitschriften-Abkürzung (container-title-short) <br>Band (volume) <br>Ausgabe (issue) <br>Seiten (page)                                                                                                                                                             |
| <h5>Website</h5>              | Autor (author) <br>Kurztitel (title-short) <br>Datum (issued) <br>Titel (title) <br>URL (URL) <br>Heruntergeladen am (accessed)                                                                                                                                                                                                                                            |
| <h5>Buchteil</h5>             | <h5>im Eintrag “Buchteil” </h5>Autor (author) <br>Kurztitel (title-short) <br>Datum (issued) <br>Titel (title) <br>Herausgeber (editor) <br>Buchtitel (container-title) <br><h5> im Eintrag “Buch” </h5>Herausgeber (editor) <br>Kurztitel (title-short) <br>Datum (issued) <br>Titel (title) <br>Auflage (edition) <br>Ort (publisher-place) <br>Verlag (publisher) |
| <h5>Interview</h5>            | <h5>in den gewöhnlichen Feldern </h5>Interview mit (author) <br>Datum (date)<br>Kurztitel (title-short)<br>Archiv (archive)<br>Standort im Archiv (archive_location)<br><h5>im Feld Extra *[mehr hier](#interview)*</h5>Event Place: <br>Page:<br>Page-First:                                                                                                                                                                                                                                                                                                                                                                           |


Wird ein Feld, wie das Datum leer gelassen, wird es durch o. J. ersetzt. Folgende Felder werden ersetzt, wenn sie leer gelassen werden:

| Feld                   | Platzhalter                                                             |
| ---------------------- | ----------------------------------------------------------------------- |
| Datum (issued)         | `o. J.` in der Fußnote <br>`keine Datumsangabe` im Literaturverzeichnis | 
| Author (author)        | `o. V.`                                                                 |
| Seite (locator=”page”) | `o. S.`                                                                 |
| Ort (publisher-place)  | `o. O.`                                                                 | 

#### Verwendung 

Wird eine Fußnote angelegt, kann im Feld Präfix ein `Vgl.` bei einem indirekten Zitat eingefügt werden. Wird das Feld Seite leer gelassen, wird statt einer Seite `o. S.` (ohne Seite) angegeben.
<img width="1076" height="708" alt="image" src="https://github.com/user-attachments/assets/31cee77e-c7b6-42e8-b8d2-066c267bf91f" />
Alle Werke, die auf diese Art in einer Fußnote erwähnt wurden, werden bei Erstellung des Literaturverzeichnisses automatisch eingetragen.

##### Buch

Ist ein Buch in der ersten Auflage, soll die Auflage nicht im Verweis im Literaturverzeichnis stehen, hierzu bitte das Feld `Auflage (edition)` leer lassen. (Gilt auch bei Buchteilen / Sammelwerken)
*Bei “normalen” Büchern, die keine Sammelwerke sind, muss das Feld Herausgeber (editor) leer bleiben!"*

##### Aufsatz aus Sammelwerk bzw. Buchteil

 Um einen Buchteil nach Vorgabe hinzuzufügen müssen zwei Einträge in das Literaturverzeichnis aufgenommen werden. Einer für den Artikel aus dem Buch und einen für das gesamte Buch. Dieses Verhalten wird von Citation Style Language (CSL) nicht unterstützt. Somit ist es nur über Umwege zu erreichen.
 Für die korrekte Zitation wird ein sowohl ein Buchteil (chapter), als auch ein Buch (book) angelegt. Hierbei sind die bei [benötigte Angaben](#benötigte-angaben) aufgeführten Felder zu befüllen.
 
##### Interview

Beim Interview müssen zusätzliche Parameter im Feld `Extra` eingegeben werden, da Zotero für diese Funktionen noch keine Felder hat. Siehe hierzu [Extra](#extra)

Interviews werden in einem gesondertes Quellenverzeichnis angegeben siehe hierzu [Literaturverzeichnis und Quellenverzeichnis](#literaturverzeichnis-und-quellenverzeichnis)

Wird kein `Event Place` angegeben, wird davon ausgegangen, dass das Interview online statt gefunden hat.

Die Einträge `Page` und `Page First` sind austauschbar. `Page` kann z.B. für Seitenbereiche verwendet werden, während `Page First` die Anfangsseite beinhaltet.

#### Literaturverzeichnis und Quellenverzeichnis

Das Literaturverzeichnis ist alphabetisch nach dem ersten Nachnamen des ersten Autors sortiert, wobei alle “klassische” Literatur zuerst kommt und alle Internetquellen danach eingefügt werden. Werden zusätzlich andere Quellen, wie Interviews verwendet, die nicht zur Literatur gehören, werden sie in ein separates Quellenverzeichnis einsortiert.

Optional kann über einen Eintrag ``Titel: (frei wählbar) z.B. Internetquellen; Eintragsart: Fall (legal-case)`` eine Automatische Überschrift im Literaturverzeichnis erzeugt werden. Hierzu wird dieser Eintrag in einer Fußnote zitiert, woraufhin im Zotero Plugin der “Refresh” Knopf gedrückt wird. Nun ist die Überschrift im Literaturverzeichnis und die Fußnote kann wieder entfernt werden. Bei erneutem “Refresh” verschwindet die Überschrift wieder.
Um zwischen einem Eintrag für `Internetquellen` und `Quellenverzeichnis`unterscheiden zu können, wird bei dem zuerst aufgeführten Eintrag (im Normalfall Internetquellen) das Feld Kurztitel leer gelassen, während es bei dem zuletzt aufgeführten Eintrag (Quellenverzeichnis) gefüllt wird. Der Text mit dem es gefüllt wird spielt hierbei keine Rolle.

## Fehler beheben

Falls der Stil sich nicht wie erwartet verhält gibt es folgende Lösungsmöglichkeiten:

- Prüfen ob alle Angaben korrekt ausgefüllt sind
- Refresh in Word klicken
- Dokumenteneinstellungen in Word prüfen
	- Die Literaturangeben sollten als Fußnoten und nicht als Endnoten angezeigt werden.
	- bei einem Artikel aus einer Fachzeitschrift kann hier entweder automatisch eine Abkürzung für den Titel der Veröffentlichung gefunden werden, oder der manuell eingetragene Titel verwendet werden:
		- [ ] Abgekürzte Zeitschriftentitel von MEDLINE verwenden
- Zotero und Word neu starten
- Die betreffende Quelle in Zotero als CSL JSON exportieren und mir schicken

---

<h2>Zusätzliche Informationen</h2>

### Extra

[das meiste aus den Zotero Docs](https://www.zotero.org/support/kb/item_types_and_fields#citeable_fields_not_included_in_zotero)

These item fields are not yet formally supported in Zotero. For citation purposes, you can convert an item of a different type to one of these types by entering them in the [Extra field](#citing-fields-from-extra) in this format:

```
CSL Variable: Value
```

For example:

```
Page First: 20
Page: 30-45
PMID: 123456
Status: in press
Original Date: 1886-04-01
Director: Kubrick || Stanley
```

| Field                    | CSL Variable               | Description                                                                                                                                                                                                |
| ------------------------ | -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| PMID                     | `PMID`                     | The [PubMed identifier](http://en.wikipedia.org/wiki/PMID#PubMed_identifier).                                                                                                                              |
| PMCID                    | `PMCID`                    | The [PubMed Central identifier](https://en.wikipedia.org/wiki/PubMed_Central#PMCID).                                                                                                                       |
| Status                   | `Status`                   | The publication status of an item (e.g., “forthcoming”, “in press”, “advance online publication”).                                                                                                         |
| Submitted Date           | `Submitted`                | The date an item was submitted for publication.                                                                                                                                                            |
| Reviewed Title           | `Reviewed Title`           | The title of a reviewed work.                                                                                                                                                                              |
| Chapter Number           | `Chapter Number`           | The number of the chapter within a book.                                                                                                                                                                   |
| Archive Place            | `Archive Place`            | The geographic location of an archive.                                                                                                                                                                     |
| Event Date               | `Event Date`               | The date an event took place. Enter in ISO format (year-month-day).                                                                                                                                        |
| Event Place              | `Event Place`              | The geographic location of an event.                                                                                                                                                                       |
| Page First               | `Page First`               | Die erste Seite. (hier die erste Seite des Anhangs / Interviews)                                                                                                                                           |
| Page                     | `Page`                     | Die erste Seite. (kann statt Page First verwendet werden, um einen Bereich anzugeben s.o.) *werden Page und Page First verwendet, wird nur Page angezeigt*                                                                                                                                                                                                           |
| Original Date            | `Original Date`            | The original date an item was published. Enter in ISO format (year-month-day).                                                                                                                             |
| Original Title           | `Original Title`           | The original title of a work (e.g., the untranslated title).                                                                                                                                               |
| Original Publisher       | `Original Publisher`       | The publisher of the original version of an item (e.g., the untranslated version).                                                                                                                         |
| Original Publisher Place | `Original Publisher Place` | The geographic location of the publisher of the original version of an item (e.g., the untranslated version).                                                                                              |
| Original Author          | `Original Author`          | A type of Creator. The original creator of a work.                                                                                                                                                         |
| Director                 | `Director`                 | A type of Creator. The director of a film, recording, or broadcast. In Zotero, “Director” is mapped to CSL author. If you need special labels for directors—“(Dir.)”, enter the `Director` label in Extra. |
| Editorial Director       | `Editorial Director`       | A type of Creator. The managing editor of a publication (“Directeur de la Publication” in French).                                                                                                         |
| Illustrator              | `Illustrator`              | A type of Creator. The illustrator of a work.                                                                                                                                                              |


#### Citing Fields from Extra

If a Zotero item type is missing fields that are needed for citations, it is possible to add these fields to the Extra field.

Enter each variable on a separate line at the top of the Extra field in the following format:

```
CSL Variable: Value
```

For example:

```
DOI: 10.1128/AEM.02591-07
Original Date: 1824
PMCID: PMC3531190
```

With the exception of Item Type (CSL `Type`) and Date variables (CSL `Issued`, etc.), variables entered in Extra will not override corresponding values entered in proper Zotero fields.

##### Dates

Dates entered in Extra will override the date entered in Zotero's Date field. Dates must be entered in ISO format (year-month-day). Date ranges can be entered in this format:

```
Issued: 2001-12-15/2001-12-31
```

##### Names

For Creator variables, separate two-field names entered in Extra with two vertical bar characters (`||`), like this:

```
Editorial Director: De Gaulle || Charles
```

---
<a href=”https://github.com/Waldi05/Zitation-nach-FOM”>FOM Zitation nach Leitfaden 2024 (note)</a> © 2025 by Lukas Waldhör is licensed under <a href="https://creativecommons.org/licenses/by-nc/4.0/">CC BY-NC 4.0</a><img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/nc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;">




