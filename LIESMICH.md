# Roseggerstrasse 9, Kirchheim unter Teck, Wohnung Nr. 3 (1. OG links)

## Was in diesem Ordner liegt

    index.html          das Expose
    bilder/             14 Bilddateien, vom Expose eingebunden
    unterlagen/         18 PDF, ueber die Downloadkarten verlinkt

Alle drei muessen beieinander bleiben. Fehlt "bilder", zeigt die Seite
keine Fotos. Fehlt "unterlagen", laufen die Downloads ins Leere.

Zusaetzlich liegt eine Stufe hoeher die Datei
`Vorschau_Roseggerstrasse-9_Wohnung-3.html`. Darin sind alle Bilder
eingebettet, sie laesst sich also per Doppelklick oeffnen und
weitergeben. Die Downloadkarten funktionieren dort nicht, weil der
Ordner "unterlagen" fehlt. Die Vorschau ist nur zum Gegenlesen,
veroeffentlicht wird der Ordner.

Aufgebaut ist das Expose auf der freigegebenen Fassung der Wohnung
Nr. 2 (EG rechts). Struktur, Gestaltung, Rechner und rechtliche
Hinweise sind unveraendert, geaendert wurden die objektbezogenen
Zahlen und Texte.

## VOR DER VEROEFFENTLICHUNG UNBEDINGT ERLEDIGEN

1. **Foto vom Kinderzimmer fehlt.** Der Bildstreifen zeigt die
   Hausansicht, fuenf Raeume und den Garten. Vom dritten Zimmer
   (KINDER, 10,69 m2) gibt es keine Aufnahme. Der Platz dafuer ist
   freigehalten: Kommt eine dazu, als `bilder/07_kinderzimmer.jpg`
   ablegen und im Kapitel 02 eine weitere Zeile in den Bildstreifen
   einfuegen, hinter `06_schlafzimmer.jpg`, das ist die letzte Zeile
   des Streifens:

       <figure><img src="bilder/07_kinderzimmer.jpg" alt="Drittes Zimmer der Wohnung Nr. 3" decoding="async"></figure>

   Umbenennen muss man dafuer nichts.

2. **Adresse der veroeffentlichten Seite eintragen.** In der
   index.html steht im Kapitel Finanzierung genau eine Zeile:

       var EXPOSE_URL = "";

   Dort die Adresse der GitHub-Pages-Seite eintragen. Bleibt das Feld
   leer, steht in der vorbereiteten Mail an die Moeglichmacher ein
   Platzhalter statt des Links.

3. **Kueche pruefen.** Auf der Aufnahme ist eine eingebaute Kueche
   mit Unter- und Oberschraenken, Arbeitsplatte, Backofen und
   Dunstabzug zu sehen. Ob sie zum Verkauf gehoert oder dem Mieter,
   geht aus den Unterlagen nicht hervor, im Mietvertrag von 1998 ist
   nur "Kueche mit Herd" angekreuzt. Das Expose behauptet deshalb
   keine Einbaukueche, sondern nennt nur "Kueche als eigener Raum mit
   Fenster". Gehoert sie mit dazu, laesst sich das in Kapitel 02 unter
   "Ausstattung und Zustand" ergaenzen, das ist ein echtes
   Verkaufsargument.

4. **Entfernungen im Kapitel Lage pruefen.** Die Geh- und Fahrzeiten
   sind aus dem Expose der Nr. 2 uebernommen und gerundet.

5. **Kostenrahmen Modernisierung.** Im Kapitel 07 steht bewusst kein
   Kostenrahmen, weil fuer diese Einheit kein Handwerkerangebot
   vorliegt.

6. **Herleitung der Kaufpreisaufteilung vervollstaendigen.** Die Datei
   geht nicht in den oeffentlichen Ordner, muss vor der Beurkundung
   aber gefuellt werden. Offen sind: "erstes Obergeschoss [bitte
   ergaenzen: links oder rechts]" ist links, der Kaufpreis fehlt
   (205.000 EUR), Gebaeudeanteil und Prozentwerte sind offen
   (161.053 EUR und 78,56 Prozent bezogen auf den Kaufpreis, im Expose
   wird mit 175.403 EUR und 79,96 Prozent bezogen auf die
   Gesamtinvestition gerechnet), und der Absatz zur Vermietungs-
   situation ist leer. Fuer den letzten Punkt: Nettokaltmiete 522 EUR,
   Mietverhaeltnis seit 01.06.1998, Miete deutlich unter der
   ortsueblichen Vergleichsmiete, dadurch eingeschraenkte Nutzbarkeit.

## Zahlengrundlage im Expose

Alle Werte stammen aus "1. og Links.xlsx", Blatt Kalkulation.

    Kaufpreis                    205.000 EUR
    Kaufpreis je m2                3.003 EUR
    Erwerbsnebenkosten 7 %        14.350 EUR
    Gesamtinvestition            219.350 EUR
    Grund und Boden               43.947 EUR   61,8969 m2 x 710 EUR
    Abschreibungsbasis           175.403 EUR   = 79,96 % der Gesamtinvestition
    Restnutzungsdauer            19 Jahre      Gutachten BeMa vom 09.08.2026,
                                               Stichtag 08.06.2026, AZ-R-2026-1153
    Abschreibung im Jahr           9.232 EUR   = 5,26 %
    Wohnflaeche                    68,27 m2    WoFlV, Aufmass 08.06.2026
    Miteigentumsanteil           158,71 / 1.000
    Nettokaltmiete                   522 EUR   = 7,65 EUR/m2
    Mietverhaeltnis              seit 01.06.1998
    Hausgeld gesamt                  224 EUR   HG-Vorschuss Wirtschaftsplan 2026
    Instandhaltungsruecklage       61,42 EUR   Rucklagenzufuehrung 2026
    Mietsubvention                 9.910 EUR   siehe Staffelung unten

Die Mietsubvention ist mit **9.910 EUR** angesetzt, wie in Zelle M44
der Kalkulation:

    Dezember 2026       190 EUR                 190 EUR
    2027 bis 2029       140 EUR je Monat      5.040 EUR
    2030 bis 2032        90 EUR je Monat      3.240 EUR
    2033 bis 2035        40 EUR je Monat      1.440 EUR
    Summe                                     9.910 EUR

Im Rechenmodell der index.html steht dafuer

    sub:[140, 140, 140, 90, 90, 90, 40, 40, 40, 0]

Das sind die Monatsbetraege fuer die Jahre 1 bis 10 nach dem Kauf, also
2027 bis 2036. Die 190 EUR fuer den Dezember 2026 liegen davor und sind
im Rechner nicht enthalten, weil er in ganzen Jahren ab dem Kauf rechnet.

## Bewusste Abweichungen von der Kalkulation

**Mieterhoehung.** Der Rechner im Expose setzt die erste Mieterhoehung
erst nach drei Jahren an, die Kalkulation dagegen schon 2027. Das
Expose rechnet damit vorsichtiger. Angeglichen wird es, indem im
Rechenmodell die Zeile

    var stufen=Math.floor((j-1)/3);

auf

    var stufen=Math.floor(j/3)+1;

geaendert wird. Dann steigen alle ausgewiesenen Ergebnisse. So war es
schon bei der Nr. 2.

**Nicht umlegbares Hausgeld.** Angesetzt sind 60 EUR im Monat, wie in
der Kalkulation. Der Hinweis auf den Wert aus dem Wirtschaftsplan
steht auf Wunsch nicht im Expose, weil dieser Punkt noch geklaert wird.

**Instandhaltungsruecklage.** Im Rechenmodell mit 62 EUR gerundet, in
der Faktenliste mit dem tatsaechlichen Wert 61,42 EUR ausgewiesen.

**Angesetzte Marktmiete.** 1.030 EUR. Hergeleitet aus der
modernisierten Nr. 1 im Erdgeschoss links, dort 1.000 EUR auf
63,90 m2, also 15,65 EUR/m2. Auf 68,27 m2 uebertragen waeren das
1.068 EUR, angesetzt wird bewusst darunter.

## Zu den Bildern

Das Titelbild ganz oben (`02_hausansicht_hero.jpg`) ist die
Strassenansicht aus dem Ordner der Nr. 2, es ist dasselbe Haus.

Im Bildstreifen steht an erster Stelle die Aussenansicht mit der gelben
Markierung (`03_hausansicht_markiert.jpg`). Sie zeigt, welche Fenster
zur Wohnung Nr. 3 gehoeren.

Die Gartenaufnahme ist aus dem Fotoordner der Nr. 3.

Reihenfolge im Bildstreifen: Garten, Flur, Bad, WC, Hausansicht,
Wohnen und Essen, Kueche, Schlafzimmer. Auf der ersten Ansicht liegen
damit Garten, Flur, Bad und WC, der Rest kommt beim Wischen. Die
Dateinamen sind nach der urspruenglichen Reihenfolge nummeriert und
stimmen mit der Anzeigereihenfolge bewusst nicht ueberein. `07` ist
fuer das Kinderzimmer freigehalten.

Der Grundriss `bilder/11_grundriss_we3.png` ist die schematische
Darstellung mit Moeblierungsvorschlag aus dem Fotoordner. Der blaue
Pfeil zeigt den Wohnungszugang. Die Bildunterschrift weist ihn als
schematisch und ohne Massstab aus und verweist fuer die
massgeblichen Angaben auf den Aufteilungsplan und die
Wohnflaechenberechnung in den Unterlagen.

Zu beachten: Im Treppenhaus stehen auf dieser Zeichnung noch
"Hauseingang" und "Zugang Keller". Beides gehoert zum Erdgeschoss und
trifft im ersten Obergeschoss nicht zu. Falls das stoert, laesst sich
eine bereinigte Fassung einsetzen, gleicher Dateiname, sonst ist
nichts zu aendern.

Die fuenf Innenaufnahmen sind die KI-aufbereiteten Fassungen aus dem
Fotoordner. Der kurze Hinweis dazu steht unter dem Bildstreifen,
ausfuehrlich steht er in den rechtlichen Hinweisen unter "Einsatz von
KI".

Kapitel 07 beginnt mit einem zweiten Bildstreifen, vier unbearbeitete
Aufnahmen der modernisierten Wohnung Nr. 1 im Erdgeschoss links, also
der Einheit direkt unter dieser Wohnung. Er steht bewusst vor dem Text,
damit man den Zustand zuerst sieht. Dateien
`20_modernisierung_wohnen.jpg` bis `23_modernisierung_flur.jpg`. Die
Bildunterschrift stellt klar, dass es sich um eine andere Einheit
handelt und dies keine Leistungszusage ist.

Die Bildstreifen sind waagerecht wischbar. Am Rechner
liegen vier Bilder nebeneinander und es gibt Pfeile am Rand, auf dem
Tablet zwei, auf dem Telefon eines. Die Punkte darunter zeigen, wo man
sich befindet. Ein Klick auf ein Bild oeffnet es weiterhin gross in der
Lightbox. Im Ausdruck wird daraus wieder ein Raster mit zwei Spalten,
dafuer sorgt die Druckregel in der index.html.

## Zu den Unterlagen

Der Ordner entspricht dem der Nr. 2, das sind durchweg Unterlagen zum
Gemeinschaftseigentum und damit fuer alle Einheiten dieselben. Ersetzt
wurde nur `04_Modernisierungsuebersicht.pdf` durch die Fassung dieser
Einheit, sie fuehrt unten "Wohnung 1. OG links" auf.

Die Erschliessungsbeitragsauskunft lag im Paket der Nr. 3 nicht bei
und stammt deshalb aus dem Paket der Nr. 2.

Nicht im Ordner "unterlagen" liegen Grundbuchauszug,
Restnutzungsdauergutachten, Herleitung der Kaufpreisaufteilung und der
Mietvertrag. Sie enthalten personenbezogene Daten. Auf GitHub Pages
ist jede Datei im Repository oeffentlich abrufbar, auch wenn sie auf
der Seite nicht verlinkt ist. Im Expose steht deshalb, dass diese
Unterlagen bei ernsthaftem Kaufinteresse nachgereicht werden.

Hinweis zur Teilungserklaerung, die im Ordner liegt: Sie enthaelt in
Abteilung III die Grundschulden des Verkaeufers. Das war bei der Nr. 2
genauso. Falls das nicht gewuenscht ist, die Datei
`01_Teilungserklaerung.pdf` loeschen und den ersten Eintrag in der
Liste `DOKS` in der index.html entfernen.

## Hochladen

Ein eigenes Repository fuer diese Wohnung anlegen. Dann auf
"Add file", danach "Upload files", und in das Fenster alles drei
zusammen ziehen:

    index.html
    bilder            (der ganze Ordner)
    unterlagen        (der ganze Ordner)

Wichtig: nicht den Ordner "Roseggerstrasse-9-1OG-links" hochladen,
sondern seinen Inhalt. Die index.html muss im Repository ganz oben
liegen.

## Pages einschalten

Settings, dann Pages. Bei Source "Deploy from a branch" waehlen,
Branch `main`, Ordner `/ (root)`. Speichern. Der erste Aufbau dauert
ein bis zwei Minuten.

## Falls ein Ordner anders heissen soll

In der index.html steht im Skript genau eine Zeile:

    var DOKBASE='unterlagen/';

Nur diese aendern. Der Schraegstrich am Ende muss bleiben.
Der Bildordner ist in den Bildpfaden hinterlegt und heisst "bilder".

## Hinweis zum Oeffnen von der Festplatte

Oeffnest du die index.html per Doppelklick, sperrt der Browser bei
manchen Einstellungen den Zugriff auf Nachbarordner. Die Seite
erscheint, die Downloads funktionieren dort aber nicht immer. Auf der
veroeffentlichten Seite laeuft alles.
