# SUPER-MD — KAP 7 PRÜFUNG (7.2 / 7.3 / 7.4 / 7.5 / 7.10)

---

## QR — QUICK ROUTER

Lies die Aufgabe → erkenne den Typ → springe zum Block:

| Schlüsselwörter | Typ | Block |
|---|---|---|
| Zahl, Summe, Produkt, Differenz, aufeinanderfolgende | Zahlenaufgabe | T-ZAHL |
| Alter, Jahre, älter, jünger, vor … Jahren, in … Jahren | Altersaufgabe | T-ALTER |
| Kapital, Zins, Zinssatz, %, Marchzins, Guthaben, Bank | Zinsaufgabe | T-ZINS |
| verteilen, Verhältnis, aufteilen, Anteil, mehr als, doppelt | Verteilungsaufgabe | T-VERT |
| keines der obigen / gemischt / Alltagsproblem | Diverses | T-DIV |

**MODUS-CHECK** (vor dem Lösen!):
- Frage sagt "aufstellen", "Tabelle", "Gleichung formulieren", "nicht lösen" → **MODUS-TAB** (nur Tabelle + D, STOP)
- Frage sagt "lösen", "berechnen", "bestimmen", "wie viel" → **MODUS-VOLL** (Tabelle + D + Lösung + Antwortsatz)

---

## MI — MICRO INDEX

- QR: Quick Router
- QT-TAB: Tabellen-Template
- QT-EQ: Gleichung-Aufstell-Template
- QT-QUAD: Quadratische Gleichung (abc-Formel)
- T-ZAHL: Zahlenaufgaben (7.2)
- T-ALTER: Altersaufgaben (7.3)
- T-ZINS: Zinsaufgaben (7.4) ⭐ PRIORITÄT 1
- T-VERT: Verteilungsaufgaben (7.5)
- T-DIV: Diverses (7.10)
- X-TRAP: Fallen & häufige Fehler
- X-FORM: Formelsammlung
- X-GLOSS: Glossar

---

## WF — WORKFLOW (für jede Aufgabe)

```
1) 📷 OCR-Check (2–4 Wörter)
2) QR → Typ erkennen
3) Modus-Check → TAB oder VOLL?
4) Variable(n) definieren
5) QT-TAB → Tabelle aufstellen
6) D = ... (Definitionsmenge)
   --- WENN MODUS-TAB → STOP HIER ---
7) Gleichung aus Tabelle ableiten
8) Lösen (nummerierte Zeilen, [Operation])
9) L = {...}
10) Antwortsatz
```

---

## AR — ANSWER RULES

### Formatregeln (STRIKT)
- Jede Zeile: `n)` dann Inhalt
- ALLES Mathematische in LaTeX: `$...$`
- Operationen am Ende in `[...]`
- Brüche: `$\frac{a}{b}$` (nie a/b)
- Kein "Schritt", kein "Zusammenfassend", keine Meta-Texte
- Text in LaTeX: `$\text{...}$`
- Maximal 1 Gleichung/Aktion pro Zeile

### Modus-TAB (nur Tabelle + D)
- Nur: 📷 → Variablen → Tabelle → D → STOP
- Keine Lösung, kein Antwortsatz
- ~5–8 Zeilen total

### Modus-VOLL (komplette Lösung)
- 📷 → Variablen → Tabelle → D → Gleichung → Lösen → L → Antwortsatz
- ~12–25 Zeilen total

---

## QT-TAB — TABELLEN-TEMPLATE

Vertikale LaTeX-Liste (kein Markdown-Table!):

```
n) $\text{[Person/Objekt 1]:} \quad x$
n+1) $\text{[Person/Objekt 2]:} \quad 2x$
n+2) $\text{[Bedingung]:} \quad x + 2x = \text{Total}$
```

Für Zinsaufgaben:
```
n) $K_1 = x, \quad K_2 = ...$
n+1) $p_1 = ...\%, \quad p_2 = ...\%$
n+2) $t = ... \text{ Monate}$
n+3) $Z_1 = K_1 \cdot \frac{p_1}{100} \cdot \frac{t}{12}$
```

---

## QT-EQ — GLEICHUNG AUFSTELLEN

```
n) $\text{Bedingung: [in Worten]}$
n+1) $[\text{linke Seite}] = [\text{rechte Seite}]$
```

---

## QT-QUAD — QUADRATISCHE GLEICHUNG (abc-Formel)

```
n) $ax^2 + bx + c = 0$
n+1) $a = ..., \quad b = ..., \quad c = ...$
n+2) $D = b^2 - 4ac = ...$
n+3) $x_{1,2} = \frac{-b \pm \sqrt{D}}{2a}$
n+4) $x_1 = ..., \quad x_2 = ...$
n+5) Prüfe: passt $x_1$ / $x_2$ zur D?
```

---

## T-ZAHL — ZAHLENAUFGABEN (7.2)

### Typische Muster

**Zwei Zahlen, Summe + Bedingung:**
```
1) $x = \text{1. Zahl}$
2) $y = \text{2. Zahl}$
3) $\text{Summe:} \quad x + y = S$
4) $\text{Bedingung:} \quad x = 2y + k$ (o.ä.)
5) $\text{Einsetzen:} \quad (2y + k) + y = S$
```

**Aufeinanderfolgende Zahlen:**
```
1) $x = \text{1. Zahl}$
2) $x+1 = \text{2. Zahl}, \quad x+2 = \text{3. Zahl}$
3) $x + (x+1) + (x+2) = S$
```

**Ziffern einer Zahl:**
```
1) $z = \text{Zehnerziffer}, \quad e = \text{Einerziffer}$
2) $\text{Zahl} = 10z + e$
3) $\text{Umgekehrt} = 10e + z$
```

### D typisch
$D = \mathbb{R}$ oder $D = \mathbb{Z}$ oder $D = \mathbb{N}$

---

## T-ALTER — ALTERSAUFGABEN (7.3)

### Schlüssel-Prinzip
> Zeitdifferenz ist für alle Personen gleich.
> "Vor 5 Jahren" → alle minus 5. "In 3 Jahren" → alle plus 3.

### Tabellen-Setup

```
1) $x = \text{Alter von [Person] heute}$
2) $\text{[Person A] heute:} \quad x$
3) $\text{[Person B] heute:} \quad x + d$ (oder $3x$, etc.)
4) $\text{Vor } n \text{ Jahren: A} = x - n, \quad \text{B} = (x+d) - n$
5) $\text{In } m \text{ Jahren: A} = x + m, \quad \text{B} = (x+d) + m$
```

### Typische Bedingungen
- "A ist doppelt so alt wie B" → $A = 2B$
- "Vor 5 Jahren war A 3-mal so alt wie B" → $(x-5) = 3(y-5)$
- "Summe der Alter = S" → $x + y = S$
- "In 10 Jahren ist A nur noch 2-mal so alt" → $(x+10) = 2(y+10)$

### D typisch
$D = \mathbb{R}^+$ (Alter muss positiv sein)

---

## T-ZINS — ZINSAUFGABEN (7.4) ⭐ PRIORITÄT 1

### Grundformel (MARCHZINS)

$$Z = K \cdot \frac{p}{100} \cdot \frac{M}{12}$$

- $K$ = Kapital (CHF)
- $p$ = Zinssatz (%)
- $M$ = Anzahl Monate (bei Jahren: $M = 12$)
- $Z$ = Zins (CHF)

### Varianten

**Nach K auflösen:**
$$K = \frac{Z \cdot 100 \cdot 12}{p \cdot M}$$

**Nach p auflösen:**
$$p = \frac{Z \cdot 100 \cdot 12}{K \cdot M}$$

**Nach M auflösen:**
$$M = \frac{Z \cdot 100 \cdot 12}{K \cdot p}$$

### Aufgaben-Typen

**Typ 1: Zwei Kapitalien, Zinsdifferenz**
```
1) $K_1 = x, \quad K_2 = x + d$ (oder $\text{Total} - x$)
2) $Z_1 = x \cdot \frac{p_1}{100} \cdot \frac{M}{12}$
3) $Z_2 = (x+d) \cdot \frac{p_2}{100} \cdot \frac{M}{12}$
4) Bedingung: $Z_1 + Z_2 = \text{Gesamtzins}$ oder $Z_1 - Z_2 = \text{Differenz}$
```

**Typ 2: Vertauschte Zinssätze**
```
1) $\text{Fall A:} \quad Z_A = K_1 \cdot \frac{p_1}{100} \cdot \frac{M}{12} + K_2 \cdot \frac{p_2}{100} \cdot \frac{M}{12}$
2) $\text{Fall B (vertauscht):} \quad Z_B = K_1 \cdot \frac{p_2}{100} \cdot \frac{M}{12} + K_2 \cdot \frac{p_1}{100} \cdot \frac{M}{12}$
3) $Z_A - Z_B = \text{Differenz}$ (oder umgekehrt)
```

**Typ 3: Kapital + Zins nach t Jahren**
```
1) $\text{Endkapital} = K + Z$
2) $\text{Endkapital} = K + K \cdot \frac{p}{100} \cdot \frac{M}{12}$
3) $\text{Endkapital} = K \left(1 + \frac{p}{100} \cdot \frac{M}{12}\right)$
```

**Typ 4: Ein-/Auszahlung zwischen Perioden**
```
1) $\text{Nach 1. Periode:} \quad K_1 = K_0 + Z_0 \pm \text{Einzahlung}$
2) $\text{Neuer Zins:} \quad Z_1 = K_1 \cdot \frac{p}{100} \cdot \frac{M}{12}$
```

### D typisch
$D = \mathbb{R}^+$ oder $D = \mathbb{Q}^+$ (Kapital/Zins positiv)

### ⚠️ Zins-Fallen
- Monate vs. Jahre: Formel braucht MONATE → $M = 12$ für 1 Jahr!
- "Jahreszins" → $M = 12$, "Halbjahr" → $M = 6$, "Quartal" → $M = 3$
- Prozent vs. Dezimal: $p$ bleibt als %, Division durch 100 in Formel
- Vertauschte Zinssätze: Differenz-Gleichung aufstellen, nicht einzeln lösen

---

## T-VERT — VERTEILUNGSAUFGABEN (7.5)

### Schlüssel-Prinzip
> Gesamtmenge = Summe aller Anteile.
> Jeder Anteil wird durch x ausgedrückt.

### Aufgaben-Typen

**Typ 1: Verhältnis-Verteilung (a : b : c)**
```
1) $\text{Verhältnis } a : b : c$
2) $\text{A} = a \cdot k, \quad \text{B} = b \cdot k, \quad \text{C} = c \cdot k$
3) $a \cdot k + b \cdot k + c \cdot k = \text{Total}$
4) $k \cdot (a + b + c) = \text{Total}$
5) $k = \frac{\text{Total}}{a + b + c}$
```

**Typ 2: Bedingungs-Verteilung**
```
1) $x = \text{Anteil von [kleinste/Referenz]}$
2) $\text{A} = x$
3) $\text{B} = 2x$ ("doppelt so viel")
4) $\text{C} = x + 50$ ("CHF 50 mehr")
5) $x + 2x + (x + 50) = \text{Total}$
```

**Typ 3: Prozent-Verteilung**
```
1) $x = \text{Gesamtbetrag}$
2) $\text{A} = 0.30 \cdot x$ (30%)
3) $\text{B} = 0.45 \cdot x$ (45%)
4) $\text{C} = x - 0.30x - 0.45x = 0.25x$ (Rest)
5) Bedingung einsetzen und lösen
```

**Typ 4: Mischform (Verhältnis + Zusatzbedingung)**
```
1) $\text{A} = 2x, \quad \text{B} = 3x$
2) $\text{Zusatz: A bekommt CHF 100 extra}$
3) $2x + 100 + 3x = \text{Total}$
```

### D typisch
$D = \mathbb{R}^+$ (Anteile positiv) oder $D = \mathbb{Q}^+$

### ⚠️ Verteilungs-Fallen
- "Mehr als" ≠ "mal so viel": $x + 50$ vs. $50x$
- Verhältnis 2:3 heisst NICHT A=2, B=3 → A=2k, B=3k
- Gesamtmenge prüfen: Summe aller Anteile = Total?
- Einheiten: CHF, kg, Liter — konsistent bleiben

---

## T-DIV — DIVERSES (7.10)

### Schlüssel-Prinzip
> Alltagsprobleme → in Gleichung übersetzen.
> Oft Kombination aus mehreren Themen.

### Häufige Muster

**Preis/Kosten-Aufgaben:**
```
1) $x = \text{Preis pro Stück}$
2) $n \cdot x = \text{Gesamtkosten}$
3) $(n + k) \cdot (x - r) = \text{Gesamtkosten}$ (mehr Stücke, weniger pro Stück)
```

**Arbeiter/Leistung:**
```
1) $x = \text{Leistung pro Person/Stunde}$
2) $n \cdot x \cdot t = \text{Gesamtarbeit}$
```

**Gewinn/Verlust:**
```
1) $\text{Gewinn} = \text{Verkauf} - \text{Einkauf}$
2) $\text{Verkauf} = \text{Einkauf} \cdot (1 + \frac{g}{100})$
```

**Strecke/Weg (einfach):**
```
1) $s = v \cdot t$
2) $\text{Hin:} \quad s = v_1 \cdot t_1$
3) $\text{Zurück:} \quad s = v_2 \cdot t_2$
4) $t_1 + t_2 = t_{\text{total}}$
```

### D typisch
Kontextabhängig — meistens $D = \mathbb{R}^+$

---

## X-TRAP — FALLEN & HÄUFIGE FEHLER

| # | Falle | Fix |
|---|---|---|
| 1 | D vergessen | IMMER D schreiben, auch wenn offensichtlich |
| 2 | Antwortsatz vergessen | Letzter Punkt = ganzer Satz mit Einheit |
| 3 | Vorzeichen beim Auflösen | Minus × Minus = Plus! |
| 4 | Klammer nicht ausmultipliziert | Jedes Glied in der Klammer! |
| 5 | Monate vs. Jahre (Zins) | Formel braucht M (Monate), nicht Jahre |
| 6 | Prozent als Dezimal vergessen | $p\%$ → $\frac{p}{100}$ in Rechnung |
| 7 | "Mehr als" vs. "mal so viel" | $+k$ vs. $\cdot k$ — genau lesen! |
| 8 | Verhältnis falsch aufgesetzt | $2:3$ → $2k$ und $3k$, nicht $2$ und $3$ |
| 9 | Negative Lösung bei Alter/Geld | Prüfe: passt Lösung zum Kontext? |
| 10 | Tabelle nicht beschriftet | Zeilen/Spalten IMMER benennen → gibt Punkte! |

---

## X-FORM — FORMELSAMMLUNG

### Zins (Marchzins)
$$Z = K \cdot \frac{p}{100} \cdot \frac{M}{12}$$

### abc-Formel (quadratische Gleichung)
$$x_{1,2} = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

### Verhältnis
$$k = \frac{\text{Total}}{\text{Summe der Verhältnisteile}}$$

### Prozent
$$\text{Anteil} = \text{Ganzes} \cdot \frac{p}{100}$$

### Gleichung lösen — erlaubte Operationen
- $[| + a]$ → auf beiden Seiten $+a$
- $[| - a]$ → auf beiden Seiten $-a$
- $[| \cdot a]$ → auf beiden Seiten $\cdot a$
- $[| : a]$ → auf beiden Seiten $: a$ (nur wenn $a \neq 0$)

---

## X-GLOSS — GLOSSAR

| Deutsch | Mathe |
|---|---|
| Summe | $a + b$ |
| Differenz | $a - b$ |
| Produkt | $a \cdot b$ |
| Quotient | $\frac{a}{b}$ |
| aufeinanderfolgende Zahlen | $x, x+1, x+2, ...$ |
| doppelt so viel | $2x$ |
| halb so viel | $\frac{x}{2}$ |
| um k grösser | $x + k$ |
| um k kleiner | $x - k$ |
| Verhältnis a:b | $a \cdot k$ und $b \cdot k$ |
| Marchzins | $Z = K \cdot \frac{p}{100} \cdot \frac{M}{12}$ |
| Definitionsmenge D | Erlaubte Werte für $x$ |
| Lösungsmenge L | Werte, die Gleichung erfüllen |
| Antwortsatz | Ganzer Satz als Antwort |
