Hier geht es um Gleichungssysteme mit einem Parameter (z.B. a), bei denen man die Anzahl der Lösungen untersuchen soll.

---

## 1. Typische Fragestellungen

- „Für welche Werte von a hat das System genau eine Lösung?“
- „Für welche Werte von a hat das System keine Lösung?“
- „Für welche Werte von a hat das System unendlich viele Lösungen?“

---

## 2. Grundidee

1. Gleichungen in eine **klare Normalform** bringen:
   - `ax + by = c` und `dx + ey = f`
2. Ein Verfahren (meist Additions- oder Gleichsetzverfahren) anwenden.
3. Beim Rechnen entstehen Ausdrücke mit dem Parameter (z.B. `0 = 0`, `0 = 5`, Faktoren mit a).
4. Aus diesen Ausdrücken werden Fälle abgeleitet:
   - genau eine Lösung
   - keine Lösung
   - unendlich viele Lösungen

---

## 3. Standardschema

```text
D: ℝ        (sofern keine Nenner; sonst D anpassen)

Schritt 1
Gleichungen in Normalform bringen:
(1) ...
(2) ...

Schritt 2
Additions- oder Gleichsetzverfahren anwenden:
...   [Umformungen, abhängig von a]

Schritt 3
Fallunterscheidung nach a:
- Fall 1: Ausdruck enthält Nenner/Faktor ≠ 0 → genau eine Lösung
- Fall 2: Widerspruch wie 0 = k (k ≠ 0) → keine Lösung
- Fall 3: wahre Aussage 0 = 0 und Gleichungen Vielfache → unendlich viele Lösungen

Schritt 4
L entsprechend angeben:
- bei einer Lösung: L: {(x|y) = (...|...)} (ggf. abhängig von a)
- bei keiner Lösung: L: ∅
- bei unendlich vielen Lösungen: L: unendlich viele Lösungen
4. Beispiel (Konzept)
Gegeben:

text
Code kopieren
(1) x + ay = 2
(2) 2x + 2ay = 4
Lösungsstruktur:

text
Code kopieren
D: ℝ

Schritt 1
(1) x + ay = 2
(2) 2x + 2ay = 4

Schritt 2
(2) ist 2 · (1):
2x + 2ay = 4     ⇔     2(x + ay) = 4

Schritt 3
Fallunterscheidung:
- Für alle a gilt: (2) ist Vielfaches von (1) und keine Widersprüche.
→ unendlich viele Lösungen (Geraden identisch).

Schritt 4
L: unendlich viele Lösungen
(z.B. in Parameterform beschreibbar)
Konkrete Fälle sind aufgabenabhängig; das Schema ist immer gleich: Normalform, Verfahren, Fälle.
