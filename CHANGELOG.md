# Änderungsprotokoll

## 1.4 — 02.11.2026

- **+5 / −0**, neuer Stand **62 eindeutig belegte deutsche Einzelnummern**. Neue Regeln: `+4915510453140` (mittel-hoch: Gewinnspiel-/KI-Anrufe), `+4915510465755` (mittel-hoch: Serien-/Ping-/Gewinnspielanrufe), `+4921130194060` (hoch: Serien-/Spam-Anrufe), `+4921130194065` und `+4930330755669` (hoch: Verdacht auf Gewinnspiel-/Lottoabo-Anrufe). Das sind Risikoeinschätzungen aus Meldungen, keine Feststellung einer Straftat.
- Für jede neue Einzelnummer am 02.11.2026 eine konkrete PhoneBlock- und eine konkrete Clever-Dialer-Einzelseite gelesen. Beide URLs, die jeweils ausgewiesenen Meldedaten, Quellenwerte und wichtige Cache-/Zählergrenzen stehen in `quellen.csv`. PhoneBlock-Sperrstimmen sind keine nachgewiesenen unabhängigen Beschwerden. Einzelnummern-Stimmen und Block-Stimmen wurden getrennt erfasst, Anbieter-Scores nicht gleichgesetzt.
- Maßnahmenliste der Bundesnetzagentur für die letzten sechs Monate am 02.11.2026 eingesehen: unter den fünf konkreten Nummern kein Treffer in der angezeigten Tabelle, deren jüngster sichtbarer Bescheid vom 07.10.2026 stammt. Kein umfassender amtlicher Negativnachweis. Abschaltungsmaßnahmen und reine SMS-/Fax-/Messenger-Fälle nicht als neue Anrufsperren übernommen. Clever-Dialer-Archiv zeigte als letzten Monatsbericht weiterhin August 2026 (Veröffentlichung 01.09.2026).
- **Offene neue Prüffälle, keine zusätzlichen Sperren:** `+4921130194058` (Clever Dialer meldet störende Anrufe, PhoneBlock zeigt auch eine Legitimitätswertung) und `+4930499189816` (wiederholte, aber teils als reguläre Meinungsforschung beschriebene Anrufe). Keine Übernahme benachbarter Rufnummern allein aus Blockhäufungen.
- Zwei ältere schwache bzw. widersprüchliche Prüffälle (`+4915510656326`, `+49695095438980`) sowie Community-Widersprüche (`+4915888361621`, `+4946190279862`) stichprobenartig nachgelesen. Teilweise lagen im Web-Lesedienst ältere Cachefassungen vor. Weder eine nachweisliche Fehlzuordnung noch eine gesicherte Abschaltung belegt. Die 57 Bestandsregeln, ihre alten Prüfdaten und die bereits markierten offenen Qualitätsfälle bleiben deshalb unverändert; die Stichprobe ist keine erneute vollständige Verifikation.
- XML-/CSV-Einzelnummernabgleich, E.164-Eindeutigkeit, XML-Dict-Struktur und Risikodokumentation vor Veröffentlichung geprüft. Keine Wildcards, keine Tellows-Daten, keine Zusatzkosten. GitHub-Veröffentlichung ist **keine bestätigte automatische iPhone-Übernahme**; entfernte Regeln müssen auf bereits importierten Geräten separat geprüft werden.

## 1.3 — 26.10.2026

- Alle **57 deutschen Bestandsnummern** anhand tatsächlich gelesener Einzelseiten von PhoneBlock (28), Clever Dialer (9) und Wer hat mich angerufen / Spam-Barometer (20) geprüft. Die zuvor 50 fehlenden Einzel-URLs ergänzt. CSV um Quellen-URL, Prüfdatum, Meldedatum-Hinweis und Prüfstatus erweitert.
- Werte aus den gelesenen Seitenständen dokumentiert, inklusive Cachegrenzen. Frühere als „Konfidenzwert“ bezeichnete PhoneBlock-Bestandszahlen präzisiert: Sperrstimmen und Prozent-Konfidenz sind unterschiedliche Größen. Blockwerte rechtfertigen keine Sperre ungemeldeter Nachbarnummern.
- **8** PhoneBlock-Einträge mit schwacher Evidenz, **3** Einträge mit widersprüchlichen Community-Signalen, **5** mit wenigen negativen Bewertungen und **4** mit offener Aktualität zur Nachprüfung markiert. Bei **14** weiteren Einträgen möglichen Blockeinfluss auf die Konfidenz gekennzeichnet. Alle 57 deutschen Regeln bleiben vorläufig aktiv; Prüfhinweise deaktivieren keine XML-Regel und sind keine Freigabe als bewiesener Spam.
- Die drei bereits in Version 1.2 markierten Rufnummern erneut geprüft. Ihre geringe PhoneBlock-Evidenz ist weiterhin sichtbar, kein belastbarer Nachweis einer Fehlklassifizierung. Im Zuge der vollständigen Quellenprüfung weitere Prüffälle erkannt.
- Persönliche US-Einzelsperre `+16465185265` aus öffentlicher XML und aktueller CSV entfernt: ein unerwünschter nicht angenommener Anruf ohne unabhängigen öffentlichen Spam-Beleg genügt nicht für die Community-Liste. Eine privat gewünschte Sperre kann bestehen bleiben. Die historische Dokumentation bleibt erhalten.
- Änderungen: **+0 / −1**, neuer Stand **57 deutsche Einzelnummern**. Keine Wildcards oder zusätzlichen Nummernblöcke, keine Tellows-Daten.
- Importanleitung um private Sicherung, Wiederholungsimport und Behandlung entfernter Regeln ergänzt. Diese Abläufe sind auf dem iPhone noch zu testen, automatische GitHub-Synchronisierung bleibt unbestätigt.
- Tellows-Dokumentation auf den belegten Projektstatus beschränkt, keine Lizenzfreigabe oder Kontaktaufnahme behauptet.
- Die vorhandene Wochenaufgabe wurde am 26.10.2026 wieder aktiviert und um strengere Quellen- und Erfolgskontrollen ergänzt. Der vorherige Laufstatus „fehlgeschlagen“ trotz veröffentlichter Version 1.2 bleibt ungeklärt. Aktivierung beweist keinen erfolgreichen Folgelauf.

## 1.2 — 26.10.2026

- Vier einzeln öffentlich belegte deutsche Rufnummern ergänzt: `+491632210807`, `+491637875622`, `+4917650642602` und `+4922376922894` (PhoneBlock-Einzelseiten, geprüft am 26.10.2026).
- Risikobewertung: Für `+491632210807`, `+491637875622` und `+4922376922894` besteht anhand mehrerer öffentlicher Meldungen ein **hoher Verdacht auf unerwünschte Gewinnspiel-/Lotto-Abo-Anrufe**, aber kein gerichtlich bestätigter Betrugsnachweis. `+4917650642602` wird ausdrücklich nur als **mittleres Belästigungsrisiko durch gemeldete Scherzanrufe** eingeordnet. Quellenlinks und Beschwerdedaten stehen jeweils in `quellen.csv`.
- Drei Bestandsnummern wegen geringer öffentlicher Evidenz **zur Nachprüfung markiert**, nicht gelöscht: `+4915510656326` (4 Stimmen/50 % Spam-Konfidenz), `+4921141747476` (4/53 %) und `+4989211290101` (4/50 %). Dies sind keine nachgewiesenen Fehlmeldungen.
- Aktuelle Bundesnetzagentur-Maßnahmenliste (letzte sechs Monate, geprüft 26.10.2026) auf die vier neuen Rufnummern kontrolliert: keine dort genannte Abschaltung gefunden. Die aufgeführten bereits abgeschalteten Nummern sowie reine SMS-/Fax-/Messenger-Fälle wurden nicht übernommen. Clever Dialers zuletzt veröffentlichter Monatsbericht (August 2026, veröffentlicht 01.09.2026) bietet keine zusätzlichen bislang fehlenden deutschen Top-10-Einzelnummern.
- Änderungen: **+4 / −0**. Listenstand: **58 einzelne Sperrregeln (57 deutsche Rufnummern, 1 gesondert gekennzeichnete US-Nutzermeldung)**. XML-Struktur und Abgleich mit `quellen.csv` geprüft. Keine Rufnummernblöcke und keine Übernahme von tellows-Daten.
- Die Veröffentlichung auf GitHub bewirkt **keine bestätigte automatische Synchronisierung** in Begone auf dem iPhone.

## 1.1 — 23.10.2026

- `+16465185265` als einzelne Sperrregel ergänzt: „Unerwünschter Kontakt – Nutzermeldung“.
- Grundlage: direkte Nutzermeldung und ausdrücklicher Wunsch, diesen Kontakt zu sperren. Identität und Anrufzweck nicht unabhängig bestätigt. Keine Einstufung als bestätigte Betrugsnummer oder Feststellung rechtswidriger Werbung.
- Nur die vollständige internationale Nummer, keine nationale Zusatzvariante und kein Rufnummernblock.
- Listenstand: 54 einzelne Rufnummern, davon 53 bisherige deutsche Einträge und eine ausdrücklich gemeldete US-Nummer. Die 53 bisherigen Regeln bleiben unverändert; ihre Quellen wurden mit dieser Ergänzung nicht erneut bewertet.
- Quellenübersicht und Beschreibung entsprechend ergänzt. Die Änderung auf GitHub bestätigt keine Übernahme auf ein iPhone.

## 1.0 — 22.10.2026

- Erste manuell zusammengestellte Community-Liste mit 53 einzeln gemeldeten deutschen Rufnummern.
- Dokumentation der Quellen und Hinweise auf mögliche Fehlmeldungen.
- Keine pauschalen Rufnummernblöcke.
- tellows als mögliche künftige Quelle vorgesehen; keine tellows-Daten übernommen.
