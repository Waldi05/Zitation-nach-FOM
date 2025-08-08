# Zitation nach FOM

Dieser Zitationsstil richtet sich nach dem "Leitfaden zur formalen Gestaltung von Seminar- und Abschlussarbeiten" der FOM Hochschule mit dem Stand aus dem Januar 2024.

## Installation 

Dieser Zitationsstil kann in jeder üblichen Zitationssoftware verwendet werden. Eine Option ist die open-source Software Zotero.

### Zotero installieren

- Zotero installieren
- falls benötigt das Plugin für den verwendeten Textprozessor installieren

### Stil installieren

- in Zotero: Bearbeiten>Einstellungen>Zitieren>+ <img width="797" height="356" alt="image" src="https://github.com/user-attachments/assets/cd2faa21-11ce-4339-b5dd-c283fcdad62d" />
- .csl Datei auswählen
- fertig

## Funktionen von FOM 2024

Momentan sind die Medientypen Buch, Website und Zeitschriftenartikel voll unterstützt.
Der Medientyp Buchteil ist eingeschränkt unterstützt, dazu [hier](#aufsatz-aus-sammelwerk-bzw-buchteil) mehr 

Der Stil verwendet den Eintrag Kurztitel (title-short) für das von der FOM geforderte Stichwort.
Folgende Felder müssen für eine korrekte Zitation nach dem Leitfaden gefüllt sein:

### benötigte Angaben
| Medientyp            | benötigte Felder                                                                                                                                                                                                                                                                                                                                                           |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <h5>Buch</h5>                 | Autor (author) <br>Kurztitel (title-short) <br>Datum / Erscheinungsjahr (issued) <br>Titel (title) <br>Auflage (edition) <br>Ort (publisher-place) <br>Verlag (publisher)                                                                                                                                                                                                  |
| <h5>Zeitschriftenartikel</h5> | Autor (author) <br>Kurztitel (title-short) <br>Datum / Erscheinungsjahr (issued) <br>Titel (title) <br>Zeitschriften-Abkürzung (container-title-short) <br>Band (volume) <br>Ausgabe (issue) <br>Seiten (page)                                                                                                                                                             |
| <h5>Website</h5>              | Autor (author) <br>Kurztitel (title-short) <br>Datum (issued) <br>Titel (title) <br>URL (URL) <br>Heruntergeladen am (accessed)                                                                                                                                                                                                                                            |
| <h5>Buchteil</h5>             | <h5> im Eintrag “Buchteil” </h5>Autor (author) <br>Kurztitel (title-short) <br>Datum (issued) <br>Titel (title) <br>Herausgeber (editor) <br>Buchtitel (container-title) <br><h5> im Eintrag “Buch” </h5> <br>Herausgeber (editor) <br>Kurztitel (title-short) <br>Datum (issued) <br>Titel (title) <br>Auflage (edition) <br>Ort (publisher-place) <br>Verlag (publisher) |

### FOM 2024 verwenden

Wird eine Fußnote angelegt, kann im Feld Präfix ein `Vgl.` bei einem indirekten Zitat eingefügt werden. Wird das Feld Seite leer gelassen, wird statt einer Seite `o. S.` (ohne Seite) angegeben.
<img width="1076" height="708" alt="image" src="https://github.com/user-attachments/assets/31cee77e-c7b6-42e8-b8d2-066c267bf91f" />
Alle Werke, die auf diese Art in einer Fußnote erwähnt wurden, werden bei Erstellung des Literaturverzeichnisses automatisch eingetragen.

#### Buch

Ist ein Buch in der ersten Auflage, soll die Auflage nicht im Verweis im Literaturverzeichnis stehen, hierzu bitte das Feld `Auflage (edition)` leer lassen. (Gilt auch bei Buchteilen / Sammelwerken)

#### Aufsatz aus Sammelwerk bzw. Buchteil

 Um einen Buchteil nach Vorgabe hinzuzufügen müssen zwei Einträge in das Literaturverzeichnis aufgenommen werden. Einer für den Artikel aus dem Buch und einen für das gesamte Buch. Dieses Verhalten wird von Citation Style Language (CSL) nicht unterstützt. Somit ist es nur über Umwege zu erreichen.
 Für die korrekte Zitation wird ein sowohl ein Buchteil (chapter), als auch ein Buch (book) angelegt. Hierbei sind die [hier](#benötigte-angaben) aufgeführten Felder zu befüllen.



#### Literaturverzeichnis

Das Literaturverzeichnis ist alphabetisch nach dem ersten Nachnamen des ersten Autors sortiert, wobei alle “klassische” Literatur zuerst kommt und alle Internetquellen danach eingefügt werden.

Optional kann über einen Eintrag ``Titel: Internetquellen, Eintragsart: Fall (legal-case)`` eine Automatische Überschrift im Literaturverzeichnis erzeugt werden. Hierzu wird dieser Eintrag in einer Fußnote zitiert, woraufhin im Zotero Plugin der “Refresh” Knopf gedrückt wird. Nun ist die Überschrift im Literaturverzeichnis und die Fußnote kann wieder entfernt werden. Bei erneutem “Refresh” verschwindet die Überschrift wieder.






