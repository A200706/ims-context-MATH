# SUPER-MD — KAP 7: Gleichungen Textaufgaben (ohne 7.7)
# IMS BWD Bern | IM25A | Probe2_2 — 01.04.2026

> **Zweck**: Dieses Dokument ist die einzige Wissensquelle für die KI.
> Lies es VOLLSTÄNDIG, bevor du antwortest.
> Antworte NUR basierend auf diesem Inhalt.

---

## [QUICK-ROUTER] Fragetyp erkennen

Lies die Aufgabe. Finde Schlüsselwörter → wähle den passenden T-Block:

| Schlüsselwörter | → Route |
|---|---|
| Zahl, Ziffer, Bruch, Zähler, Nenner, Stellenwert, zweistellig, dreistellig, Produkt zweier Zahlen, Summe zweier Zahlen, Differenz zweier Zahlen | → T-ZAHL |
| alt, Jahre, Mutter, Vater, Tochter, Sohn, heute, vor … Jahren, in … Jahren | → T-ALTER |
| Kapital, Zins, verzinst, Sparkonto, Bankkonto, Prozentpunkt, Zinssatz, Jahreszins, Marchzins, Zinsgutschrift, Darlehen | → T-ZINS |
| aufgeteilt, verteilt, erhält, Anteil, Gewinn, Lottogewinn, Kosten … aufgeteilt, Firmen | → T-VERT |
| Mischung, Gehalt, Spiritus, Alkohol, Mehl, Sorte, Legierung, Kakao, Tee, Preis pro kg | → T-MISCH |
| Geschwindigkeit, km/h, Strecke, fährt, Zug, Auto, Radfahrer, kreuzen, überholt, entgegen | → T-BEWEG |
| Rechteck, Quadrat, Fläche, Flächeninhalt, Umfang, Seite, cm, m², verlängert, verkürzt | → T-GEO |
| Alles andere (Treppe, Stufen, Verein, Bus, Einkauf, Hemden, Orangen, Mitglieder) | → T-DIV |

---

## [MICRO-INDEX] Token-Verzeichnis

**QT-Tokens (Antwort-Schablonen):**
- QT-TAB → Analyse-Tabelle (IMMER verwenden — gibt Punkte!)
- QT-EQ1 → Gleichung mit 1 Unbekannten lösen
- QT-EQ2 → Gleichungssystem mit 2 Unbekannten lösen
- QT-QUAD → Quadratische Gleichung (abc-Formel)
- QT-BRUCH → Bruchgleichung (Hauptnenner)

**T-Tokens (Themenblöcke):**
- T-ZAHL → Zahlenaufgaben (7.2)
- T-ALTER → Altersaufgaben (7.3)
- T-ZINS → Kapital und Zins (7.4)
- T-VERT → Verteilungsaufgaben (7.5)
- T-MISCH → Mischungsaufgaben (7.6)
- T-BEWEG → Bewegung (7.8)
- T-GEO → Geometrie (7.9)
- T-DIV → Diverses (7.10)

**X-Tokens (Fallen/Referenz):**
- X-TRAP → Häufige Fehler pro Thema
- X-FORMELN → Alle Formeln (LaTeX)
- X-GLOSSAR → Deutsche Mathe-Begriffe

---

## [WORKFLOW] Universelle 7-Schritte-Methode

Jede Textaufgabe wird so gelöst:

1. **Analyse** → Aufgabe lesen, Tabelle aufstellen (QT-TAB), Beziehungen identifizieren
2. **Variable** → x = gesuchte Grösse definieren (evtl. y bei 2 Unbekannten)
3. **Gleichung** → Aus Tabelle die Gleichung(en) aufstellen
4. **D** → Definitionsmenge angeben (z.B. D = Q⁺, D = N, D = Q⁺\{0})
5. **Lösen** → Gleichung Schritt für Schritt lösen (QT-EQ1/EQ2/QUAD/BRUCH)
6. **L / Antwortsatz** → Lösungsmenge + vollständiger Antwortsatz mit Einheiten
7. **Probe** → Nur wenn explizit verlangt oder Platz vorhanden

---

## [ANSWER-RULES] Ausgabeformat — STRIKT

### Formatregeln (HARD):
- Jede Zeile beginnt mit n) → 1), 2), 3), …
- KEIN "Schritt"-Header, KEIN "Zusammenfassend", KEIN Meta-Kommentar
- Genau EINE Gleichung/Aktion pro nummerierte Zeile
- Operationen IMMER am Ende in [ ] → z.B. `[| ·100]` oder `[| ausmultiplizieren]`
- Brüche in LaTeX: `\frac{a}{b}` (nie a/b)
- Wenn Zeile zu lang → aufteilen in zwei nummerierte Zeilen
- Sprache: Deutsch, Schulniveau Sek II
- IMMER: Tabelle → Variable → Gleichung → D → Lösung → Antwortsatz

### Tabelle (QT-TAB) — IMMER ausgeben:
```
Tabelle:
| | Grösse 1 | Grösse 2 | Beziehung |
|---|---|---|---|
| Zeile 1 | Wert | Wert | ... |
| Zeile 2 | Wert | Wert | ... |
```
Zeilen und Spalten BESCHRIFTEN. Gibt Punkte auch bei falschem Rechenweg!

### Beispiel einer perfekten Ausgabe:

**Aufgabe:** Die Mutter ist heute 5-mal so alt wie ihre Tochter. In 6 Jahren wird sie nur noch 3-mal so alt sein. Wie alt sind Mutter und Tochter heute?

**Ausgabe:**

Tabelle:
| | Mutter | Tochter |
|---|---|---|
| Heute | 5x | x |
| In 6 Jahren | 5x + 6 | x + 6 |

Beziehung: Alter Mutter in 6 J. = 3 · Alter Tochter in 6 J.

1) x = Alter der Tochter heute
2) 5x + 6 = 3(x + 6)
3) D = \mathbb{N}
4) 5x + 6 = 3x + 18 [| ausmultiplizieren]
5) 2x + 6 = 18 [| -3x]
6) 2x = 12 [| -6]
7) x = 6 [| :2]
8) Alter Mutter: 5 \cdot 6 = 30
9) Die Mutter ist heute 30 Jahre, die Tochter 6 Jahre alt.

---

## [QT-TAB] Analyse-Tabelle — Vorlagen pro Typ

### Altersaufgabe:
| | Person A | Person B |
|---|---|---|
| Heute | ... | x |
| Vor n Jahren | ... | x - n |
| In n Jahren | ... | x + n |

### Zinsaufgabe:
| | Kapital 1 | Kapital 2 |
|---|---|---|
| Guthaben | x | ... |
| Zinssatz (%) | ... | ... |
| Zeit | ... | ... |
| Zins | \frac{K \cdot p \cdot M}{100 \cdot 12} | \frac{K \cdot p \cdot M}{100 \cdot 12} |

### Verteilungsaufgabe:
| Person | Anteil |
|---|---|
| A | x |
| B | ... (in x ausdrücken) |
| C | ... (in x ausdrücken) |
| **Total** | **Gesamtbetrag** |

### Mischungsaufgabe:
| | Komponente 1 | Komponente 2 | Mischung |
|---|---|---|---|
| Menge | ... | ... | Summe |
| Gehalt (%) | ... | ... | x |
| Reinmenge | Menge₁ · Gehalt₁ | Menge₂ · Gehalt₂ | Summe · x |

### Bewegungsaufgabe:
| | Objekt A | Objekt B |
|---|---|---|
| v (km/h) | ... | ... |
| t (h) | x | x (oder x ± Δt) |
| s (km) | v_A · t_A | v_B · t_B |
| Gesamt | s_A + s_B = d (oder s_A = s_B) |

### Geometrie:
| | Original | Neu |
|---|---|---|
| Länge | ... | ... ± Δ |
| Breite | ... | ... ± Δ |
| Fläche | l · b | l_neu · b_neu |

---

## [QT-EQ1] Gleichung mit 1 Unbekannten

Schema:
1) x = [Definition]
2) [Gleichung aufstellen]
3) D = [Definitionsmenge]
4) [Umformung] [| Operation]
5) [Umformung] [| Operation]
6) x = [Ergebnis] [| letzte Operation]
7) [Antwortsatz]

---

## [QT-EQ2] Gleichungssystem mit 2 Unbekannten

Schema (Gleichsetzungs- oder Einsetzungsverfahren):
1) x = [Definition], y = [Definition]
2) (1) [Gleichung 1]
3) (2) [Gleichung 2]
4) D = [Definitionsmenge]
5) Aus (1): x = ... [| nach x auflösen]
6) Einsetzen in (2): ... [| x ersetzen]
7) [Lösen nach y] [| Operation]
8) y = [Ergebnis]
9) x berechnen: x = ... [| y einsetzen]
10) [Antwortsatz]

Oder Additionsverfahren:
5) (1) · k: ... [| ·k]
6) (2) · m: ... [| ·m]
7) Gleichungen addieren/subtrahieren
8) [Lösen] [| Operation]

---

## [QT-QUAD] Quadratische Gleichung

Schema (abc-Formel):
1) [Gleichung in Normalform bringen]: ax² + bx + c = 0
2) a = ..., b = ..., c = ...
3) x_{1,2} = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
4) x_{1,2} = \frac{... \pm \sqrt{...}}{...} [| einsetzen]
5) x_1 = ..., x_2 = ...
6) [Prüfen: Welche Lösung passt in D?]
7) [Antwortsatz]

---

## [QT-BRUCH] Bruchgleichung

Schema:
1) D bestimmen: Nenner ≠ 0 → D = ...
2) Hauptnenner (HN) = ...
3) [Gleichung] [| ·HN]
4) [Ausmultiplizieren] [| ausmultiplizieren]
5) [Vereinfachen und lösen] [| Operation]
6) [Antwortsatz]

---

## [T-ZAHL] Zahlenaufgaben (7.2)

**Grundmenge:** G = Q bzw. Q × Q

### Stellenwert-Muster:
- Zweistellige Zahl mit Ziffern a, b: 10a + b
- Dreistellige Zahl mit Ziffern a, b, c: 100a + 10b + c
- Vierstellige Zahl: 1000a + 100b + 10c + d

### "Ziffer hinzufügen"-Muster:
- Links Ziffer d anfügen bei zweistelliger Zahl x: 100d + x (wird dreistellig)
- Rechts Ziffer d anfügen bei zweistelliger Zahl x: 10x + d (wird dreistellig)
- Links UND rechts Ziffer d anfügen: 1000d + 10x + d (bei zweistellig → vierstellig)

### Bruch-Muster:
- Zähler + Nenner = Summe → z + n = S
- Bruch = \frac{z}{n}, Kehrwert = \frac{n}{z}
- "Addiert man k zum Zähler und Nenner": \frac{z+k}{n+k} = Wert

### Produkt/Summe/Differenz:
- "Summe ist S, Differenz ist D" → x + y = S, x - y = D → löse System
- "Produkt ist P, Summe ist S" → x · y = P, x + y = S → quadratische Gl.

---

## [T-ALTER] Altersaufgaben (7.3)

**Grundmenge:** G = N bzw. N × N (Alter = natürliche Zahlen)

### Zeitverschiebungs-Muster:
- "Heute" → Alter = x (oder 5x, etc.)
- "Vor n Jahren" → Alter MINUS n bei ALLEN Personen
- "In n Jahren" → Alter PLUS n bei ALLEN Personen

### ⚠️ WICHTIG:
- "x-mal so alt" = MULTIPLIKATION: Alter_A = x · Alter_B
- "x Jahre älter" = ADDITION: Alter_A = Alter_B + x
- NICHT verwechseln!

### Typische Gleichung:
Aussage: "In 6 Jahren ist Mutter 3-mal so alt wie Tochter"
→ (Alter_M + 6) = 3 · (Alter_T + 6)

### Setup:
1) Tabelle mit Heute / Vor n J. / In n J. aufstellen
2) x = Alter der jüngeren Person heute
3) Ältere Person in x ausdrücken (z.B. 5x, x + 20, etc.)
4) Zeitverschiebung anwenden
5) Gleichung aus der 2. Aussage bilden

---

## [T-ZINS] Kapital und Zins (7.4) — GRÖSSTER BLOCK

**Grundmenge:** G = Q⁺ bzw. Q⁺ × Q⁺

### Formeln:

**Jahreszins:**
$$Z = \frac{K \cdot p}{100}$$

**Marchzins (Monate):**
$$Z = \frac{K \cdot p \cdot M}{100 \cdot 12}$$

**Marchzins (Tage):**
$$Z = \frac{K \cdot p \cdot t}{100 \cdot 360}$$

Wobei: K = Kapital, p = Zinssatz (ohne %), M = Monate, t = Tage

### Muster A: Zwei Kapitalien, Gesamtzins
Gegeben: K₁ = x, K₂ = x + d (oder K₂ = Gesamt - x)
Zinssätze und Zeitraum bekannt.
Gleichung: Zins₁ + Zins₂ = Gesamtzins

### Muster B: Vertauschte Zinssätze (2 Gleichungen, 2 Unbekannte)
Fall 1: K₁ zu p₁%, K₂ zu p₂% → Gesamtzins = A
Fall 2: K₁ zu p₂%, K₂ zu p₁% → Gesamtzins = B
→ Gleichungssystem aufstellen, Additionsverfahren verwenden

### Muster C: Zinseszins über 2 Jahre (→ quadratische Gleichung)
- Jahr 1: Kapital K₀, Zins₁ = K₀ · p/100, Kontostand = K₀ + Zins₁
- Jahr 2: Neues Kapital = K₀ + Zins₁, Zins₂ = (K₀ + Zins₁) · p/100
- Kontostand nach 2 Jahren = K₀ + Zins₁ + Zins₂
- Wenn p gesucht → quadratische Gleichung in p

### Muster D: Einzahlung/Abhebung zwischen Jahren
- Nach Zinsgutschrift Jahr 1: Kontostand₁ = K₀ + Zins₁
- Einzahlung +E oder Abhebung -A am gleichen Tag
- Neues Kapital für Jahr 2: K₁ = Kontostand₁ ± E/A
- Zins Jahr 2 basiert auf K₁

### Muster E: Zinssatz-Änderung
- Jahr 1: Zinssatz p
- Jahr 2: Zinssatz p + Δ (erhöht) oder p - Δ (gesenkt)
- Δ = Prozentpunkte (NICHT Prozent!)

### ⚠️ FALLEN:
- Prozentpunkte vs. Prozent: "0.5 Prozentpunkte höher" → p + 0.5 (NICHT p · 1.005)
- Marchzins: M/12 NICHT vergessen! 8 Monate = \frac{8}{12} = \frac{2}{3}
- Zinseszins: Zins wird zum Kapital addiert → neues Kapital
- "Gleicher Jahreszins" bei verschiedenen Kapitalien → K₁·p₁ = K₂·p₂

### Beispiel-Setup (Muster A):
Tabelle:
| | Kleineres Kapital | Grösseres Kapital |
|---|---|---|
| Guthaben | x | x + 13'000 |
| Zinssatz | 1.5% | 1.25% |
| Zeit | 8 Monate | 8 Monate |
| Zins | \frac{x \cdot 1.5 \cdot 8}{100 \cdot 12} | \frac{(x+13000) \cdot 1.25 \cdot 8}{100 \cdot 12} |

Gleichung: Zins₁ + Zins₂ = 585

---

## [T-VERT] Verteilungsaufgaben (7.5)

**Grundmenge:** G = Q⁺ bzw. Q⁺ × Q⁺

### Kernprinzip:
ALLE Anteile durch EINE Variable x ausdrücken, dann:
Summe aller Anteile = Gesamtbetrag

### Prozent-Muster:
| Ausdruck | Bedeutung | Formel |
|---|---|---|
| "50% mehr als x" | x plus die Hälfte von x | 1.5x |
| "20% weniger als x" | x minus ein Fünftel | 0.8x |
| "25% mehr als x" | | 1.25x |
| "40% weniger als x" | | 0.6x |
| "Doppelt so viel wie x" | | 2x |
| "Die Hälfte von x" | | 0.5x |
| "Ein Drittel von x" | | \frac{x}{3} |
| "Ein Drittel mehr als x" | x plus ein Drittel von x | \frac{4}{3}x |
| "Ein Drittel weniger als x" | x minus ein Drittel von x | \frac{2}{3}x |

### Verhältnis-Muster:
"Verhältnis A : B = 3 : 2" → Wenn B = x, dann A = \frac{3}{2}x

### Setup:
1) Wähle die Person/Firma als x, von der die meisten anderen abhängen
2) Drücke alle anderen Anteile in x aus
3) Gleichung: Summe aller Anteile = Gesamtbetrag
4) Löse nach x → berechne alle Anteile

---

## [T-MISCH] Mischungsaufgaben (7.6)

**Grundmenge:** G = Q⁺ × Q⁺

### Kernprinzip:
Reinmenge₁ + Reinmenge₂ = Reinmenge_Mischung

Wobei: Reinmenge = Menge × \frac{Gehalt}{100}

### Gehalt-Tabelle:
| | Komp. 1 | Komp. 2 | Mischung |
|---|---|---|---|
| Menge (Liter/kg) | m₁ | m₂ | m₁ + m₂ |
| Gehalt (%) | g₁ | g₂ | x |
| Reinmenge | m₁ · g₁ | m₂ · g₂ | (m₁+m₂) · x |

Gleichung: m₁ · g₁ + m₂ · g₂ = (m₁ + m₂) · x

### Preis-Mischung (gleiche Logik):
| | Sorte 1 | Sorte 2 | Mischung |
|---|---|---|---|
| Menge (kg) | m₁ | m₂ | m₁ + m₂ |
| Preis/kg | p₁ | p₂ | x |
| Gesamtpreis | m₁ · p₁ | m₂ · p₂ | (m₁+m₂) · x |

### Sonderfälle:
- Wasser hat 0% Gehalt (Verdünnung)
- "Reines Kupfer" = 100% Gehalt
- Verhältnis a:b → m₁ = a·k, m₂ = b·k

---

## [T-BEWEG] Bewegung (7.8)

**Grundmenge:** G = Q⁺ bzw. Q⁺ × Q⁺

### Grundformel:
$$s = v \cdot t$$
Strecke = Geschwindigkeit × Zeit

### Muster A: Gegenfahrt (aufeinander zu)
Zwei Objekte fahren aufeinander zu:
s₁ + s₂ = Gesamtstrecke d
v₁ · t + v₂ · t = d (gleiche Zeit t)
→ t = \frac{d}{v_1 + v_2}

### Muster B: Verfolgung (Überholung)
Objekt B startet Δt später, fährt schneller:
s_A = s_B bei Überholung
v_A · t_A = v_B · t_B, wobei t_B = t_A - Δt
→ v_A · t = v_B · (t - Δt)

### Muster C: Hin und Rückfahrt
Gesamtstrecke = 2 · d
Radfahrerin A fährt schneller, wendet in B, trifft B auf dem Rückweg:
s_A + s_B = 2d

### Einheiten:
- Minuten → Stunden: ÷ 60 (z.B. 10 Min = \frac{1}{6} h)
- km/h ist Standard → alles in km/h und Stunden rechnen
- Entfernung vom Treffpunkt: s = v · t für das jeweilige Objekt

---

## [T-GEO] Geometrie (7.9)

**Grundmenge:** G = Q⁺ bzw. Q⁺ × Q⁺

### Formeln:
- Rechteck: A = l · b, U = 2(l + b)
- Quadrat: A = a², U = 4a

### Typisches Muster:
1) Original: Länge = f(x), Breite = g(x), Fläche₁ = f(x) · g(x)
2) Neu: Länge ± Δ, Breite ± Δ, Fläche₂ = (f(x) ± Δ₁)(g(x) ± Δ₂)
3) Beziehung: Fläche₂ = Fläche₁ + k oder Fläche₂ = Fläche₁

### Beispiele:
- "3-mal so lang wie breit": l = 3x, b = x
- "Verkürzt um 20 cm": l_neu = l - 20
- "Vergrössert um 20 cm": b_neu = b + 20
- Flächenvergleich: l_neu · b_neu = l · b + 800

### ⚠️ Führt oft zu quadratischer Gleichung → QT-QUAD verwenden
### ⚠️ Negative Lösung fällt weg (Länge kann nicht negativ sein)

---

## [T-DIV] Diverses (7.10)

**Grundmenge:** Hängt von Aufgabe ab

### Muster A: Kosten pro Person bei Teilnehmeränderung
- Gesamtkosten fix = G
- Geplant: x Personen, Kosten/Person = \frac{G}{x}
- Effektiv: (x - n) Personen, Kosten/Person = \frac{G}{x - n}
- Beziehung: \frac{G}{x-n} = \frac{G}{x} \cdot 1.2 (z.B. 20% mehr)
- → Bruchgleichung (QT-BRUCH)

### Muster B: Treppe/Stufen
- H = Anzahl Stufen × Höhe pro Stufe
- Gleiche Gesamthöhe bei weniger/mehr Stufen mit anderer Stufenhöhe
- n₁ · h₁ = n₂ · h₂

### Muster C: Einkauf (Preis × Menge = Total)
- Gesamtbetrag fix = G
- Original: Preis p, Menge = \frac{G}{p}
- Neu: Preis (p - Δ), Menge = \frac{G}{p - Δ} = \frac{G}{p} + n
- → Bruchgleichung

### Muster D: Geldvergleich/Schenkung
- Person A: x CHF, Person B: y CHF
- "Wenn A gibt B k CHF": A hat (x-k), B hat (y+k)
- Beziehung aufstellen → Gleichungssystem

### Muster E: Zwei Produkte (Kalender/Poster, Hemden, Orangen)
- Preis₁ · Menge₁ + Preis₂ · Menge₂ = Gesamtkosten
- Zweite Bedingung → zweite Gleichung
- → Gleichungssystem (QT-EQ2)

---

## [X-TRAP] Häufige Fehler — VERMEIDE DIESE

### Allgemein:
- ❌ D (Definitionsmenge) vergessen → Punktabzug!
- ❌ Antwortsatz vergessen → Punktabzug!
- ❌ Tabelle nicht aufgestellt → Punkte verschenkt!
- ❌ Einheiten im Antwortsatz fehlen (CHF, Jahre, km, cm, %, Liter)

### Zins (T-ZINS):
- ❌ Marchzins: M/12 oder t/360 vergessen
- ❌ "Prozentpunkte" mit "Prozent" verwechselt
  - "um 0.5 Prozentpunkte höher" → p + 0.5
  - "um 50% höher" → p · 1.5
- ❌ Bei Zinseszins: Zins des 1. Jahres NICHT zum Kapital addiert
- ❌ Einzahlung/Abhebung: Zeitpunkt falsch (NACH Zinsgutschrift!)

### Alter (T-ALTER):
- ❌ "5-mal so alt" als Addition statt Multiplikation gelesen
- ❌ Zeitverschiebung nur bei einer Person angewendet (BEIDE!)

### Verteilung (T-VERT):
- ❌ "Ein Drittel weniger" = \frac{2}{3}x (NICHT x - \frac{1}{3})
- ❌ "20% weniger als x" = 0.8x (NICHT x - 20)
- ❌ Summe der Anteile ≠ Gesamtbetrag (Kontrolle!)

### Mischung (T-MISCH):
- ❌ Wasser = 0% Gehalt vergessen
- ❌ Reinmenge statt Gehalt in Gleichung

### Bewegung (T-BEWEG):
- ❌ Minuten und Stunden gemischt (alles in h!)
- ❌ Gegenfahrt vs. Verfolgung verwechselt (+ vs. =)

### Geometrie (T-GEO):
- ❌ Negative Lösung nicht ausgeschlossen
- ❌ Ausmultiplizieren fehlerhaft bei (a+b)(c+d)

---

## [X-FORMELN] Formelsammlung (LaTeX)

### Zins:
$$Z_{Jahr} = \frac{K \cdot p}{100}$$
$$Z_{Monat} = \frac{K \cdot p \cdot M}{100 \cdot 12}$$
$$Z_{Tag} = \frac{K \cdot p \cdot t}{100 \cdot 360}$$

### Quadratische Gleichung (abc-Formel):
$$x_{1,2} = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

### Geometrie:
$$A_{Rechteck} = l \cdot b$$
$$U_{Rechteck} = 2(l + b)$$
$$A_{Quadrat} = a^2$$

### Bewegung:
$$s = v \cdot t$$

### Bruchrechnung:
$$\frac{a}{b} + \frac{c}{d} = \frac{ad + bc}{bd}$$

---

## [X-GLOSSAR] Deutsche Mathe-Begriffe

| Begriff | Bedeutung |
|---|---|
| Definitionsmenge (D) | Erlaubte Werte für x |
| Grundmenge (G) | Zahlenbereich (N, Z, Q, R) |
| Gleichung aufstellen | Mathematische Beziehung formulieren |
| Ausmultiplizieren | Klammern auflösen: a(b+c) = ab + ac |
| Zusammenfassen | Gleiche Terme vereinen |
| Hauptnenner (HN) | Kleinster gemeinsamer Nenner |
| Kehrwert | \frac{a}{b} → \frac{b}{a} |
| Stellenwert | Position einer Ziffer (Einer, Zehner, Hunderter) |
| Marchzins | Zins für weniger als 1 Jahr |
| Prozentpunkte | Absolute Änderung des Zinssatzes |
| Verhältnis a:b | a zu b → \frac{a}{b} |
| Verzinst | Zins wird berechnet |
| Zinsgutschrift | Zins wird dem Konto gutgeschrieben |
| Vertauscht | Zinssätze/Werte werden getauscht |

---

**ENDE SUPER-MD — Alle Informationen für KAP 7 (ohne 7.7) sind hier enthalten.**
