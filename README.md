# Aktien-Kompass – private Aktien-Mindmap

## Enthalten
- Installierbare PWA für Windows (Edge/Chrome) und Android (Chrome)
- Interaktive Mindmap mit Kategorien und Aktien
- Zeiträume 1 Tag, 1 Woche, 1 Monat, 1 Jahr, 5 Jahre und Gesamt
- CSV-/JSON-Kursimport, lokale Charts, Quellen-/Zeitstempelanzeige
- Aktienvergleich per Doppelklick
- Optionales, manuelles Depot
- Lokale Datensicherung und Wiederherstellung
- Keine Registrierung, kein Login, keine Broker-Verbindung, kein eigener Server

## Wichtiger Datenhinweis
Diese Version enthält absichtlich **keine automatische Kursabfrage**. Es gibt keine offiziell bestätigte, kostenlose und für die automatische Einbindung in diese App freigegebene Schnittstelle, die alle gewünschten Handelsplätze und die benötigten historischen Daten abdeckt. Insbesondere erlaubt die kostenlose gettex-Delayed-Data-Bereitstellung die private Nutzung durch eine natürliche Person und untersagt die Weitergabe an Dritte. Bitte beachte die jeweils aktuellen Nutzungsbedingungen deiner Datenquelle.

Importiere ausschließlich Kursdateien, die du rechtmäßig für deine private lokale Nutzung verwenden darfst. Die App liest keine Webseiten aus und überträgt importierte Daten nicht an einen Server. CSV-Spalten:
`symbol,date,price,venue,currency,source`
- `symbol`: muss exakt der WKN/ISIN-Kennung der Aktie in der Mindmap entsprechen
- `date`: ISO-Datum oder ISO-Zeit
- `price`: positiver Zahlenwert
- `venue`: Tradegate, gettex, Stuttgart, Lang & Schwarz Exchange, Baader Trading oder Sonstige / Import
- `currency` und `source`: optional

## Installation
Eine PWA benötigt HTTPS oder localhost:
1. ZIP entpacken und den Ordner auf einem HTTPS-fähigen Webspace bereitstellen, auf den nur du Zugriff hast, oder lokal über einen lokalen Webserver öffnen.
2. Windows: in Edge/Chrome öffnen → Menü → Apps → Diese Website als App installieren.
3. Android: in Chrome öffnen → Menü → App installieren bzw. Zum Startbildschirm hinzufügen.

Ein ZIP allein ist noch keine installierte App. Für eine private, geräteübergreifende Synchronisierung wäre später ein eigener geschützter Server nötig; diese Version speichert alles nur lokal je Gerät.

## Datenschutz und Grenzen
- Daten werden im Browser-LocalStorage gespeichert.
- Kein Konto und keine Cloud-Synchronisierung.
- Jeder mit Zugriff auf dasselbe Browserprofil/Gerät kann möglicherweise die lokalen Daten sehen.
- Die App ist keine Anlageberatung. Datenimporte können fehlerhaft oder unvollständig sein.
