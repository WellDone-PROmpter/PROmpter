# PROmpter

**Ergebnis-Aufbereitung für den Roche LightCycler PRO** — ein kostenloses, vollständig **offline** laufendes Windows-Werkzeug.

## ⬇ Download

- **Download-Seite (empfohlen):** <https://welldone-prompter.github.io/PROmpter/> — ein Klick, immer die neueste `PROmpter_<Version>.exe`.
- **Alle Versionen & Änderungen:** [Releases](https://github.com/WellDone-PROmpter/PROmpter/releases)

Keine Installation nötig — die `.exe` einfach in einen festen Ordner legen und per Doppelklick starten (**keine Administratorrechte**).

> **Erster Start (SmartScreen):** Beim allerersten Start zeigt Windows evtl. *„Der Computer wurde durch Windows geschützt"* → **„Weitere Informationen" → „Trotzdem ausführen"**. Das ist normal (die App ist neu und nicht signiert) und erscheint nur einmal.

## 📖 Handbuch

- [Handbuch (Deutsch, PDF)](HANDBUCH.pdf)
- [Manual (English, PDF)](MANUAL_EN.pdf)

## Was macht PROmpter?

PROmpter **überwacht den Export-Ordner** des LightCycler PRO und bereitet die exportierten Läufe automatisch zu einem **PDF-Bericht** (Befund/Zusammenfassung inkl. Kurven) und einer **Excel-Tabelle** der Ergebnisse auf — danach wird die Originaldatei archiviert. Oberfläche und Handbuch in **Deutsch & Englisch**.

## 🧪 Schwester-App: WellDone!

Passend dazu — **vor** dem Lauf: [**WellDone!**](https://welldone-prompter.github.io/WellDone/) belegt die PCR-Platte und erzeugt das Pipettierschema + das LC-PRO-Setup. *(WellDone = Vorbereitung, PROmpter = Auswertung.)*

## ⚠️ Wichtiger Hinweis

PROmpter ist ein **Hilfswerkzeug, kein Medizinprodukt und nicht validiert**. Erzeugte Berichte **vor der Verwendung prüfen**. Es wird keine Haftung für Schäden oder fehlerhafte Ergebnisse übernommen.

## Kontakt

Feedback & Fehlerberichte: [well.done.pcr.setup@gmail.com](mailto:well.done.pcr.setup@gmail.com) · [Online-Formular](https://forms.gle/9QYvGAw1AXsfxYRk8)

## Lizenz / Weitergabe

Freie, private Weitergabe erwünscht; **kein Verkauf / kein kommerzieller Vertrieb**. PROmpter nutzt quelloffene Bibliotheken (PySide6/Qt — GNU LGPL v3; ReportLab — BSD; openpyxl — MIT; watchdog — Apache 2.0). „Roche" und „LightCycler" sind Marken der jeweiligen Inhaber; PROmpter ist ein **unabhängiges, privates Projekt**, **nicht** von Roche geprüft oder verantwortet.

---

*English — PROmpter is a free, fully **offline** Windows tool that watches the Roche LightCycler PRO export folder and turns exported runs into a **PDF report** and an **Excel table** of the results. Download from the [download page](https://welldone-prompter.github.io/PROmpter/). **Helper tool — not a medical device, not validated; check every report.** See the [English manual](MANUAL_EN.pdf). Sister app: [WellDone!](https://welldone-prompter.github.io/WellDone/) (plate setup before the run). An independent, private project, not reviewed or endorsed by Roche.*
