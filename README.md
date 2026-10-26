# Begone-Spamsperrliste Deutschland (Community-Projekt)

**Stand: 26.10.2026 · Version 1.2 · Experimentelle Community-Zusammenstellung**

Eine kostenlose, manuell zusammengestellte XML-Sperrliste für [Begone](https://begone.app/) auf dem iPhone. Sie richtet sich an Nutzer in Deutschland und enthält neben deutschen Nummern auch ausdrücklich gemeldete unerwünschte Kontakte aus dem Ausland.

## Inhalt

- [**Sperrliste herunterladen**](begone-de-gemeldete-nummern.xml): 58 einzelne Telefonnummern als Sperrregeln: 57 deutsche Einträge und eine US-Nummer aufgrund einer direkten Nutzermeldung. Keine Wildcards oder flächendeckenden Vorwahl-Sperren.
- [**Quellenübersicht**](quellen.csv): Zuordnung aller 58 Nummern zu öffentlich nachvollziehbaren Meldungen bei Clever Dialer, PhoneBlock, Spam-Barometer oder zu der gesondert gekennzeichneten direkten Nutzermeldung. Vier neue deutsche Einträge (Prüfdatum 26.10.2026) sind mit Einzel-URL, Datum und Risiko dokumentiert; drei schwach belegte Bestandsnummern mit Prüfhinweis gekennzeichnet.
- [**tellows – Integrationsstatus**](TELLOWS_INTEGRATION.md): mögliche künftige Datenquelle, derzeit **nicht** eingebunden.
- [**Änderungsprotokoll**](CHANGELOG.md).

### Unerwünschter Kontakt ist nicht gleich nachgewiesener Spam oder Betrug

`+16465185265` wurde am 23.10.2026 auf ausdrücklichen Wunsch eines Nutzers nach einem nicht angenommenen Anruf aufgenommen. Der Eintrag trägt die Bezeichnung **„Unerwünschter Kontakt – Nutzermeldung“**. Identität und Anrufzweck sind nicht unabhängig bestätigt. Dies ist eine einzelne subjektive Meldung, keine allgemeine Spamfeststellung und kein Nachweis von Betrug oder rechtswidriger Werbung. Die Regel betrifft nur diese vollständige internationale Nummer, keinen Nummernblock. Andere Nutzer können diese Nummer von der Sperre ausnehmen.

Die 53 deutschen Einträge aus Version 1.1 bleiben als Sperrregeln unverändert; drei davon sind wegen geringer aktueller Beleglage in `quellen.csv` zur Nachprüfung markiert. Es wurde keine dieser Nummern ohne belastbaren Gegenbeleg gelöscht.

**Ergänzungen vom 26.10.2026:** Vier einzelne, bei PhoneBlock öffentlich dokumentierte deutsche Rufnummern wurden aufgenommen. Bei drei Nummern berichten Nutzer über angebliche Gewinnspiel- oder Lotto-Abos (hohe Risikoeinstufung als *Verdacht*); eine Nummer ist als störender Scherzanrufdienst eingestuft (mittleres Belästigungsrisiko, kein Betrugsvorwurf). Die Einzelbelege, die Daten der letzten Beschwerden und die Risikoeinstufung stehen in `quellen.csv`. Nach Sichtung der aktuellen Maßnahmenliste der Bundesnetzagentur fand sich für diese vier Rufnummern kein dort dokumentierter Abschaltbescheid; dies ist kein Nachweis, dass die Rufnummern tatsächlich aktiv oder den angezeigten Anrufern zuzuordnen sind.

**Wichtig:** Meldungen von Nutzern sind keine unabhängig bewiesenen Betrugsfälle. Ein angezeigter Anruf kann eine gefälschte Rufnummer tragen (Caller-ID-Spoofing). Telefonnummern können später neu vergeben werden. Eine Sperre kann dadurch legitime Anrufe treffen.

## Import in Begone

1. XML-Datei auf dem iPhone in der App *Dateien* speichern.
2. Begone → *Importieren* → *Neue Nummern importieren* → XML-Datei auswählen.
3. Begone → *Alle Nummern neu laden* bzw. *Nummern aktualisieren*.
4. Bestehende eigene Sperren und gegebenenfalls Freigaben kontrollieren.

Die XML-Syntax wurde maschinell geprüft. Der erfolgreiche Import auf unterschiedlichen Begone-/iOS-Versionen ist **nicht** allgemein verifiziert.

## Quellen und Lizenz

Es handelt sich um eine begrenzte redaktionelle Auswahl öffentlich gemeldeter Nummern, ergänzt um ausdrücklich beauftragte und entsprechend gekennzeichnete direkte Nutzermeldungen; **keine vollständige Kopie fremder Datenbanken**. Die Quelle ist je Nummer in `quellen.csv` angegeben. Keine übernommenen Kommentartexte oder markenrechtlichen Bezeichnungen.

Die Daten von *tellows* sind **nicht** in dieser Version enthalten. Für eine systematische Nutzung oder öffentliche Weitergabe von tellows-Scorelisten sollte zuvor eine geeignete Lizenz oder Freigabe von tellows eingeholt werden. Das Projekt ist weder mit tellows noch mit Begone verbunden.

## Korrektur und Beschwerden

Bitte einen [GitHub-Issue](../../issues) eröffnen, wenn eine Rufnummer zu Unrecht gelistet erscheint, die Quelle nicht nachvollziehbar ist oder die Nummer nicht mehr auffällig ist. Nenne ausschließlich die betroffene Rufnummer, den Grund für die Korrektur und nach Möglichkeit einen öffentlichen Beleg; **keine Namen, Adressen oder privaten Anruflisten** einstellen. Bis zur Prüfung kann die Nummer individuell in Begone freigegeben werden.

## Aktualisierungen

Die Liste ist eine Momentaufnahme. Keine automatische Synchronisierung mit dem Telefon, und keine Zusage regelmäßiger Updates. Vor neuen Versionen sollten Quellen und aktuelle Meldedaten überprüft werden; veraltete oder beanstandete Nummern werden entfernt. Änderungen bitte mit Datum im Änderungsprotokoll dokumentieren.

## Haftungsausschluss

Nutzung auf eigene Verantwortung, ohne Gewähr auf Vollständigkeit, Fehlerfreiheit oder Wirksamkeit. Die Liste beschuldigt keine konkrete Person oder Firma, einen Betrug begangen zu haben.
