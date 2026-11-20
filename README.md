# Amazon-Seller Prompt-Library

70 Prompts in 7 Bereichen: Margenkalkulator, Produktoptimierung, Verhandlung, Produktsuche, Ads-Optimierung, Geld sparen, KW-Tracking.

> **So nutzt du sie:** Prompt kopieren, alles in [eckigen Klammern] durch deine Zahlen ersetzen, deine Daten darunter einfügen. Fehlt etwas, fragt der Prompt nach, statt zu raten. Die Badges zeigen, welche Regel der Prompt einhält.

## Inhalt

- [Margenkalkulator](#margenkalkulator)
- [Produktoptimierung](#produktoptimierung)
- [Verhandlung](#verhandlung)
- [Produktsuche](#produktsuche)
- [Ads-Optimierung](#ads-optimierung)
- [Geld sparen](#geld-sparen)
- [KW-Tracking](#kw-tracking)
- [Regeln](#regeln)

## Legende (Badges)

| Badge | Bedeutung |
|---|---|
| `basis` | ACoS- und Preisbasis nennen |
| `frei` | nur Vorschlag, Freigabe nötig |
| `platz` | Platzhalter, keine erfundenen Zahlen |
| `fach` | Fachfrage, keine Auskunft |
| `daten` | nur deine eingefügten Daten |
| `bew` | Amazon-Bewertungsregeln |
| `dsg` | Kundendaten vorher anonymisieren |

## Margenkalkulator

### 1. Break-even-ACoS berechnen

**Wann:** Vor jeder Werbeentscheidung

**Regeln:** `ACoS- und Preisbasis nennen` · `Platzhalter, keine erfundenen Zahlen`

```text
Du bist Analyst für Amazon-FBA-Margen. Berechne meine Break-even-ACoS.
Eingaben (fehlt etwas, frag nach, statt zu schätzen):
- Verkaufspreis brutto: [ ] €
- MwSt-Satz: [ ] %
- Amazon-Verkaufsgebühren pro Stück: [ ] €
- FBA-/Versandgebühr pro Stück: [ ] €
- Wareneinsatz inkl. Fracht und Zoll: [ ] €
- Sonstige variable Kosten: [ ] €

Schritte:
1. Netto-Verkaufspreis berechnen.
2. Marge vor Werbung in € und in % des Nettopreises.
3. Break-even-ACoS = Werbekosten, bei denen der Gewinn genau 0 € ist, als Anteil am Umsatz.
4. Zeige die Break-even-ACoS zweimal: auf Netto-Umsatz und auf Brutto-Umsatz. Kennzeichne jede Zahl mit ihrer Basis.
5. Liste alle Annahmen am Ende auf.
```

### 2. MwSt-Check des Netto-Preises

**Wann:** Bei jedem neuen Produkt und bei Kategoriewechsel

**Regeln:** `Fachfrage, keine Auskunft` · `Platzhalter, keine erfundenen Zahlen`

```text
Prüfe, ob mein Netto-Preis richtig aus dem Brutto-Preis gerechnet ist.
Brutto: [ ] € · Satz laut meiner Kalkulation: [ ] %
Zeige den Rechenweg: Netto = Brutto ÷ (1 + Satz). Danach die Differenz zu meiner Kalkulation in €.
Ob der Satz für [Produktart] richtig ist, kannst du nicht final beurteilen. Formuliere stattdessen 2 konkrete Fragen für meinen Steuerberater.
```

### 3. Vollständigkeits-Check der Kosten

**Wann:** Wenn die Marge „zu gut“ aussieht

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Prüfe, welche Kostenposten in meinem Margenrechner fehlen könnten. Geh diese Liste durch:
Abo-Gebühr, Lagergebühren (monatlich und Langzeit), Inbound-Versand, Retouren (Verlust und Entsorgung), Verpackung, Zoll und Einfuhrumsatzsteuer, Werbung, Rücklagen für Reklamationen, Zahlungsgebühren.

Ausgabe als Tabelle:
Posten | in meiner Kalkulation? (ja / nein / unklar) | welche Zahl ich dafür brauche
```

### 4. Preis-Szenarien

**Wann:** Vor Preisänderung oder Aktion

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Rechne fünf Preisszenarien für [Produkt]: Verkaufspreis brutto -10 %, -5 %, aktuell, +5 %, +10 %. Die Kosten bleiben gleich.
Tabelle:
Preis brutto | Netto | Marge € | Marge % | Break-even-ACoS (Basis angeben)

Ergänze eine Zeile: ab welchem Preis die Marge unter meine Mindestmarge von [ ] % fällt.
```

### 5. Rabatt-Check für Aktionen

**Wann:** Vor Coupon oder Blitzangebot

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Ich plane eine Aktion mit [ ] % Rabatt auf einen Verkaufspreis brutto von [ ] €.
Berechne:
1. Marge € und % nach Rabatt (mit Netto-Preis, Rechenweg zeigen)
2. Break-even-ACoS nach Rabatt (Basis angeben)
3. Die höchste Rabattstufe, bei der die Marge meine Grenze von [ ] % nicht unterschreitet

Das ist eine Kalkulation. Ob die Aktion nach Amazon-Vorgaben erlaubt ist, prüfe ich selbst.
```

### 6. Retouren in die Marge einrechnen

**Wann:** Wenn die Retourenquote steigt

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Meine Daten:
- Retourenquote: [ ] %
- Kosten je Retoure (Versand, Verlust, Entsorgung): [ ] €
- Wiederverkaufsquote der Retouren: [ ] %

Berechne die effektive Marge pro verkauftem Stück nach Retouren. Zeige, wie sich die Break-even-ACoS dadurch verschiebt (Basis angeben). Nenne jede Annahme, die ich bestätigen muss.
```

### 7. Einstandskosten bei Import (Landed Cost)

**Wann:** Bei Einkauf aus Asien oder Drittland

**Regeln:** `Fachfrage, keine Auskunft` · `Platzhalter, keine erfundenen Zahlen`

```text
Berechne die Einstandskosten pro Stück (landed cost) für [Produkt].
Eingaben:
- Einkaufspreis je Stück: [ ] €
- Frachtkosten gesamt: [ ] €
- Stückzahl: [ ]
- Zollsatz laut Zolltarif: [ ] %
- Einfuhrumsatzsteuer: [ ] %
- Nebenkosten (Zollabfertigung, Transport zum Lager): [ ] €

Reihenfolge: Zollwert (Warenwert + Fracht bis EU-Grenze) → Zoll → Einfuhrumsatzsteuer auf Zollwert + Zoll. Zeige jeden Schritt.
Den Zollsatz prüfst du im offiziellen Zolltarif. Du übernimmst ihn nicht ungeprüft.
```

### 8. Break-even-Stückzahl mit Fixkosten

**Wann:** Vor Bestellung oder Werbebudget

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Meine Zahlen:
- Fixkosten pro Monat (Tool-Abos, Lagerfixkosten): [ ] €
- Marge vor Werbung je Stück: [ ] €
- Geplantes Werbebudget pro Monat: [ ] €

Berechne:
1. Stückzahl pro Monat, bei der die Fixkosten ohne Werbung gedeckt sind.
2. Stückzahl pro Monat mit dem geplanten Werbebudget.
3. Den Umsatz, der dazu nötig ist (brutto und netto).
```

### 9. Plausibilitäts-Check meiner Kalkulation

**Wann:** Bevor du Entscheidungen darauf stützt

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Prüfe meine Kalkulation auf typische Fehler, bevor ich Entscheidungen darauf stütze. Meine Eingaben: [einfügen]
Checkliste, pro Punkt "ok" oder "prüfen" mit einem Satz Begründung:
- Netto und Brutto verwechselt?
- Gebühr auf der falschen Basis berechnet?
- Werbekosten doppelt eingerechnet?
- Wareneinsatz pro Stück oder pro Karton?
- Gewicht und Maße passen zur angegebenen Versandklasse?
```

### 10. Margenrechnung einfach erklärt

**Wann:** Wenn du sie einem Teammitglied oder Einsteiger erklären willst

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Erkläre meine Margenrechnung einem Einsteiger in fünf Schritten.
Jeder Schritt: ein Satz plus eine Zahl aus meiner Kalkulation: [einfügen]
Keine Fachbegriffe ohne Erklärung. Zum Schluss: frag mich, welcher Schritt noch unklar ist.
```

## Produktoptimierung

### 1. Titel verbessern

**Wann:** Bei schwacher Sichtbarkeit oder niedriger Klickrate

**Regeln:** `Platzhalter, keine erfundenen Zahlen` · `nur deine eingefügten Daten`

```text
Verbessere den Titel meines Produkts.
- Aktueller Titel: [ ]
- Keyword-Liste aus meinem Tool-Export: [einfügen]
- Produktmerkmale, die ich belegen kann: [ ]
- Zeichenlimit laut Amazon-Vorgabe der Kategorie: [ ] (bitte selbst prüfen)

Liefere 3 Titelvorschläge: zuerst lesbar, dann Keywords. Erfinde keine Merkmale, die nicht in meinen Angaben stehen. Gib pro Titel die Zeichenzahl an.
```

### 2. Bullet Points aus Kundenbewertungen

**Wann:** Wenn das Listing die Kundensprache nicht trifft

**Regeln:** `Kundendaten vorher anonymisieren` · `nur deine eingefügten Daten` · `Amazon-Bewertungsregeln`

```text
Hier sind [Anzahl] Kundenbewertungen, nur Text, anonymisiert:
[einfügen]

Finde die fünf Themen, die Kunden am häufigsten loben, und die drei, die sie am häufigsten kritisieren.
Formuliere daraus 5 Bullet Points: Nutzen zuerst, Merkmal danach. Nur Aussagen, die in den Bewertungen vorkommen.
```

### 3. Retouren-Ursachen clustern

**Wann:** Monatlich, wenn die Retourenquote steigt

**Regeln:** `Kundendaten vorher anonymisieren` · `Platzhalter, keine erfundenen Zahlen`

```text
Hier ist mein Retourenexport (Grund als Freitext, Anzahl, SKU):
[einfügen]

1. Gruppiere die Gründe in höchstens 6 Cluster.
2. Ordne jedes Cluster einer Ursache zu: Listing (Erwartung falsch), Produkt (Qualität, Passform) oder Versand.
3. Für Listing-Gründe: welcher Satz oder welches Bild würde das verhindern?
4. Priorisiere nach Anzahl × Kosten je Retoure [ ] €.
```

### 4. 1–3-Sterne-Bewertungen analysieren

**Wann:** Einmal pro Monat

**Regeln:** `Kundendaten vorher anonymisieren` · `Amazon-Bewertungsregeln`

```text
Analysiere die 1–3-Sterne-Bewertungen:
[einfügen, anonymisiert]

Ausgabe:
- Wiederkehrende Probleme mit ungefährer Häufigkeit
- Welche davon ich im Produkt, in der Verpackung oder in der Anleitung ändern kann
- Welche ich nur im Listing klarer erklären muss

Keine Vorschläge, Bewertungen entfernen zu lassen oder Kunden zu einer Änderung zu bewegen.
```

### 5. FAQ-Entwurf

**Wann:** Vor dem Start oder nach neuen Kundenfragen

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Erstelle 15 Fragen, die Käufer vor dem Kauf wahrscheinlich stellen. Grundlage sind nur diese Produktdaten:
[einfügen]

Beantworte jede Frage nur mit Fakten aus meinen Angaben. Braucht eine Antwort Daten, die ich nicht genannt habe, schreib "Bitte ergänzen: ..." statt zu raten.
```

### 6. Bildbriefing

**Wann:** Vor dem Fotoshooting oder Grafik-Auftrag

**Regeln:** `Fachfrage, keine Auskunft`

```text
Erstelle ein Bildbriefing für [Produkt] mit 7 Bildslots: Hauptbild, Nutzenbild 1–3, Maße, Lieferumfang, Anwendung.
Pro Slot:
- Botschaft in einem Satz
- Overlay-Text (höchstens [ ] Wörter)
- Hintergrund und Setting
- Requisiten

Das Hauptbild muss die aktuellen Amazon-Bildrichtlinien für die Kategorie erfüllen. Prüfe das anhand der Richtlinien selbst.
```

### 7. A+-Content-Module

**Wann:** Wenn die Markenseite fehlt oder schwach ist

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Schreibe Texte für vier A+-Content-Module zu [Produkt]:
1. Problem und Lösung
2. Funktionen mit Maßen
3. Vergleich zu [Alternative], ohne Namen anderer Marken zu nennen
4. Anwendung in drei Schritten

Nutze nur Angaben aus: [einfügen]
Kurze Sätze, höchstens [ ] Zeichen pro Modul.
```

### 8. Keyword-Lücken im Listing finden

**Wann:** Nach einem Keyword-Export

**Regeln:** `Platzhalter, keine erfundenen Zahlen` · `nur deine eingefügten Daten`

```text
Vergleiche Titel, Bullets und Beschreibung:
[einfügen]
mit meiner Keyword-Liste:
[einfügen]

Zeige:
- Relevante Keywords, die fehlen
- Keywords, die doppelt vorkommen, ohne Mehrwert
- Keywords, die nicht zum Produkt passen

Keine Keyword-Häufung: Jeder Begriff nur dort, wo er einen Satz besser macht.
```

### 9. Varianten prüfen

**Wann:** Wenn Varianten Bestand binden oder Bewertungen streuen

**Regeln:** `nur Vorschlag, Freigabe nötig`

```text
Prüfe die Varianten von [Produkt]:
[Liste: Farbe, Größe, Verkäufe, Bewertungen, Bestand]

Empfehle pro Variante: behalten, zusammenführen oder auslaufen lassen. Begründe jeweils mit den Zahlen.
Nur Vorschläge. Ich entscheide, was umgesetzt wird.
```

### 10. Eigenes Listing gegen drei Wettbewerber

**Wann:** Vor einer Listing-Überarbeitung

**Regeln:** `nur deine eingefügten Daten`

```text
Vergleiche mein Listing:
[einfügen]
mit drei Listings, die ich unten eingefügt habe:
[einfügen]

Nutze nur die eingefügten Texte. Nichts aus dem Netz.
Ausgabe: Tabelle mit Titel, Anzahl Bilder, Bullets, Preis, Bewertungsanzahl (von mir angegeben). Markiere, wo ich klar zurückliege, und nenne die 3 einfachsten Verbesserungen.
```

## Verhandlung

### 1. Preisgespräch vorbereiten

**Wann:** Vor dem Anruf oder Videocall mit dem Lieferanten

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Bereite mich auf ein Preisgespräch mit meinem Lieferanten vor.
- Angebot: [ ] € je Stück bei [ ] Stück
- Mein Ziel: [ ] €
- Mein Walk-away-Preis (aus meiner Margenrechnung): [ ] €
- Was ich bieten kann: [z. B. Abnahmemenge, Vorkasse, Langfristigkeit]

Erstelle:
1. Ziel und Ausweichpreis
2. Drei Argumente mit Belegen
3. Drei Gegenfragen des Lieferanten mit meinen Antworten
4. Zugeständnisse nur gegen eine Gegenleistung

Den Walk-away-Preis nenne ich dem Lieferanten nie.
```

### 2. Preisanfrage per E-Mail (Englisch)

**Wann:** Für Lieferanten in China oder Asien

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Schreibe eine höfliche Preisanfrage an einen Lieferanten auf Englisch für [Produkt].
Inhalt:
- Bezug auf meine Anfrage vom [Datum]
- Menge: [ ] Stück
- Zielpreis je Stück: [ ] (EXW oder FOB, bitte angeben)
- Frage nach Staffelpreisen für [ ] und [ ] Stück
- Frage nach Musterkosten und Lieferzeit

Ton: sachlich und freundlich. Höchstens 120 Wörter.
Keine Zusagen für künftige Großaufträge, die ich nicht gemacht habe.
```

### 3. MOQ-Abwägung

**Wann:** Wenn der Lieferant eine hohe Mindestmenge verlangt

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Mein Lieferant verlangt eine Mindestmenge (MOQ) von [ ] Stück zu [ ] € je Stück. Ich möchte [ ] Stück bestellen.

Berechne für drei Szenarien:
- Stückpreis, der bei meiner Menge nötig wäre
- Kapitalbindung in €
- Lagerkosten über [ ] Monate
- Auswirkung auf meine Marge (Basis angeben)

Tabelle mit drei Szenarien. Empfiehl eine Verhandlungsforderung.
```

### 4. Muster-Bestellung verhandeln

**Wann:** Vor der ersten Großbestellung

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Verhandle Muster für [Produkt]:
- Musterkosten: [ ] €
- Versandkosten: [ ] €
- Mein Wunsch: Muster-Kosten werden bei der Hauptbestellung angerechnet

Schreib mir:
1. Eine Forderung
2. Ein Angebot, das ich machen kann
3. Eine Prüfliste für das Muster: Maße, Material, Verpackung, Funktion
```

### 5. Zahlungsbedingungen prüfen

**Wann:** Wenn der Lieferant hohe Vorkasse verlangt

**Regeln:** `Fachfrage, keine Auskunft` · `Platzhalter, keine erfundenen Zahlen`

```text
Der Lieferant verlangt [ ] % Anzahlung und [ ] % vor Versand.
Erstelle:
1. Einen Vorschlag für ein ausgewogeneres Zahlungsmodell
2. Eine Liste von Absicherungs-Optionen (z. B. Zahlungsabsicherung über die Bank, Qualitätsprüfung vor Versand)
3. Fünf Fragen, die ich vor der Zahlung klären muss

Das ist keine Rechtsberatung. Vertragsentwürfe lasse ich vor der Unterschrift von Fachleuten prüfen.
```

### 6. Logistik-Angebote vergleichen

**Wann:** Bei neuen Versanddienstleistern

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Vergleiche diese Angebote für [Strecke / Menge]:
[einfügen]

Tabelle mit: Gesamtkosten inkl. aller Zusatzposten (Zollabfertigung, Lagerannahme, Treibstoffzuschlag, Mindestmenge), Lieferzeit, Haftung, Kündigungsfrist.
Markiere Posten, die nur im Kleingedruckten stehen. Liste die Fragen, die ich jedem Anbieter stellen muss.
```

### 7. Rollenspiel: harter Lieferant

**Wann:** Zum Üben, bevor du echte Gespräche führst

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Spiele meinen Lieferanten in einem Verhandlungsgespräch. Du bist hart, aber fair, und bringst immer neue Einwände.
Ich starte mit: [mein Angebot]

Nach jeder Runde: zwei Sätze Feedback (was gut war, was ich besser machen kann).
Nach 6 Runden: Auswertung und ein Vorschlag für meine beste Schlussformulierung.
Mein Ziel: [Preis].
```

### 8. Agenturhonorar bewerten

**Wann:** Bei Ads- oder Listing-Agenturen

**Regeln:** `ACoS- und Preisbasis nennen` · `Platzhalter, keine erfundenen Zahlen`

```text
Ich verhandle mit einer Agentur. Angebot: [Fixpreis / Prozent vom Umsatz / Prozent vom Gewinn].
Rechne drei Szenarien (Umsatz niedrig, mittel, hoch) mit meiner Marge von [ ] % (Basis angeben):
- Was ich an die Agentur zahle
- Wie sich das auf meine Marge auswirkt

Schlag eine Vertragsgestaltung vor, bei der mein Risiko begrenzt bleibt, auch bei schwachen Ergebnissen.
```

### 9. Logistiker-Konditionen neu verhandeln

**Wann:** Wenn das Paketvolumen gestiegen ist

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Ich will die Kosten mit meinem Logistikdienstleister neu verhandeln.
- Aktuelle Kosten je Paket: [ ] €
- Volumen: [ ] Pakete pro Monat
- Retourenquote: [ ] %

Erstelle:
1. Einen Zielpreis
2. Argumente, die auf meinem Volumen beruhen
3. Ein Gegenangebot mit Mengenstaffel oder Mindestbetrag
4. Die Frage, welche Zusatzgebühren er zuerst offenlegen muss
```

### 10. Gebührenabweichung an Amazon-Support

**Wann:** Wenn ein Settlement nicht stimmt

**Regeln:** `Fachfrage, keine Auskunft`

```text
Schreibe eine sachliche Nachricht an den Amazon-Seller-Support zu einer Abweichung im Settlement.
Fakten:
- Settlement-ID: [ ]
- Zeitraum: [ ]
- Erwartete Gebühr: [ ] €
- Abgerechnete Gebühr: [ ] €
- Belege: [Liste]

Keine Vorwürfe, nur Fakten und die Bitte um Prüfung und ggf. Korrektur. Ende mit der konkreten Frage, welche Gebühr geprüft werden soll.
Ich prüfe und sende die Nachricht selbst.
```

## Produktsuche

### 1. Produktideen bewerten (Scoring)

**Wann:** Wenn du mehrere Ideen parallel prüfst

**Regeln:** `Platzhalter, keine erfundenen Zahlen` · `nur deine eingefügten Daten`

```text
Bewerte diese Produktideen: [Liste]
Kriterien und Gewichtung (Vorschlag, bitte anpassen):
- Marge vor Werbung (30 %)
- Wettbewerbsdichte (20 %)
- Gewicht, Größe, Versandkosten (15 %)
- Saisonalität (10 %)
- Einkaufsrisiko und Zertifikate (15 %)
- Bewertungsqualität der Wettbewerber (10 %)

Pro Idee: 1–5 Punkte je Kriterium mit Begründung aus meinen Daten: [einfügen]
Fehlt ein Datenwert, schreib "offen" statt zu schätzen.
```

### 2. Mindest-Margen-Filter

**Wann:** Bei einer langen Kandidatenliste

**Regeln:** `ACoS- und Preisbasis nennen` · `Platzhalter, keine erfundenen Zahlen` · `nur deine eingefügten Daten`

```text
Filtere meine Kandidatenliste:
[einfügen: Produkt, VK brutto, Gebühren, Wareneinsatz]
Mindestmarge vor Werbung: [ ] % (Basis: netto)

Ausgabe in drei Gruppen:
- Über der Grenze
- Knapp darunter (bis [3] Prozentpunkte)
- Weit darunter

Keine Annahmen zu Gebühren, die nicht in der Liste stehen.
```

### 3. Wettbewerbsdichte einordnen

**Wann:** Vor der Entscheidung für eine Nische

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Bewerte die Wettbewerbsdichte für [Keyword / Produkt] mit diesen Daten:
- Anzahl relevanter Angebote: [ ]
- Anteil der Top-10-Angebote mit mehr als [ ] Bewertungen: [ ] %
- Anzahl Marken: [ ]
- Preisspanne: [ ] bis [ ] €

Ergebnis: niedrig, mittel oder hoch, mit Begründung.
Welche Annahme hat die größte Unsicherheit? Welche Daten sollte ich zusätzlich holen?
```

### 4. Saison und Trend prüfen

**Wann:** Vor einer Erstbestellung

**Regeln:** `Platzhalter, keine erfundenen Zahlen` · `nur deine eingefügten Daten`

```text
Analysiere Saisonalität und Trend für [Produkt] auf Basis dieses Exports: [Trend- oder Verlaufsdaten einfügen]

Ausgabe:
- Hoch- und Tiefpunkte pro Monat
- Bis wann der Bestand vor Saisonstart da sein muss (Vorlauf Lieferant [ ] Wochen + Transport [ ] Wochen)
- Ob der Trend stabil wirkt oder nach einer Einmal-Welle aussieht
```

### 5. Compliance-Checkliste

**Wann:** Vor Verkaufsstart in Deutschland oder der EU

**Regeln:** `Fachfrage, keine Auskunft`

```text
Erstelle eine Checkliste für [Produkt, Kategorie] für den Verkauf in Deutschland und der EU.
Prüfe jeweils, ob es zutrifft:
- CE-Kennzeichnung
- Batterien (Batteriegesetz, Registrierungspflicht)
- Verpackungsregister (VerpackG)
- Vorgaben für Lebensmittel oder Kosmetik
- Sicherheitsdatenblatt
- Allgemeine Produktsicherheit

Pro Punkt: die Frage, die ich an die zuständige Stelle oder die Händler-Dokumentation richte. Keine verbindliche Aussage.
```

### 6. Lieferanten-Bewertungsmatrix

**Wann:** Bei Alibaba oder anderen Plattformen

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Erstelle eine Bewertungsmatrix für Lieferanten von [Produkt].
Kriterien: Handelsart (Hersteller oder Händler), Zertifikate, Musterqualität, Antwortzeit, Mindestbestellmenge, Dokumentation (Datenblatt, Prüfberichte).

Pro Lieferant: 1–5 Punkte je Kriterium, Begründung und rote Flaggen.
Zusätzlich: 5 Fragen, die ich jedem Lieferanten vor den Mustern stelle.
```

### 7. Produktlücken aus fremden Bewertungen

**Wann:** Für bessere Version eines Konkurrenzprodukts

**Regeln:** `Kundendaten vorher anonymisieren` · `nur deine eingefügten Daten` · `Amazon-Bewertungsregeln`

```text
Analysiere die 1–3-Sterne-Bewertungen von [Anzahl] Konkurrenzprodukten:
[einfügen, anonymisiert]

Ausgabe als Tabelle:
Problem | wie oft genannt | mögliche Produktverbesserung | Machbarkeit (niedrig / mittel / hoch)

Keine Nutzerdaten übernehmen. Nur Themen, nicht Personen.
```

### 8. Versandklasse und Gewicht prüfen

**Wann:** Vor Produktentscheidung und Verpackungsplanung

**Regeln:** `Fachfrage, keine Auskunft` · `Platzhalter, keine erfundenen Zahlen`

```text
Schätze die Versandkosten-Situation für [Produkt]:
- Maße: [L × B × H cm]
- Gewicht: [ ] g
- Verkaufspreis brutto: [ ] €

Zeige, in welche Größen- und Gewichtsklasse es nach den Amazon-Vorgaben fällt. Die Gebühr bitte in den aktuellen Gebührenseiten selbst bestätigen.
Was würde eine Verpackungsänderung auf [ ] cm bringen? Das Ergebnis ist eine Hypothese, keine verbindliche Gebühr.
```

### 9. Go/No-Go-Memo

**Wann:** Bevor du Geld für die erste Bestellung ausgibst

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Schreibe ein Go/No-Go-Memo für [Produkt], höchstens eine Seite.
Abschnitte:
1. Idee in einem Satz
2. Zahlen: Marge, Break-even-ACoS (Basis angeben), Kapitalbedarf für die erste Bestellung
3. Größte Unbekannte
4. Kill-Kriterien mit Zahlen: wann ich abbreche
5. Testbudget und Testdauer

Empfehlung nur aus meinen Angaben. Fehlen Daten, nenne "Entscheidung verschieben" als Option.
```

### 10. Spec-Sheet für Lieferanten

**Wann:** Für die erste Anfrage oder ein Angebot

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Erstelle aus meinen Angaben ein Produkt-Spec-Sheet für eine Lieferanten-Anfrage:
Maße, Material, Gewicht, Farben, Verpackung, Logo-Wünsche, Zertifikate, Menge, Zielpreis.
Fehlende Punkte mit [FEHLT] markieren.
Format: Tabelle, die ich in eine E-Mail kopieren kann.
Meine Angaben: [einfügen]
```

## Ads-Optimierung

### 1. Wochen-Report (Montag)

**Wann:** Jeden Montag über die letzten 7 Tage

**Regeln:** `ACoS- und Preisbasis nennen` · `nur Vorschlag, Freigabe nötig`

```text
Erstelle meinen Ads-Wochenreport für die letzten 7 Tage (Mo bis So) aus diesem Export:
[Kampagne, Suchbegriff oder Platzierung, Ausgaben, Umsatz, Klicks, Impressionen, Bestellungen]

Basis: ACoS in beiden Varianten, brutto und netto, bis die Basisfrage geklärt ist. Jede Zahl mit Basis und Zeitfenster kennzeichnen.
Ausgabe:
1. Top 3 Gewinner mit Zahlen
2. Top 3 Verlierer mit Zahlen
3. Vorschläge mit Begründung
4. Offene Fragen

Keine Änderung ausführen. Nur Vorschläge für meine Freigabe.
```

### 2. Suchbegriffe sortieren

**Wann:** Nach dem Suchbegriffsbericht

**Regeln:** `ACoS- und Preisbasis nennen` · `nur Vorschlag, Freigabe nötig`

```text
Sortiere diese Suchbegriffe in vier Gruppen: Negativ setzen (Vorschlag), Gebot senken, Gebot halten, Hochskalieren.
[Export einfügen]

Pro Begriff ein Satz Begründung mit einer Zahl (Klicks, Ausgaben, Bestellungen, ACoS mit Basis).
Mindestklicks für eine Entscheidung: [ ]. Darunter: "zu wenig Daten".
```

### 3. Negativ-Keywords vorschlagen

**Wann:** Wenn Ausgaben ohne Bestellung laufen

**Regeln:** `nur Vorschlag, Freigabe nötig` · `ACoS- und Preisbasis nennen`

```text
Erstelle Negativ-Keyword-Vorschläge aus diesem Suchbegriffsbericht:
[einfügen]

Nur Begriffe, die klar nicht zum Produkt passen oder nach [ ] Klicks ohne Bestellung liegen.
Format: Begriff | Match-Typ (negativ exakt oder Phrase) | Begründung | Klicks | Ausgaben

Nichts davon anlegen. Das mache ich nach Freigabe.
```

### 4. Gebotsvorschläge am Break-even

**Wann:** Wenn die Ziel-ACoS nicht erreicht wird

**Regeln:** `ACoS- und Preisbasis nennen` · `nur Vorschlag, Freigabe nötig` · `Platzhalter, keine erfundenen Zahlen`

```text
Schlage Gebotsanpassungen für diese Keywords vor.
Grundlage: Break-even-ACoS von [ ] % (Basis: [netto oder brutto]) und Ziel-ACoS von [ ] % (gleiche Basis).
Regelentwurf:
- Gebot senken, wenn ACoS über Ziel liegt und genug Daten vorhanden sind
- Gebot halten, wenn ACoS zwischen Ziel und Break-even liegt
- Nie über Break-even bieten

Pro Keyword: Vorschlag, Begründung und die Zahl, auf der er beruht. Vergleiche nur Werte mit gleicher Basis. Du änderst nichts.
Keywords: [einfügen]
```

### 5. Tagesalarm-Check

**Wann:** Täglich, nur bei Abweichung

**Regeln:** `ACoS- und Preisbasis nennen`

```text
Prüfe diese Tagesdaten nur auf Abweichungen:
[einfügen]

Prüfe:
- Tagesausgaben über [ ]-fachem des 7-Tage-Schnitts
- Budget vor [ ] Uhr aufgebraucht
- Umsatz 0 bei Kampagnen, die in der Vorwoche Bestellungen hatten

Gib nur Treffer aus, mit Zahlen. Ohne Treffer: "keine Alarme". Du änderst nichts.
```

### 6. Platzierungen vergleichen

**Wann:** Wenn Top-of-Search anders läuft als der Rest

**Regeln:** `ACoS- und Preisbasis nennen`

```text
Vergleiche die Platzierungen meiner Kampagne (Top of Search, Produktseiten, Rest):
[Export einfügen]

Ausgabe pro Platzierung: ACoS (Basis angeben), Klicks, Bestellungen.
Vorschlag für Gebotszuschläge mit Begründung. Sag ausdrücklich, wenn die Datenbasis zu dünn ist.
```

### 7. Kampagnenstruktur prüfen

**Wann:** Wenn Kampagnen sich gegenseitig Klicks wegnehmen

**Regeln:** `nur Vorschlag, Freigabe nötig`

```text
Prüfe die Struktur meiner Kampagnen:
[Liste: Name, Typ (automatisch oder manuell), Match-Typen, Budget, Gebotsstrategie]

Empfehle, wo Kampagnen zusammengelegt, getrennt oder pausiert werden sollten. Begründe mit meinem Ziel (Break-even, genug Lerndaten).
Nur Vorschläge.
```

### 8. Creative-Testplan

**Wann:** Bevor du zwei Anzeigen gegeneinander testest

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Entwirf einen Testplan für zwei Anzeigen-Creatives (A: [ ], B: [ ]) für [Produkt].
Enthalten:
- Hypothese in einem Satz
- Metrik (z. B. CTR oder ACoS, mit Basis)
- Testdauer und Mindest-Impressionen pro Variante
- Stop-Regel
- Was ich nach dem Test entscheide

Keine Ergebnisse erfinden. Ohne Daten nur den Plan. Keine Änderung an Kampagnen.
```

### 9. ACoS und TACoS erklären

**Wann:** Wenn Kennzahlen verwechselt werden

**Regeln:** `ACoS- und Preisbasis nennen`

```text
Erkläre ACoS und TACoS einfach, anhand meiner Zahlen:
- Werbeausgaben: [ ] €
- Umsatz aus Werbung: [ ] €
- Gesamtumsatz: [ ] €
- Zeitraum: [ ]

Berechne beide. Nenne die Basis und das Zeitfenster.
Sag, welche Kennzahl ich für welche Entscheidung nehmen sollte und warum beide verschiedene Fragen beantworten.
Keine Änderung an Kampagnen.
```

### 10. Freigabe-Nachricht für Slack

**Wann:** Nach dem Wochenreport, vor jeder Änderung

**Regeln:** `nur Vorschlag, Freigabe nötig` · `ACoS- und Preisbasis nennen`

```text
Formuliere eine Freigabe-Nachricht für Slack. Pro Vorschlag eine Zeile:
Aktion | Kampagne oder Keyword | Grund in einem Satz | erwarteter Effekt | Risiko | Basis (brutto oder netto, Zeitfenster)

Am Ende: "Freigabe nötig: ja / nein" pro Zeile.
Jede Aktion bestätige ich einzeln. Nichts umsetzen.
```

## Geld sparen

### 1. Settlement-Gebühren-Audit

**Wann:** Alle zwei Wochen beim Settlement

**Regeln:** `nur deine eingefügten Daten` · `Fachfrage, keine Auskunft`

```text
Prüfe diese Settlement-Zeilen auf unerwartete oder doppelte Gebühren:
[einfügen]

Gruppiere: Verkaufsgebühren, FBA-Gebühren, Lager, Werbung, Erstattungen, Sonstiges.
Ausgabe:
- Auffälligkeiten mit Betrag und Zeile
- Pro Auffälligkeit eine sachliche Frage für den Amazon-Support

Keine Schlüsse über Absicht. Nur was die Zahlen zeigen.
```

### 2. Abo- und Tool-Check

**Wann:** Einmal im Quartal

**Regeln:** `nur Vorschlag, Freigabe nötig`

```text
Liste meine Abos und Tools:
[Name | Kosten pro Monat | Nutzen in einem Satz | letzte Nutzung]

Empfehle pro Eintrag: behalten, prüfen oder kündigen.
Rechne die Jahreskosten und den Anteil am Monatsumsatz [ ] €.
Ich entscheide. Du kündigst nichts.
```

### 3. Lagerkosten analysieren

**Wann:** Wenn Lagergebühren steigen

**Regeln:** `nur Vorschlag, Freigabe nötig`

```text
Analysiere meine Lagerkosten:
[Export: SKU, Bestand, Lagertage, Gebühren, Verkaufsrate]

Ausgabe:
- SKUs mit hohen Lagergebühren oder Risiko für Langzeitlager
- Bestandsreichweite in Tagen (Bestand ÷ Tagesabverkauf)
- Optionen pro SKU: abverkaufen, zurückholen oder entsorgen (als Optionen, nicht als Befehl)
```

### 4. Versandoptionen vergleichen

**Wann:** Vor einem Wechsel des Versandwegs

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Vergleiche diese Versandoptionen für [Produkt]:
- Paketgewicht: [ ] kg
- Maße: [ ]
- Zielgebiet: [ ]
[Angebote einfügen]

Tabelle: Gesamtkosten je Paket, Lieferzeit, Tracking, Haftung, Mindestabnahme.
Rechne den Effekt auf die Marge in € aus.
```

### 5. Retourenkosten senken

**Wann:** Wenn die Retourenquote über deiner Grenze liegt

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Meine Retourenquote liegt bei [ ] %, Kosten je Retoure [ ] €, Retouren pro Monat [ ].
Nenne 8 Hebel, sortiert nach erwartetem Effekt und Aufwand: Listing-Erwartung, Größentabelle, Verpackung, Produktqualität, Retourenbearbeitung.
Pro Hebel: ungefähre Ersparnis in € pro Monat, mit Rechenweg.
```

### 6. Verpackung und Gewicht optimieren

**Wann:** Wenn Versandkosten zu hoch sind

**Regeln:** `Fachfrage, keine Auskunft` · `Platzhalter, keine erfundenen Zahlen`

```text
Analysiere meine Verpackung:
[Maße, Gewicht, Material, Füllmaterial]

Finde Einsparungen bei Gewicht oder Größenklasse, ohne den Produktschutz zu verringern.
Liste Varianten mit Kosten und Risiko für Beschädigungen.
Die Pflichten nach dem Verpackungsgesetz prüfe ich mit einem Fachmann. Das ist hier keine Auskunft.
```

### 7. Fragen für den Steuerberater

**Wann:** Vor dem Quartalsgespräch

**Regeln:** `Fachfrage, keine Auskunft`

```text
Bereite eine Fragenliste für meinen Steuerberater vor.
Themen: [z. B. Umsatzsteuer bei Verkäufen aus Drittländern, Einfuhrumsatzsteuer, Betriebsausgaben, Lager im EU-Ausland]

Stelle Fragen, keine Antworten. Pro Frage: welche Unterlage ich mitbringe.
Keine Steuerberatung durch dich.
```

### 8. Werbeausgaben ohne Ertrag finden

**Wann:** Monatlich oder bei steigendem ACoS

**Regeln:** `ACoS- und Preisbasis nennen` · `nur Vorschlag, Freigabe nötig` · `nur deine eingefügten Daten`

```text
Finde Werbeausgaben, die keinen Umsatz bringen.
Daten: [Export: Kampagne oder Keyword, Ausgaben, Umsatz, Bestellungen, Zeitraum]

Ausgabe:
- Summe der Ausgaben ohne Bestellung im Zeitraum
- Top 10 Verursacher
- Pro Verursacher ein Vorschlag (prüfen, senken oder negativ setzen) als Liste zur Freigabe

Keine Änderung.
```

### 9. Bestandsreichweite und gebundenes Kapital

**Wann:** Vor einer Nachbestellung

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Berechne für [SKUs]:
- Bestandsreichweite in Tagen (Bestand ÷ Tagesabverkauf)
- Gebundenes Kapital in € (Bestand × Einkaufspreis)
- Kapitalkosten bei [ ] % Zinsen pro Jahr

Empfiehl eine Nachbestellmenge, bei der das Lager nicht länger als [ ] Tage reicht, plus Sicherheitsbestand für eine Lieferzeit von [ ] Wochen.
```

### 10. Monatlicher Kosten-Check

**Wann:** Am Monatsende

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Erstelle eine Vorlage für meinen monatlichen Kosten-Check.
Positionen: Fixkosten, variable Kosten, Gebühren, Werbung, Lager, Versand, Retouren, Bank und Zahlung.
Pro Position: Betrag aktuell, Betrag Vormonat, Abweichung in €, offene Frage an mich.
Keine Zahlen erfinden. Lass die Felder leer, wo ich nichts angegeben habe.
```

## KW-Tracking

### 1. Tracking-Liste aufbauen

**Wann:** Zu Beginn für jede ASIN

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Baue eine Keyword-Tracking-Liste für ASIN [ ].
Input: Keyword-Liste mit Suchvolumen-Hinweis: [einfügen]
Aktuelle Listing-Position je Keyword: [einfügen]

Ausgabe als Tabelle:
Keyword | Priorität (1–3) | Zielfeld (Titel, Bullets, Backend) | Tracking-Frequenz

Höchstens 30 Keywords mit Priorität 1. Begründung in einem Satz je Keyword.
```

### 2. Ranking-Veränderungen auswerten

**Wann:** Wöchentlich

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Hier ist mein Ranking-Export der letzten 14 Tage:
[Keyword, Position je Tag]

1. Alle Keywords mit einem Verlust von mehr als [ ] Positionen in 7 Tagen
2. Alle Keywords mit Gewinn
3. Zu jedem größeren Verlust: Prüffragen zu möglichen Ursachen (Preis, Bestand, Bewertungen, Ads-Änderung, Konkurrenz)

Ich habe keine Ursachendaten. Formuliere Ursachen als Fragen, die ich prüfen kann.
```

### 3. Keywords nach Suchabsicht clustern

**Wann:** Wenn die Liste unübersichtlich wird

**Regeln:** `Platzhalter, keine erfundenen Zahlen` · `nur deine eingefügten Daten`

```text
Gruppiere diese Keywords nach Suchabsicht:
[einfügen]

Cluster: Kauf (z. B. kaufen, günstig), Vergleich, Problem und Lösung, Information, Marke.
Pro Cluster: Anzahl, Top-Keywords, welches Listing-Element es stärken sollte.
Keine Keywords erfinden.
```

### 4. Keyword-Lücke zum Wettbewerber

**Wann:** Vor einer Listing-Überarbeitung

**Regeln:** `nur deine eingefügten Daten`

```text
Vergleiche meine Rankings:
[Liste]
mit der Liste eines Wettbewerbers, die ich unten eingefügt habe:
[Liste]

Zeige:
- Keywords, bei denen der Wettbewerber vorne liegt und ich fehle
- Keywords, bei denen ich vorne liege
- 5 Lücken mit dem besten Verhältnis aus Relevanz und Machbarkeit

Nur mit den eingefügten Daten arbeiten.
```

### 5. Keywords dem Listing zuordnen

**Wann:** Vor dem Schreiben der Texte

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Ordne diese Keywords den Listing-Feldern zu:
[einfügen]
Felder: Titel, Bullet 1 bis 5, Beschreibung, Backend-Suchbegriffe.

Regeln: Jedes Keyword einmal an der sinnvollsten Stelle. Keine Häufung. Der Titel bleibt lesbar.
Ausgabe: Tabelle, plus eine Liste der Keywords, die ins Listing nicht mehr passen.
```

### 6. Alarm-Regeln definieren

**Wann:** Einmal einrichten, dann nachschärfen

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Definiere 6 Alarm-Regeln für mein Keyword-Tracking. Format:
"Wenn [Keyword] in [Zeitraum] um mehr als [ ] Positionen fällt, dann prüfen: [ ]"

Themen: Ranking-Verlust, Verlust aus den Top 3, neue Konkurrenz, Bestandsrisiko, Preisabweichung, Verlust an Bewertungen.
Jede Schwelle als Platzhalter.
```

### 7. Long-Tail-Varianten bilden

**Wann:** Wenn Seed-Keywords zu allgemein sind

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Erstelle 30 Long-Tail-Varianten aus diesem Seed-Keyword: [ ]
Meine Produktmerkmale, die ich belegen kann: [ ]

Markiere pro Variante, zu welchem Merkmal sie passt. Keine Varianten, die das Produkt nicht beschreiben.
Sortiere nach Relevanz, nicht nach geschätztem Volumen.
```

### 8. Saison-Kalender für Keywords

**Wann:** Einmal im Jahr planen

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Erstelle einen Keyword-Saisonkalender für [Produkt] für die nächsten 12 Monate.
Input: meine Verkaufsdaten [einfügen], Trend-Export [einfügen].
Pro Monat: welche Keywords vorbereitet werden müssen, Lieferanten-Vorlauf [ ] Wochen, Ads-Start.
Fehlen Vorjahresdaten, markiere den Monat als "offen".
```

### 9. Suchvolumen einordnen

**Wann:** Bevor du Zahlen aus einem Tool übernimmst

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Ich habe Suchvolumen aus [Tool] für diese Keywords: [einfügen]. Stand: [Datum], Zeitraum: [ ].

Erkläre:
- Wie belastbar diese Zahlen sind
- Welche Zahlen Schätzungen sind
- Wie ich sie mit meinen eigenen Verkaufs- und Klickzahlen gegenprüfe

Keine eigene Zahl erfinden.
```

### 10. Keyword-Monatsreport

**Wann:** Am Monatsende

**Regeln:** `Platzhalter, keine erfundenen Zahlen`

```text
Erstelle meinen Keyword-Monatsreport aus diesen Daten:
[Keyword, Position Monatsanfang, Position Monatsende, Suchvolumen-Hinweis]

KPIs:
- Anzahl Keywords in den Top 10 (vorher und nachher)
- Anzahl in den Top 3
- Gewonnen und verloren
- Größter Gewinner und größter Verlierer

Drei Maßnahmen für den nächsten Monat, jede mit Begründung und Erfolgsmessung.
```

## Regeln

**Keine erfundenen Zahlen**  
Gebühren, Schwellen und Benchmarks stehen als [Platzhalter] oder kommen von dir. Die Vorlage aus dem GitHub-Repo nannte generische Benchmarks (z. B. ROAS über 4). Übernommen wurde nur der Aufbau, keine Werte.

**ACoS immer mit Basis**  
Jede ACoS- oder Margenangabe nennt Netto oder Brutto und das Zeitfenster. Die Break-even-ACoS folgt deiner Definition: Werbung, bei der der Gewinn genau 0 € ist. Ob Amazon brutto oder netto rechnet, ist offen. Deshalb zeigen die Prompts beide Varianten.

**Ads nur als Vorschlag**  
Kein Ads-Prompt ändert etwas. Jede Aktion braucht eine einzelne Freigabe, so wie es dein Ads-Workflow vorsieht.

**Keine Scraping-Prompts**  
Wettbewerber- und Produktdaten nur, was du einfügst oder exportierst. Kein Prompt fragt nach Abruf von Amazon-Seiten oder umgeht Zugriffsbeschränkungen.

**Bewertungen nach Amazon-Regeln**  
Keine Bitte um positive Bewertungen, keine Anreize, keine Versuche, Bewertungen entfernen zu lassen. Kundenkommunikation bleibt sachlich.

**Steuern, Zoll, Recht, Produktsicherheit**  
Die Prompts liefern Checklisten und Fragen, keine verbindliche Auskunft. Offen ist zum Beispiel der MwSt-Satz für Tee (Memory: 7 % oder 19 %, nicht geprüft). Das klärt der Steuerberater.

**Keine Finanz- oder Anlageberatung**  
Die Prompts betreffen Geschäftskosten und Werbung. Keine Empfehlung zu Geldanlagen.

**Keine Zugangsdaten, Kundendaten anonymisieren**  
Kein Prompt verlangt Passwörter, API-Schlüssel oder Kontodaten. Bewertungs- und Retourenlisten bitte vorher von Namen und Adressen befreien.

**Keine Aussagen über N42-Funktionen**  
Die Prompts sagen „dein Margenrechner“ und beschreiben keine Funktionen des N42-MCP. Dessen Umfang ist laut Memory noch nicht bestätigt.

**Sprache**  
Deutsch, Du-Form. Englisch nur für die beiden Lieferanten-Mails (V2) und die Preisanfrage.

**Neutrale Formulierungen**  
Keine Pronomen für dich im Text, weil sie nicht angegeben sind.

## Teilen

Wenn dir die Prompts helfen und du zufrieden bist, teile sie gern weiter und markiere **@listingschmiede**. Das freut uns sehr. 🙂

## Lizenz

Dieses Werk steht unter der [Creative Commons Namensnennung 4.0 International](https://creativecommons.org/licenses/by/4.0/deed.de) (CC BY 4.0). Du darfst es nutzen, teilen und verändern, auch kommerziell, solange du den Urheber nennst: **CKnauz**.
