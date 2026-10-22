# Begone-Spamsperrliste Deutschland (Community-Projekt)

**Stand: 22.10.2026 · Version 1.0 · Experimentelle Community-Zusammenstellung**

Eine kostenlose, manuell zusammengestellte XML-Sperrliste für [Begone](https://begone.app/) auf dem iPhone.

## Inhalt

- [**Sperrliste herunterladen**](begone-de-gemeldete-nummern.xml): 53 **einzeln öffentlich gemeldete** deutsche Telefonnummern als Sperrregeln. Keine Wildcards oder flächendeckenden Vorwahl-Sperren.
- [**Quellenübersicht**](quellen.csv): Zuordnung der Nummern zu öffentlich zugänglichen Meldungen bei Clever Dialer, PhoneBlock oder Spam-Barometer (Auswertungsstand Oktober 2026).
- [**tellows – Integrationsstatus**](TELLOWS_INTEGRATION.md): mögliche künftige Datenquelle, derzeit **nicht** eingebunden.
- [**Änderungsprotokoll**](CHANGELOG.md).

**Wichtig:** Meldungen von Nutzern sind keine unabhängig bewiesenen Betrugsfälle. Ein angezeigter Anruf kann eine gefälschte Rufnummer tragen (Caller-ID-Spoofing). Telefonnummern können später neu vergeben werden. Eine Sperre kann dadurch legitime Anrufe treffen.

## Import in Begone

1. XML-Datei auf dem iPhone in der App *Dateien* speichern.
2. Begone → *Importieren* → *Neue Nummern importieren* → XML-Datei auswählen.
3. Begone → *Alle Nummern neu laden* bzw. *Nummern aktualisieren*.
4. Bestehende eigene Sperren und gegebenenfalls Freigaben kontrollieren.

Die XML-Syntax wurde maschinell geprüft. Der erfolgreiche Import auf unterschiedlichen Begone-/iOS-Versionen ist **nicht** allgemein verifiziert.

## Quellen und Lizenz

Es handelt sich um eine begrenzte redaktionelle Auswahl öffentlich gemeldeter Nummern; **keine vollständige Kopie fremder Datenbanken**. Die Quelle ist je Nummer in `quellen.csv` angegeben. Keine übernommenen Kommentartexte oder markenrechtlichen Bezeichnungen.

Die Daten von *tellows* sind **nicht** in dieser Version enthalten. Für eine systematische Nutzung oder öffentliche Weitergabe von tellows-Scorelisten sollte zuvor eine geeignete Lizenz oder Freigabe von tellows eingeholt werden. Das Projekt ist weder mit tellows noch mit Begone verbunden.

## Korrektur und Beschwerden

Bitte einen [GitHub-Issue](../../issues) eröffnen, wenn eine Rufnummer zu Unrecht gelistet erscheint, die Quelle nicht nachvollziehbar ist oder die Nummer nicht mehr auffällig ist. Nenne ausschließlich die betroffene Rufnummer, den Grund für die Korrektur und nach Möglichkeit einen öffentlichen Beleg; **keine Namen, Adressen oder privaten Anruflisten** einstellen. Bis zur Prüfung kann die Nummer individuell in Begone freigegeben werden.

## Aktualisierungen

Die Liste ist eine Momentaufnahme. Keine automatische Synchronisierung mit dem Telefon, und keine Zusage regelmäßiger Updates. Vor neuen Versionen sollten Quellen und aktuelle Meldedaten überprüft werden; veraltete oder beanstandete Nummern werden entfernt. Änderungen bitte mit Datum im Änderungsprotokoll dokumentieren.

## Haftungsausschluss

Nutzung auf eigene Verantwortung, ohne Gewähr auf Vollständigkeit, Fehlerfreiheit oder Wirksamkeit. Die Liste beschuldigt keine konkrete Person oder Firma, einen Betrug begangen zu haben.
