# Zitation-nach-FOM

Dieser Zitationsstil richtet sich nach dem Leitfaden zur formalen Gestaltung von Seminar- und Abschlussarbeiten der FOM Hochschule mit dem Stand aus dem Januar 2024.

## Installation 

Dieser Zitationsstil kann in jeder üblichen Zitationssoftware verwendet werden. Eine Option ist die open-source Software Zotero.

### Zotero installieren

- Zotero installieren
- falls benötigt das Plugin für den verwendeten Textprozessor installieren

### Stil installieren

- in Zotero: Bearbeiten>Einstellungen>Zitieren>+ <img width="797" height="356" alt="image" src="https://github.com/user-attachments/assets/cd2faa21-11ce-4339-b5dd-c283fcdad62d" />
- .csl Datei auswählen
- fertig

## FOM 2024 verwenden

### Funktionen

Momentan sind die Medientypen Buch, Website und Zeitschriftenartikel voll unterstützt.
Der Medientyp Buchteil ist eingeschränkt unterstützt, dazu [[#Buchteil | hier]] mehr 

Der Stil verwendet den Eintrag Kurztitel (title-short) für das von der FOM geforderte Stichwort.
Folgende Felder müssen für eine korrekte Zitation nach dem Leitfaden gefüllt sein:


| Medientyp            | benötigte Felder                                                                                                                                                                                               |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Buch                 | Autor (author) <br>Kurztitel (title-short) <br>Datum / Erscheinungsjahr (issued) <br>Titel (title) <br>Auflage (edition) <br>Ort (publisher-place) <br>Verlag (publisher)                                      |
| Zeitschriftenartikel | Autor (author) <br>Kurztitel (title-short) <br>Datum / Erscheinungsjahr (issued) <br>Titel (title) <br>Zeitschriften-Abkürzung (container-title-short) <br>Band (volume) <br>Ausgabe (issue) <br>Seiten (page) |
| Internetquellen      | Autor (author) <br>Kurztitel (title-short) <br>Datum (issued) <br>Titel (title) <br>URL (URL) <br>Heruntergeladen am (accessed)                                                                                |
| Buchteil             |                                                                                                                                                                                                                |

Wird eine Fußnote angelegt, kann im Feld Präfix ein `Vgl.` bei einem indirekten Zitat eingefügt werden. Wird das Feld Seite leer gelassen, wird statt einer Seite `o. S.` (ohne Seite) angegeben.
<img width="1076" height="708" alt="image" src="https://github.com/user-attachments/assets/31cee77e-c7b6-42e8-b8d2-066c267bf91f" />
Alle Werke, die auf diese Art in einer Fußnote erwähnt wurden, werden bei Erstellung des Literaturverzeichnisses automatisch eingetragen.

#### Buchteil

wip.

#### Literaturverzeichnis

Das Literaturverzeichnis ist alphabetisch nach dem ersten Nachnamen des ersten Autors sortiert, wobei alle “klassische” Literatur zuerst kommt und alle Internetquellen danach eingefügt werden.

Optional kann über einen Eintrag ``Titel: Internetquellen, Eintragsart: Fall (legal-case)`` eine Automatische Überschrift im Literaturverzeichnis erzeugt werden. Hierzu wird dieser Eintrag in einer Fußnote zitiert, woraufhin im Zotero Plugin der “Refresh” Knopf gedrückt wird. Nun ist die Überschrift im Literaturverzeichnis und die Fußnote kann wieder entfernt werden. Bei erneutem “Refresh” verschwindet die Überschrift wieder.






