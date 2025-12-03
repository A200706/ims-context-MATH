Hier geht es um Gleichungssysteme, in denen Variablen im Nenner stehen, z.B. `1/(x − 3)` oder `2/y`.

---

## 1. Grundidee

1. **Definitionsmenge D bestimmen:**
   - Alle Ausdrücke im Nenner dürfen **nicht 0** sein.
   - Diese Bedingungen werden in D gesammelt.

2. **Nenner entfernen:**
   - Einen gemeinsamen **Hauptnenner (HN)** bestimmen.
   - Alle Gleichungen mit dem HN multiplizieren.
   - Danach ist das System ohne Nenner.

3. **Normales Verfahren anwenden:**
   - Einsetz-, Gleichsetz- oder Additionsverfahren.
   - Standard: Additionsverfahren, wenn möglich.

---

## 2. Standardschema

```text
D: ℝ \ {verbotene Werte}

Schritt 1
Gleichungssystem hinschreiben, Nenner erkennen.

Schritt 2
Hauptnenner bestimmen und alle Gleichungen mit HN multiplizieren:
...   [·HN]

Schritt 3
Entstandenes Gleichungssystem (ohne Nenner) vereinfachen.

Schritt 4
Mit Einsetz-, Gleichsetz- oder Additionsverfahren lösen.

Schritt 5
Lösungsmenge angeben und prüfen, ob Lösung mit D verträglich ist.
Wenn Lösung gegen D verstößt:
L: ∅
3. Beispiel (Schema)
Gleichungssystem (nur als Struktur, nicht konkrete Zahlen):

text
Code kopieren
(1) 1/(x − 2) + y = 3
(2) 2/(x − 2) − y = 1
Lösungsstruktur:

text
Code kopieren
D: ℝ \ {2}

Schritt 1
(1) 1/(x − 2) + y = 3
(2) 2/(x − 2) − y = 1

Schritt 2
HN = (x − 2)
(1) mit (x − 2) multiplizieren:
1 + y(x − 2) = 3(x − 2)        [·(x − 2)]
(2) mit (x − 2) multiplizieren:
2 − y(x − 2) = 1(x − 2)        [·(x − 2)]

Schritt 3
System ohne Nenner aufschreiben:
(1') ...
(2') ...

Schritt 4
(1') und (2') mit passendem Verfahren (oft Additionsverfahren) lösen.

Schritt 5
Ergebnis prüfen:
- darf x nicht 2 sein
- falls x = 2 resultiert, ist L: ∅
- sonst Lösung in der Form L: {(x|y) = (...|...)}
4. Typische Fehlerquellen
D nicht oder falsch angegeben

falscher Hauptnenner

vergessen, alle Terme mit HN zu multiplizieren

gefundene Lösung verletzt D (z.B. x = 2, obwohl x ≠ 2)
