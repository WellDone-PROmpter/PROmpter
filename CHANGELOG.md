# Versionsverlauf — PROmpter

Neueste Version oben. Aktuelle Releases & Download: https://welldone-prompter.github.io/PROmpter/

**Version 1.9** (Juni 2026)
- **Schwester-App verlinkt:** Der **„❓"-Dialog (Über / Hilfe)** verweist jetzt direkt auf **WellDone!** – die Schwester-App für **Plattenbelegung & PCR-Setup vor dem Lauf**. *WellDone! = Vorbereitung, PROmpter = Auswertung.*
- **Handbuch aktualisiert:** Ein überflüssiger Abschnitt wurde entfernt und ein Beispiel anonymisiert (neutrale Beispiel-Einrichtung statt einer realen).

**Version 1.8** (Juni 2026)
- **Englische Sprachvariante:** PROmpter spricht jetzt **Deutsch und Englisch** — umschaltbar in den **Einstellungen** (*Dateimanagement → „Sprache / Language"*, Standard Deutsch). Die Umstellung betrifft Oberfläche, PDF-Bericht, Excel und alle Meldungen und greift nach einem Neustart; im englischen Modus werden Zahlen mit **Punkt** statt Komma geschrieben. **Geräte- und Probendaten bleiben in beiden Sprachen unverändert** (PROmpter rechnet und interpretiert nichts neu). Das Handbuch liegt jetzt auf **Deutsch und Englisch** vor und öffnet automatisch in der eingestellten Sprache.

**Version 1.7** (Juni 2026)
- **Ordner-Überwachung auf Netzlaufwerken:** Die Automatik fragt den Überwachungsordner jetzt im festen Takt aktiv ab (*Polling*), statt auf Betriebssystem-Ereignisse zu warten. Dadurch werden neue Exporte auch auf **Netz-/SMB-Freigaben** zuverlässig erkannt (dort blieben die nativen Datei-Ereignisse aus — vor allem, wenn ein anderer Rechner schreibt). Das Abfrageintervall ist in den **Einstellungen** (*Dateimanagement → „Ordner abfragen alle … Sek."*, Standard 5 s) einstellbar; abgefragt wird nur das Verzeichnis, nicht die Dateiinhalte (minimale Last).
- **Excel — kritische Flags im Klartext:** Neue, abwählbare Spalte **„Kritische Flags"** im Blatt *Ergebnisse* (neben „Flags", das weiterhin **alle** Flags zeigt) und neue Spalte **„Kritische Flags"** am Ende der **Zusammenfassung** — wie in der PDF-Übersicht nur die schwer gewichteten Flags.
- **Zusammenfassung wie die PDF-Übersicht:** In der Kreuztabelle bedeutet eine **leere Zelle „nicht getestet"** und **„–" „getestet, aber negativ"** (vorher beide leer und damit nicht unterscheidbar).
- **Block „LCAPs & Assays" übersichtlicher:** je Target jetzt **„Name (Farbstoff Anregung/Emission)"**, z. B. „Parechovirus (FAM 494/523)" — Farbstoff und Kanäle in *einer* Klammer. Zusätzlich wird jetzt auch die **interne Kontrolle** aufgeführt — hinten angehängt und mit **„IC:"** gekennzeichnet (z. B. „…, IC: Internal control (Cy5 657/675)").
- **Excel — Kanal & Farbstoff:** Die Spalte **„Kanal"** zeigt jetzt zusätzlich die Anregungs-/Emissions-Wellenlängen (**„22 (494/523)"**), und es gibt eine neue, abwählbare Spalte **„Farbstoff"** (z. B. FAM, R6G, Cy5).
- **Dateinamen-Vorschau:** Die Vorschau im Einstellungen-Dialog zeigt den Baustein **`{Plattenname}`** jetzt mit Beispielwert (er wurde in der echten Datei immer korrekt eingesetzt, blieb aber in der Vorschau leer).

**Version 1.6** (Juni 2026)
- **Automatischer Druck:** Der PDF-Bericht kann nach der Erstellung direkt gedruckt werden — mit **Druckerauswahl** (Standard- oder bestimmter Drucker) und **Anzahl Kopien**. Einstellbar im Reiter *Dateimanagement → Drucken*. PROmpter druckt das PDF **selbst** (unabhängig vom installierten PDF-Programm).
- **Neuer Kopfblock** im PDF: **Plattenname** (aus der Plattenbelegung), **PCR-Profil**, **Reaktionsvolumen**, **Zyklen**, **Gerät inkl. Block** (z. B. „96er Block"), **Plate-ID**, **Block-Seriennr.** und **Instrument-Software**. Die Untertitel-Zeile zeigt **Plattenname - Lauf-ID**.
- **Plattenname** als neuer Dateinamen-Baustein **`{Plattenname}`** und als (erste) **Excel-Spalte**.
- Im Block „LCAPs & Assays" steht je Target jetzt zusätzlich der **Farbstoff** (z. B. „FAM"), nicht nur die Anregungs-/Emissions-Kanäle.
- **„Assay" → „LCAP" klargestellt:** Die Excel-Spalte heißt jetzt **„LCAP"** und zeigt **je Probe deren eigenen LCAP** (vorher überall der erste LCAP des Laufs). Der Dateinamen-Baustein `{Assay}` heißt jetzt **`{LCAP}`** (bzw. `{LCAPVersion}`); die alten Namen funktionieren weiter.
- **Grund für „ungültig" sichtbar:** Bei ungültigen Proben werden die **kritischen Geräte-Flags im Klartext** angezeigt — in der **Ergebnis-Übersicht** (Spalte „Targets", z. B. „Validierung fehlgeschlagen: ungültige interne Kontrolle; Ungültiges Ergebnis") und in **„Amplifikationskurven je Target"** als **nummerierte Fußnote** direkt unter der Zuordnungstabelle. (Nur kritische Flags; reine Info-Flags werden nicht aufgeführt.)
- **384er-Platten:** Die **Plattenübersicht erkennt das Format automatisch** (96 = 8×12, 384 = 16×24) und zeichnet das passende Raster — im Hochformat. Die übrigen Auswertungen (Übersicht, Cq, Excel, Kurven) waren ohnehin schon formatunabhängig.

**Version 1.5** (Juni 2026)
- Diese Versionsübersicht ins Handbuch aufgenommen.

**Version 1.4**
- Die Tabelle „Einzelwerte — Cq je Target" wird bei **vielen Targets automatisch im Querformat** dargestellt (sonst Hochformat).
- **Leere Zelle = Target nicht im Panel** der Probe; **„–" = getestet, aber negativ** (kein Cq).

**Version 1.3**
- **Kanäle (Anregung/Emission)** hinter jedem Target, z. B. (494/523).
- Besser unterscheidbare, **farbfehlsichtigkeits-taugliche Kurvenfarben**.
- Abwechselnd hinterlegte Tabellenzeilen für bessere Lesbarkeit.
- Target-Reihenfolge **nach LCAP gruppiert**.
- In „Amplifikationskurven je Target" neue Spalte **„Ergebnis"** (reaktiv / ungültig / Kontrolle).
- Excel: reaktive **und ungültige** Ergebnisse fett; Spalte „Typ" in der Zusammenfassung entfernt.

**Version 1.2**
- Unterstützung für Läufe mit **mehreren LCAPs (Assays)**: alle LCAPs samt Targets im Kopf, jedes Target als eigene Spalte.
- Neue Ergebnis-Kategorie **„ungültig"** (deutlich markiert).
- Korrektur: negative Ergebnisse werden zuverlässig als **„nicht reaktiv"** erkannt.

**Version 1.1**
- Fehlerbehebung bei der PDF-Erstellung mit sehr vielen reaktiven Proben auf einem Target.

**Version 1.0**
- Erste Version: automatische Aufbereitung der LightCycler-PRO-Kundendaten zu **PDF-Bericht** und **Excel-Tabelle**, inkl. Amplifikationskurven, konfigurierbarer Berichte und Update-Prüfung.

---
