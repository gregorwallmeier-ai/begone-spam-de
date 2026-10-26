# Begone-Spamsperrliste Deutschland (Community-Projekt)

**Stand: 26.10.2026 · Version 1.3 · Experimentelle Community-Zusammenstellung**

Kostenlose redaktionelle Auswahl öffentlich gemeldeter deutscher Rufnummern für [Begone](https://begone.app/) auf dem iPhone. Gemeldeter Spam ist keine bewiesene Straftat. Angezeigte Nummern können gefälscht oder später neu vergeben werden.

## Dateien und aktueller Stand

- [Sperrliste](begone-de-gemeldete-nummern.xml): **57 deutsche Einzelnummern**, keine Wildcards, Vorwahl- oder Nummernblocksperren.
- [Quellenübersicht](quellen.csv): für jede der 57 Nummern eine tatsächlich gelesene Einzelquelle und das Prüfdatum 26.10.2026, dazu Meldedatum-Hinweis und Prüfstatus.
- [Änderungen](CHANGELOG.md): zuletzt **+0 / −1** gegenüber Version 1.2.
- [Tellows-Status](TELLOWS_INTEGRATION.md): nicht integriert, keine Übernahme von Scorelisten.

Die US-Nummer aus Version 1.1/1.2 wurde aus der öffentlichen XML und der aktuellen Quellenübersicht entfernt, weil nur eine persönliche Unerwünschtheit ohne unabhängigen öffentlichen Spam-Beleg vorlag. Eine persönlich gewünschte Sperre kann privat auf dem eigenen Telefon bestehen bleiben. Der Vorgang bleibt im Changelog nachvollziehbar.

## Quellen lesen und richtig einordnen

CSV-Trennzeichen ist das Semikolon, Zeichensatz UTF-8 mit BOM. Die ersten drei Spalten bleiben Rufnummer, Quelle und Quellenhinweis. Hinzu kommen konkrete Quellen-URL, Prüfdatum, Meldedatum-Hinweis und Prüfstatus.

Quellenkürzel:
- **PB**: [PhoneBlock](https://phoneblock.net/). Sperrstimmen sind keine Anzahl unabhängiger Beschwerden. Die angezeigte Konfidenz kann auch zusammen mit Block-Sperrstimmen erscheinen. Blockwerte rechtfertigen keine Übernahme ungemeldeter Nachbarnummern.
- **CD**: Clever Dialer, [Monatsbericht August 2026](https://www.cleverdialer.app/telefonspam-check/2026/09/01/clever-dialer-telefonspam-check-die-nummern-fuer-august-2026/) und verlinkte Einzelseiten. Sterne, Bewertungen, gemeldete Anrufe und Blockierungen sind unterschiedliche Größen.
- **SB**: [Spam-Barometer / Wer hat mich angerufen?](https://wer-hat-mich-angerufen.de/spam-barometer) und Einzelseiten. Bewertungen und Erfahrungsberichte dürfen nicht ungeprüft als unabhängige Fälle addiert werden.

**Prüfdatum bedeutet: Die verlinkte Quelle wurde an diesem Tag gelesen.** Der Web-Lesedienst kann zwischengespeicherte Seiten liefern. Cachehinweise stehen in der CSV. Die Werte sind keine Live-Messung und können zwischen Rangliste und Einzelseite abweichen. Ein leerer oder unklarer letzter Meldetermin wird nicht aus Suchanfragen oder Abrufdatum abgeleitet.

## Offene Qualitätsprüfung

Alle 57 deutschen Regeln wurden als Bestandsregeln beibehalten. Das ist keine erneute Freigabe jeder Nummer als sicherer Spamfall:
- **8** Einträge mit geringer PhoneBlock-Evidenz sind zur Nachprüfung markiert. Darunter die drei bereits in Version 1.2 markierten Nummern.
- **3** Einträge haben widersprüchliche Community-Signale, darunter als seriös eingeordnete Bewertungen oder Berichte.
- **5** weitere Einträge haben nur wenige negative Bewertungen in der gelesenen Einzelquelle.
- **4** Clever-Dialer-Einträge benötigen eine Aktualitätsprüfung, weil die gelesene Einzelseite null Anrufe im dortigen 30-Tage-Fenster ausweist. Das beweist weder Abschaltung noch Unbedenklichkeit.
- Bei **14** weiteren PhoneBlock-Einträgen ist ein möglicher Einfluss von Blockwerten auf die Konfidenz zu beachten. Es existieren Einzelnummern-Sperrstimmen; keine Nachbarnummern wurden ergänzt.

Diese Kategorien sind redaktionelle Prüfhilfen, keine einheitliche Risikoskala verschiedener Anbieter. **Prüfhinweise in der CSV deaktivieren keine XML-Regel.** Wer Fehlblockaden besonders vermeiden möchte, sollte die betroffene Einzelsperre vorläufig individuell ausnehmen.

## Regeln für die weitere Pflege

1. Neue Regeln nur für vollständig belegte einzelne deutsche Rufnummern mit konkreter Quellen-URL, Prüfdatum, Meldedatum soweit verfügbar und nachvollziehbarem unerwünschtem Anrufgrund aufnehmen. Ein bloß verpasster Anruf, Suchhäufigkeit, eine Nachbarnummer oder ein Blockscore reichen nicht.
2. Bei schwacher oder widersprüchlicher Evidenz zusätzliche unabhängige Belege suchen. Bestehende unklare Regeln als Prüffall dokumentieren und nicht als neue gesicherte Fälle darstellen.
3. Nachweislich falsche Zuordnungen oder unpassende Regeln korrigieren. Amtlich abgeschaltete Nummern sowie reine SMS-/Fax-/Messenger-Fälle nicht blind übernehmen. Für Maßnahmen die [Bundesnetzagentur](https://www.bundesnetzagentur.de/) als Primärquelle nutzen.
4. XML und CSV müssen dieselben eindeutigen Nummern enthalten. Persönliche Kontakte ohne öffentliche belastbare Spam-Belege gehören ausschließlich in die private Sperrliste.
5. Keine Zusatzkosten, kostenpflichtigen APIs oder Abonnements. Keine Tellows-Scorelisten ohne geeignete ausdrückliche kostenlose Weitergabefreigabe.
6. Änderungen im Changelog dokumentieren, möglichst gemeinsam veröffentlichen und alle geänderten Dateien zurücklesen.

## Import und Aktualisierung in Begone

**GitHub-Veröffentlichung und iPhone-Übernahme sind getrennte Schritte.** Der Hersteller dokumentiert Import/Export und Community-Listen, aber in den geprüften öffentlichen Angaben keine automatische Synchronisierung dieser GitHub-Datei:
- [Begone beim Hersteller](https://begone.app/)
- [Begone im App Store](https://apps.apple.com/app/id1596818195)

Bis zu einem belegten anderen Verfahren gilt der manuelle Weg:
1. Vor dem ersten bzw. erneuten Import die vorhandene Begone-Konfiguration privat exportieren und sichern. Der Export kann persönliche Regeln enthalten und gehört nicht in dieses öffentliche Repository.
2. Die [aktuelle XML](https://raw.githubusercontent.com/gregorwallmeier-ai/begone-spam-de/main/begone-de-gemeldete-nummern.xml) als Datei herunterladen und auf dem iPhone in „Dateien“ speichern.
3. In Begone den angebotenen Nummernimport öffnen und die Datei auswählen. Die konkreten Menünamen müssen an der installierten App-Version geprüft werden.
4. Falls Begone eine Aktualisierung bzw. ein Neuladen der Nummern anbietet, diese ausführen und die Erfolgsmeldung kontrollieren. Das Neuladen allein ist kein belegter Download von GitHub.
5. Stichprobenartig eine bekannte Listenregel und die eigenen Freigaben kontrollieren. Die 57 XML-Regeln müssen wegen vorhandener privater Regeln und möglicher nationaler Zusatzvarianten nicht der Gesamtanzeige der App entsprechen.

**Noch offen, auf dem iPhone zu testen:**
- Akzeptiert die installierte Version diese XML und bleiben eigene Regeln/Freigaben erhalten?
- Erzeugt ein erneuter Import Duplikate oder erkennt Begone bereits vorhandene Nummern?
- Werden Regeln, die aus der XML entfernt wurden, bei einem erneuten Import auf dem Telefon gelöscht? Bis zum Nachweis nicht davon ausgehen. Betroffene Nummern gezielt prüfen und bei Bedarf manuell korrigieren.
- Lässt sich unsere Liste getrennt von privaten Sperren verwalten?
- Gibt es für unsere eigene URL eine dokumentierte kostenlose Aktualisierungsfunktion?

Für die Löschprüfung nur eine selbst kontrollierte Testnummer in einer privaten Testkonfiguration verwenden, keine fremden echten Nummern ergänzen. Keine vollständige Sperrliste löschen, um einen Import zu erzwingen. Ein technischer Dateitest ersetzt keinen Import- oder Anruftest auf dem iPhone.

## Automatische Repository-Pflege

Eine bestehende wöchentliche ChatGPT-Aufgabe pflegt das Repository. Am 26.10.2026 wurde sie nach deaktiviertem Zustand wieder aktiviert und um genauere Qualitäts- und Rücklesekontrollen ergänzt. Es gibt im Repository keinen eigenen GitHub-Actions-Workflow.

Der frühere Lauf vom 26.10.2026 ist im Aufgabensystem als fehlgeschlagen gespeichert, obwohl die Änderungen für Version 1.2 tatsächlich auf GitHub veröffentlicht wurden. Die Ursache ist nicht ausgewiesen; eine vollständige Fehlerbehebung oder erfolgreiche künftige Ausführung ist daher noch nicht nachgewiesen. Ausführung und Zustellung der nächsten Aufgabe müssen kontrolliert werden. Die Aufgabe bewirkt keine bestätigte iPhone-Synchronisierung.

## Quellenrechte und Korrekturen

Begrenzte redaktionelle Einzelauswahl, keine Kopie kompletter Datenbanken. Keine fremden Kommentartexte übernehmen. Öffentlich lesbar bedeutet keine pauschale Erlaubnis zum Datenbankexport. Bei unklaren Nutzungsbedingungen vor einer Ausweitung die Bedingungen klären.

Für Korrekturen bitte einen [GitHub-Issue](https://github.com/gregorwallmeier-ai/begone-spam-de/issues) mit Rufnummer, Grund und möglichst öffentlichem Beleg eröffnen. Keine Namen, Adressen oder privaten Anruflisten veröffentlichen.

Das Projekt ist weder mit Begone noch mit Tellows verbunden. Nutzung ohne Gewähr auf Vollständigkeit, Fehlerfreiheit oder Wirksamkeit.
