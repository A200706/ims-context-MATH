# Einsetzverfahren – LGS mit 2 Variablen

Dieses Dokument beschreibt das **Einsetzverfahren** zur Lösung linearer Gleichungssysteme mit zwei Variablen.

---

## 1. Wann Einsetzverfahren?

- Wenn sich eine Gleichung leicht nach **x** oder **y** auflösen lässt.
- Besonders geeignet, wenn eine Variable **ohne Koeffizient** auftritt:
  - z.B. `x = 3y − 2` oder `y = 5 − 2x`.

---

## 2. Standardschema

Bei einem Gleichungssystem

```text
(1) ...
(2) ...


wird im Einsetzverfahren immer nach folgendem Schema gearbeitet:

D: ...

Schritt 1
Gleichungen aufschreiben:
(1) ...
(2) ...

Schritt 2
Eine Gleichung nach x oder y auflösen:
...   [Umformungen mit [+c], [−c], [·c], [:c]]
x = ...    oder    y = ...

Schritt 3
Ausdruck in die andere Gleichung einsetzen:
...   [Einsetzen]

Schritt 4
Die entstandene Gleichung nach der verbleibenden Variablen lösen:
...   [Umformungen]

Schritt 5
Gefundene Variable in die umgestellte Gleichung einsetzen, um die andere Variable zu berechnen:
...   [Einsetzen]

Schritt 6
Lösungsmenge angeben:
L: {(x|y) = (...|...)}


Brüche immer als Wortbrüche: a/b → a btel.

3. Beispiel

Gegeben:

(1) x + y = 5
(2) x − y = 1


Lösung im Einsetzverfahren:

D: ℝ

Schritt 1
(1) x + y = 5
(2) x − y = 1

Schritt 2
(1) nach x auflösen:
x + y = 5       [−y]
x = 5 − y

Schritt 3
x in (2) einsetzen:
(2) x − y = 1
(2) (5 − y) − y = 1     [Einsetzen]

Schritt 4
Nach y lösen:
5 − y − y = 1
5 − 2y = 1              [−5]
−2y = −4                [:−2]
y = 2

Schritt 5
y in x = 5 − y einsetzen:
x = 5 − 2
x = 3

Schritt 6
L: {(x|y) = (3|2)}

4. Typische Fehlerquellen

falsches Einsetzen (falsche Gleichung oder Variable)

Vorzeichenfehler beim Vereinfachen

L ohne Klammerformat (x|y)

D vergessen bei vorherigen Nennern (falls vorhanden)
