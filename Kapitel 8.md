# SUPER-MD — KAP 8 PRÜFUNG (8.1 – 8.11)
# Potenzen: Vereinfachen & Umformen

---

## QR — QUICK ROUTER

Lies den Ausdruck → erkenne den Typ → wende die Regel an:

| Muster im Foto | Typ | Regel |
|---|---|---|
| Gleiche Basis, gleicher Exponent, + oder − | T-ADD | Koeffizienten addieren/subtrahieren |
| Gleiche Basis, verschiedene Exponenten, · | T-MUL | Exponenten addieren |
| Gleiche Basis, verschiedene Exponenten, : oder Bruch | T-DIV | Exponenten subtrahieren |
| Potenz hoch Potenz: $(a^m)^n$ | T-POT | Exponenten multiplizieren |
| Gleicher Exponent, verschiedene Basen, · | T-MUL-B | Basen multiplizieren |
| Gleicher Exponent, verschiedene Basen, : | T-DIV-B | Basen dividieren |
| Bruch mit Potenzen | T-BRUCH | Zähler/Nenner separat, dann kürzen |
| Parameter im Exponenten (n, m, k) | T-PARAM | Normale Regeln, Exponenten algebraisch vereinfachen |
| Klammern mit Potenzen | T-KLAM | Klammer zuerst, dann potenzieren |
| Multiple Choice (richtig/falsch) | T-MC | Jede Option prüfen |

---

## PG — POTENZGESETZE (8 Kernregeln)

### Regel 1: Exponent 0
$$a^0 = 1 \quad (a \neq 0)$$

### Regel 2: Exponent 1
$$a^1 = a$$

### Regel 3: Multiplikation (gleiche Basis)
$$a^m \cdot a^n = a^{m+n}$$
> Exponenten ADDIEREN

### Regel 4: Division (gleiche Basis)
$$\frac{a^m}{a^n} = a^{m-n}$$
> Exponenten SUBTRAHIEREN

### Regel 5: Potenz einer Potenz
$$(a^m)^n = a^{m \cdot n}$$
> Exponenten MULTIPLIZIEREN

### Regel 6: Multiplikation (gleicher Exponent)
$$a^n \cdot b^n = (a \cdot b)^n$$
> Basen MULTIPLIZIEREN

### Regel 7: Division (gleicher Exponent)
$$\frac{a^n}{b^n} = \left(\frac{a}{b}\right)^n$$
> Basen DIVIDIEREN

### Regel 8: Negativer Exponent
$$a^{-n} = \frac{1}{a^n}$$
> Kehrwert bilden

---

## T-ADD — ADDITION/SUBTRAKTION (8.1)

### Kernregel
> NUR gleiche Basis UND gleicher Exponent können addiert/subtrahiert werden.

### Beispiele
```
3a² + 5a² = 8a²              ✓ (gleich)
3a² + 5a³ = 3a² + 5a³        ✗ (versch. Exponenten → nicht vereinfachbar)
3a² + 5b² = 3a² + 5b²        ✗ (versch. Basen → nicht vereinfachbar)
2x³y² - 5x³y² = -3x³y²       ✓ (alles gleich)
```

---

## T-MUL — MULTIPLIKATION GLEICHE BASIS (8.2)

### Kernregel
$$a^m \cdot a^n = a^{m+n}$$

### Beispiele
```
x³ · x⁵ = x⁸
a² · a⁻³ = a⁻¹ = 1/a
2a³ · 3a² = 6a⁵
(-2x²)·(3x⁴) = -6x⁶
```

---

## T-DIV — DIVISION GLEICHE BASIS (8.3)

### Kernregel
$$\frac{a^m}{a^n} = a^{m-n}$$

### Spezialfälle
```
a^m : a^m = a^0 = 1
a^3 : a^5 = a^{-2} = 1/a²
```

### Beispiele
```
x⁷ : x³ = x⁴
a⁵/a² = a³
12x⁶/(4x²) = 3x⁴
a³/a⁵ = a⁻² = 1/a²
```

---

## T-POT — POTENZIEREN (8.4)

### Kernregel
$$(a^m)^n = a^{m \cdot n}$$

### Beispiele
```
(x³)⁴ = x¹²
(a⁻²)³ = a⁻⁶ = 1/a⁶
(2x³)² = 4x⁶         ← Koeffizient auch potenzieren!
(-3a²)³ = -27a⁶      ← Vorzeichen beachten!
```

### Vorzeichen-Regel
```
(-a)^gerade = +a^n
(-a)^ungerade = -a^n
```

---

## T-DIV-B — DIVISION GLEICHER EXPONENT (8.5)

### Kernregel
$$\frac{a^n}{b^n} = \left(\frac{a}{b}\right)^n$$

### Beispiele
```
x⁴/y⁴ = (x/y)⁴
8a³/(2a)³ = 8a³/8a³ = 1
```

---

## T-BRUCH — BRÜCHE MIT POTENZEN (8.6, 8.7)

### Multiplikation (8.6)
$$\frac{a^m}{b^n} \cdot \frac{c^p}{d^q} = \frac{a^m \cdot c^p}{b^n \cdot d^q}$$

### Division (8.7)
$$\frac{a^m}{b^n} : \frac{c^p}{d^q} = \frac{a^m \cdot d^q}{b^n \cdot c^p}$$

### Beispiele
```
(a³/b²) · (a²/b) = a⁵/b³
(x⁴/y³) : (x²/y) = x²/y²
```

---

## T-PARAM — PARAMETER IM EXPONENTEN (8.8, 8.9)

### Kernprinzip
> Gleiche Regeln, aber Exponenten enthalten Variablen (n, m, k).

### Beispiele Multiplikation (8.8)
```
a^{n+2} · a^{3-n} = a^{(n+2)+(3-n)} = a^5
x^{2m} · x^{3m+1} = x^{5m+1}
```

### Beispiele Division (8.9)
```
a^{n+3}/a^{n-1} = a^{(n+3)-(n-1)} = a^{n+3-n+1} = a^4
x^{2n+1}/x^{n+2} = x^{n-1}
```

### ⚠️ Häufiger Fehler
```
(n+3) - (n-1) = n+3-n+1 = 4     ✓
(n+3) - (n-1) = n+3-n-1 = 2     ✗ (Minus nicht durchgezogen!)
```

---

## T-KLAM — KLAMMERN POTENZIEREN (8.10)

### Kernregel
$$(a^m \cdot b^n)^p = a^{m \cdot p} \cdot b^{n \cdot p}$$

### Beispiele
```
(2a³b²)⁴ = 16a¹²b⁸
(x²y⁻¹)³ = x⁶y⁻³ = x⁶/y³
(a^n · b^{n+1})² = a^{2n} · b^{2n+2}
```

---

## T-MC — MULTIPLE CHOICE (8.11)

### Strategie
```
1) Jede Option einzeln prüfen
2) Potenzgesetz anwenden
3) Vergleichen: Stimmt links = rechts?
4) Antwort: "Korrekt: A, C" oder "Falsch: B"
```

### Typische Fallen
```
a² + a³ = a⁵           ✗ FALSCH (Addition ≠ Multiplikation!)
a² · a³ = a⁶           ✗ FALSCH (Exp. addieren: 2+3=5)
(a²)³ = a⁵             ✗ FALSCH (Exp. multiplizieren: 2·3=6)
a⁰ = 0                 ✗ FALSCH (a⁰ = 1)
a⁻² = -a²              ✗ FALSCH (a⁻² = 1/a²)
```

---

## X-TRAP — FALLEN & HÄUFIGE FEHLER

| # | Falle | Falsch | Richtig |
|---|---|---|---|
| 1 | Addition vs. Multiplikation | $a^2 + a^3 = a^5$ | nicht vereinfachbar |
| 2 | Exponenten bei · | $a^2 \cdot a^3 = a^6$ | $a^5$ |
| 3 | Exponenten bei Potenz | $(a^2)^3 = a^5$ | $a^6$ |
| 4 | Exponent 0 | $a^0 = 0$ | $a^0 = 1$ |
| 5 | Negativer Exponent | $a^{-2} = -a^2$ | $\frac{1}{a^2}$ |
| 6 | Vorzeichen potenzieren | $(-2)^3 = 8$ | $-8$ |
| 7 | Koeffizient vergessen | $(2a)^3 = 2a^3$ | $8a^3$ |
| 8 | Minus in Klammer | $(n+1)-(n-1) = 0$ | $= 2$ |

---

## X-FORM — FORMELSAMMLUNG

| # | Name | Formel |
|---|---|---|
| 1 | Exponent 0 | $a^0 = 1$ |
| 2 | Exponent 1 | $a^1 = a$ |
| 3 | Mult. (gl. Basis) | $a^m \cdot a^n = a^{m+n}$ |
| 4 | Div. (gl. Basis) | $\frac{a^m}{a^n} = a^{m-n}$ |
| 5 | Potenz einer Potenz | $(a^m)^n = a^{m \cdot n}$ |
| 6 | Mult. (gl. Exponent) | $a^n \cdot b^n = (ab)^n$ |
| 7 | Div. (gl. Exponent) | $\frac{a^n}{b^n} = (\frac{a}{b})^n$ |
| 8 | Negativer Exponent | $a^{-n} = \frac{1}{a^n}$ |

---

## AR — ANSWER RULES

### Formatregeln
1) Jede Zeile: `n)` dann Inhalt
2) ALLES in LaTeX: `$...$`
3) Hinweise am Ende: `[| ...]`
4) Brüche: `$\frac{a}{b}$`
5) 1 Umformung pro Zeile
6) KEIN "Schritt", KEIN "Also"
7) Letzte Zeile = Endergebnis
