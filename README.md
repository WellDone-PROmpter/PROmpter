# PROmpter

**Ergebnis-Übersicht – kompatibel mit LightCycler® PRO** — ein kostenloses, vollständig **offline** laufendes Windows-Werkzeug.

## ⬇ Download

- **Download-Seite (empfohlen):** <https://welldone-prompter.github.io/PROmpter/> — ein Klick, immer die neueste `PROmpter_<Version>.exe`.
- **Alle Versionen & Änderungen:** [Releases](https://github.com/WellDone-PROmpter/PROmpter/releases)

Keine Installation nötig — die `.exe` einfach in einen festen Ordner legen und per Doppelklick starten (**keine Administratorrechte**).

> **Erster Start (SmartScreen):** Beim allerersten Start zeigt Windows evtl. *„Der Computer wurde durch Windows geschützt"* → **„Weitere Informationen" → „Trotzdem ausführen"**. Das ist normal (die App ist neu und nicht signiert) und erscheint nur einmal.

## 📖 Handbuch

- [Handbuch (Deutsch, PDF)](HANDBUCH.pdf)
- [Manual (English, PDF)](MANUAL_EN.pdf)

## Was macht PROmpter?

PROmpter **überwacht den Export-Ordner** des LightCycler PRO und bereitet die exportierten Läufe automatisch zu einer formatierten **PDF-Übersicht** (Zusammenfassung inkl. Kurven) und einer **Excel-Tabelle** der Ergebnisse auf — danach wird die Originaldatei archiviert. Oberfläche und Handbuch in **Deutsch & Englisch**.

## 🧪 Schwester-App: WellDone!

Passend dazu — **vor** dem Lauf: [**WellDone!**](https://welldone-prompter.github.io/WellDone/) belegt die PCR-Platte und erzeugt das Pipettierschema + das LC-PRO-Setup. *(WellDone = Vorbereitung, PROmpter = Ergebnis-Übersicht.)*

## ⚠️ Wichtiger Hinweis

PROmpter ist ein kostenloses, **nicht validiertes Hilfswerkzeug**. Es übernimmt Cq-Werte, Geräte-Calls und Kurven unverändert aus dem LightCycler-PRO-Export und fasst die Calls je Probe nach einer festen Regel übersichtlich zusammen; es berechnet keine Werte neu und setzt keine eigenen Grenzwerte. **Maßgeblich bleiben die Ergebnisse in der Gerätesoftware und die Befundfreigabe durch das Labor.** PROmpter wird **nicht als Medizinprodukt oder In-vitro-Diagnostikum in Verkehr gebracht**, trägt keine CE-Kennzeichnung und wurde regulatorisch nicht formal geprüft. Vor dem Routineeinsatz ist es im Qualitätsmanagement des Labors zu prüfen und freizugeben. Die Haftung richtet sich nach den gesetzlichen Vorschriften.

## Kontakt

Feedback & Fehlerberichte: [well.done.pcr.setup@gmail.com](mailto:well.done.pcr.setup@gmail.com) · [Online-Formular](https://forms.gle/9QYvGAw1AXsfxYRk8)

## Lizenz / Weitergabe

Freie, private Weitergabe erwünscht; **kein Verkauf / kein kommerzieller Vertrieb**. PROmpter nutzt quelloffene Bibliotheken (PySide6/Qt — GNU LGPL v3; ReportLab — BSD; openpyxl — MIT; watchdog — Apache 2.0). „Roche" und „LightCycler" sind Marken der jeweiligen Inhaber; PROmpter ist ein **unabhängiges, privates Projekt**, **nicht** von Roche geprüft oder verantwortet.

---

*English — PROmpter is a free, fully **offline** Windows tool that watches the LightCycler® PRO export folder and turns exported runs into a formatted **PDF overview** and an **Excel table** of the results. Download from the [download page](https://welldone-prompter.github.io/PROmpter/). **Non-validated helper tool — it takes Cq values, instrument calls and curves unchanged and summarises the calls per sample by a fixed rule; the instrument software and the laboratory's result release remain authoritative. Not placed on the market as a medical device/IVD, no CE marking, no formal regulatory assessment; release it in your lab's QM before routine use. Liability is governed by the statutory provisions.** See the [English manual](MANUAL_EN.pdf). Sister app: [WellDone!](https://welldone-prompter.github.io/WellDone/) (plate setup before the run). An independent, private project, not reviewed or endorsed by Roche.*
