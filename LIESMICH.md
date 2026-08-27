# Roseggerstrasse 9, Kirchheim unter Teck, Wohnung Nr. 3

## Was in diesem Ordner liegt

    index.html          das Expose
    bilder/             17 Bilddateien, vom Expose eingebunden
    unterlagen/         17 PDF, ueber die Downloadkarten verlinkt

Alle drei muessen beieinander bleiben. Fehlt "bilder", zeigt die Seite
keine Fotos. Fehlt "unterlagen", laufen die Downloads ins Leere.

## Hochladen

Ein eigenes Repository fuer diese Wohnung anlegen. Dann auf
"Add file", danach "Upload files", und in das Fenster alles drei
zusammen ziehen:

    index.html
    bilder            (der ganze Ordner)
    unterlagen        (der ganze Ordner)

Wichtig: nicht den Ordner "Wohnung-3" hochladen, sondern seinen Inhalt.
Die index.html muss im Repository ganz oben liegen.

## Pages einschalten

Settings, dann Pages. Bei Source "Deploy from a branch" waehlen,
Branch `main`, Ordner `/ (root)`. Speichern. Der erste Aufbau dauert
ein bis zwei Minuten, danach steht die Adresse oben auf der Seite.

## Groessen

Die PDF sind verkleinert, damit der Weblader von GitHub sie annimmt.
Vorher 44 MB, jetzt 18,7 MB. Die groesste Datei ist
13_Gebaeudeversicherung.pdf mit 4,4 MB. Scans liegen bei 150 dpi,
Text und Plaene bleiben lesbar.

GitHub nimmt ueber den Weblader je Vorgang nur rund 25 MB. Ein Upload
mit index.html, bilder und unterlagen zusammen sind rund 20 MB
und passt damit in einen Vorgang. Wird es dennoch abgewiesen, in zwei
Vorgaengen hochladen: erst index.html und bilder, danach unterlagen.

Die Seite selbst laedt beim Besucher mit rund 1,5 MB, davon 1,4 MB Bilder,
die nach dem Text nachgeladen werden. Die PDF laedt nur, wer sie anklickt.

## Nicht enthalten, mit Absicht

Grundbuchauszug, Restnutzungsdauergutachten, Kaufpreisaufteilung,
Mietvertrag und das Protokoll der Bestandsaufnahme liegen nicht in
"unterlagen". Sie enthalten personenbezogene Daten. Auf GitHub Pages ist
jede Datei im Repository oeffentlich abrufbar, auch wenn sie auf der
Seite nicht verlinkt ist. Im Expose steht deshalb, dass diese Unterlagen
bei ernsthaftem Kaufinteresse nachgereicht werden.

## Falls ein Ordner anders heissen soll

In der index.html steht im Skript genau eine Zeile:

    var DOKBASE='unterlagen/';

Nur diese aendern. Der Schraegstrich am Ende muss bleiben.
Der Bildordner ist in den Bildpfaden hinterlegt und heisst "bilder".

## Hinweis zum Oeffnen von der Festplatte

Oeffnest du die index.html per Doppelklick, sperrt der Browser bei
manchen Einstellungen den Zugriff auf Nachbarordner. Die Seite erscheint,
die Downloads funktionieren dort aber nicht immer. Auf der
veroeffentlichten Seite laeuft alles.
