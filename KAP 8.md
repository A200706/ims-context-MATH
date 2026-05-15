# SUPER-MD — KAP 8 PRÜFUNG (8.1–8.11)
# Potenzen: Vereinfachen & Umformen (LaTeX-SAFE)

---

## 0) Output-Style (LaTeX-SAFE)

Wenn ein Viewer LaTeX nur dann rendert, wenn die ZEILE komplett LaTeX ist, benutze dieses Template:

- Jede Ausgabelinie ist GENAU ein LaTeX-Block:
  - beginnt mit `$`
  - endet mit `$`
- Nummerierung steht IN LaTeX:
  - `\text{1) }`, `\text{2) }`, ...
- Wörter/Hinweise IMMER in `\text{...}`
- Hinweise am Ende als `\text{[| ...]}`
- Keine Unicode-Hochzahlen (⁴), nur LaTeX: `x^4`, `x^{-2}`

### Beispiel (Multiplikation gleiche Basis)

$\text{1) OCR: } x^4 \cdot x^3 \cdot x^{-2}$

$\text{2) } = x^{4+3+(-2)}\ \text{[| Exp. addieren]}$

$\text{3) } = x^5$

---

## 1) Potenzgesetze (Kernstoff)

1. $a^0 = 1$ (für $a \neq 0$)
2. $a^1 = a$
3. $a^m \cdot a^n = a^{m+n}$
4. $\frac{a^m}{a^n} = a^{m-n}$
5. $(a^m)^n = a^{m\cdot n}$
6. $a^n \cdot b^n = (ab)^n$
7. $\frac{a^n}{b^n} = \left(\frac{a}{b}\right)^n$
8. $a^{-n} = \frac{1}{a^n}$

---

## 2) Quick Router (8.1–8.11)

- 8.1 Add/Sub: nur gleiche Basis UND gleicher Exponent.
- 8.2 Multiplikation (gleiche Basis): Exponenten addieren.
- 8.3 Division (gleiche Basis): Exponenten subtrahieren.
- 8.4 Potenz von Potenz: Exponenten multiplizieren.
- 8.5 Gleicher Exponent im Bruch: $(\frac{a}{b})^n$.
- 8.6/8.7 Brüche: bei Division Kehrwert.
- 8.8/8.9 Parameter im Exponenten: Klammern korrekt auflösen.
- 8.10 Klammern potenzieren: jeden Faktor potenzieren.
- 8.11 Multiple Choice: jede Option einzeln prüfen.

---

## 3) Workflow (pro Aufgabe)

1. OCR-Zeile
2. Passende Regel anwenden
3. Exponenten korrekt zusammenfassen
4. Endergebnis

---

## 4) Beispiele pro Typ

### 8.1 (Add/Sub)
$\text{1) OCR: } 5x^3 + 2x^3 - 4x^3$

$\text{2) } = (5+2-4)\cdot x^3\ \text{[| Koeff. zusammenfassen]}$

$\text{3) } = 3x^3$

### 8.3 (Division mit negativem Exponenten)
$\text{1) OCR: } \frac{x^2}{x^7}$

$\text{2) } = x^{2-7}\ \text{[| Exp. subtrahieren]}$

$\text{3) } = x^{-5}$

$\text{4) } = \frac{1}{x^5}\ \text{[| negativer Exp.]}$

### 8.8/8.9 (Parameter)
$\text{1) OCR: } \frac{x^{2n+3}}{x^{n+1}}$

$\text{2) } = x^{(2n+3)-(n+1)}\ \text{[| Exp. subtrahieren]}$

$\text{3) } = x^{2n+3-n-1}\ \text{[| Klammer auflösen]}$

$\text{4) } = x^{n+2}$

### 8.10 (Klammern)
$\text{1) OCR: } (a^n \cdot b^{n+1})^3$

$\text{2) } = a^{n\cdot 3} \cdot b^{(n+1)\cdot 3}\ \text{[| jeden Faktor potenzieren]}$

$\text{3) } = a^{3n} \cdot b^{3n+3}$

### 8.11 (Multiple Choice)
$\text{1) OCR: } \text{Welche Aussage ist korrekt?}$

$\text{2) A)}\ a^{3+4}=a^7 \neq a^{12}\ \text{[| FALSCH]}$

$\text{3) B)}\ a^{3+4}=a^7\ \text{[| KORREKT]}$

$\text{4) C)}\ a^{3\cdot 4}=a^{12} \neq a^7\ \text{[| FALSCH]}$

$\text{5) D)}\ a^0=1 \neq 0\ \text{[| FALSCH]}$

$\text{6) Antwort: }\text{B}$

---

## 5) Häufige Fehler (Fallen)

- $a^2 + a^3$ ist NICHT $a^5$.
- $a^2 \cdot a^3 = a^5$ (Exponenten addieren).
- $(a^2)^3 = a^6$ (Exponenten multiplizieren).
- $(2a)^3 = 8a^3$ (Koeffizient mitpotenzieren).
- Bei Parametern Minus durchziehen: $(n+3)-(n-1)=n+3-n+1=4$.
