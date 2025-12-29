# IMS Math – Kapitel 6: Quadratische Gleichungen (SUPER Truth File)
Version: 1.0 (für 7-Cal / OCR / Prüfungsstil)

Dieses Dokument ist absichtlich **lang**, aber **hart strukturiert**, damit eine AI schnell springen kann.
Regel: **Wenn etwas hier steht und dein “Standard-Mathe-Stil” anders ist: dieses File gewinnt.**

============================================================
SECTION 0 — 7-CAL WORKFLOW (BILD ODER TEXT)
============================================================

0.1 Input
- Wenn Aufgabe kurz ist: Text eintippen.
- Wenn Aufgabe lang/mit Graph/mehrteilig: Foto (gerade, nah, scharf, guter Kontrast).

0.2 Immer zuerst:
- Aufgabe lesen (aus Bild/Text).
- Entscheiden: **Gleichung** oder **Textaufgabe**.
- Prüfen ob **Nenner** oder **Wurzeln** Einschränkungen geben → dann **D** setzen.

0.3 Ergebnis-Check (Pflicht)
- Jede gefundene Lösung **einsetzen** (kurz), ob sie die Ausgangsgleichung erfüllt.
- Wenn D Einschränkungen hat: Lösung muss D erfüllen, sonst raus.

============================================================
SECTION 1 — LEHRER-STIL OUTPUT (SEHR STRICT)
============================================================

1.1 Output ist PLAIN TEXT
- **Kein LaTeX**, kein Markdown in der Ausgabe.
- Keine Sätze/Erklärtexte. Nur: D, Schritte, Gleichungen, Operation-Tags, L.

1.2 Definitionsmenge
Ganz am Anfang:
D: ...

- Wenn keine Einschränkungen: D: R
- Wenn Nenner: Nenner ≠ 0 → Werte ausschliessen
  Beispiel: D: R \ {3}
- Wenn Wurzel (√): Radikand ≥ 0 (falls reell verlangt)
  Beispiel: D: {x ∈ R | x-5 ≥ 0}

1.3 Schritte
- Jeder Schritt hat genau:
Schritt 1
<Zeile(n)>

Schritt 2
<Zeile(n)>

- “Schritt n” = immer **neue Zeile / Absatz**.
- Keine Nummerierung im Text, nur “Schritt 1/2/3…”.

1.4 Umformungen markieren
- Jede Umformung bekommt am Zeilenende einen Tag in eckigen Klammern:
  [+2]   [-y]   [·3]   [:2]   [√]   [^2]   [p-q]   [a=1] etc.
- Keine Sätze wie “wir addieren 2”. Nur Tags.

Beispiel:
x - 2 = 7   [+2]
x = 9

1.5 Bruch-Darstellung (Wortbruch)
- Niemals “a/b” schreiben.
- Immer Wortbruch: “a btel”
  7/10  -> 7 10tel
  1/2   -> 1 2tel
  x/3   -> x 3tel
- Wenn Zähler oder Nenner ein ganzer Term ist: immer Klammern:
  (2x-1) 3tel   bedeutet (2x-1)/3
  (a+b) (2c)tel bedeutet (a+b)/(2c)

1.6 Lösung am Schluss
- Immer:
L: {(x1, x2)}  oder bei zwei Variablen: L: {(x|y) = (...|...)}
Hier (quadratisch) typisch:
L: {x1 = ..., x2 = ...}
oder wenn nur eine Lösung:
L: {x = ...}
oder:
L: ∅

============================================================
SECTION 2 — ERKENNEN: “IST DAS QUADRATISCH?”
============================================================

2.1 Quadratische Gleichung (Standard)
- höchste Potenz ist 2:
  ax^2 + bx + c = 0   (a ≠ 0)

2.2 Häufige Formen
- Normalform: ax^2 + bx + c = 0
- Schon faktorisiert: (x - p)(x - q) = 0
- Quadratisch in Klammern: (x+2)^2 = 9
- Brüche / Nenner: 1/(x-3) = x  → erst D, dann Nenner weg

2.3 Ziel immer:
- Auf eine Form bringen, die man sauber lösen kann:
  - faktorisiert (Nullprodukt)
  - (x+d)^2 = k (Wurzel ziehen)
  - x^2 + px + q = 0 (pq-Formel)
  - ax^2 + bx + c = 0 (Mitternachtsformel)

============================================================
SECTION 3 — METHODEN (80/20, aber vollständig)
============================================================

------------------------------------------------------------
3A) Nullprodukt (Faktorisieren) – wenn möglich, ist das am schnellsten
------------------------------------------------------------

Typ:
x^2 + px + q = 0  und man findet zwei Zahlen r,s mit:
r + s = p   und   r·s = q
Dann:
(x + r)(x + s) = 0

Template Output:
D: R
Schritt 1
x^2 + px + q = 0
(x + r)(x + s) = 0   [fakt]
Schritt 2
x + r = 0   [Nullprod]
x + s = 0   [Nullprod]
Schritt 3
x = -r
x = -s
L: {x1 = -r, x2 = -s}

Schnell-Check (typisch):
- q positiv → r,s gleiches Vorzeichen
- q negativ → r,s verschiedene Vorzeichen

------------------------------------------------------------
3B) Wurzelziehen – wenn (x+d)^2 = k
------------------------------------------------------------

Typ:
(x + d)^2 = k

Rules:
- Wenn k < 0 und reell gefragt → keine Lösung
- Sonst:
x + d = ±√k

Template:
D: R  (oder mit Bedingungen falls)
Schritt 1
(x + d)^2 = k
x + d = √k   [√]
x + d = -√k  [√]
Schritt 2
x = √k - d   [-d]
x = -√k - d  [-d]
L: {x1 = ..., x2 = ...}

------------------------------------------------------------
3C) pq-Formel – wenn a=1 (x^2 + px + q = 0)
------------------------------------------------------------

Form:
x^2 + px + q = 0

Formel in Wortbruch:
x = (-p 2tel) ± √( (p 2tel)^2 - q )

Template:
D: R
Schritt 1
x^2 + px + q = 0
p = ...
q = ...
Schritt 2
x = (-p 2tel) + √( (p 2tel)^2 - q )   [pq]
x = (-p 2tel) - √( (p 2tel)^2 - q )   [pq]
Schritt 3
x = ...  [rechnen]
x = ...  [rechnen]
L: {x1 = ..., x2 = ...}

Fehlerquellen:
- p ist der Koeffizient von x, nicht von x^2
- Vorzeichen von q
- (p/2)^2 richtig

------------------------------------------------------------
3D) Mitternachtsformel – allgemein (ax^2 + bx + c = 0)
------------------------------------------------------------

Form:
ax^2 + bx + c = 0   (a ≠ 0)

Diskriminante:
Δ = b^2 - 4ac

Lösungen:
x = (-b ± √Δ) (2a)tel

Template:
D: R  (oder mit Bedingungen)
Schritt 1
ax^2 + bx + c = 0
a = ...
b = ...
c = ...
Schritt 2
Δ = b^2 - 4·a·c   [Δ]
Δ = ...           [rechnen]
Schritt 3
x = (-b + √Δ) (2a)tel   [Mitternacht]
x = (-b - √Δ) (2a)tel   [Mitternacht]
Schritt 4
x = ...   [rechnen]
x = ...   [rechnen]
L: {x1 = ..., x2 = ...}

Δ-Fälle:
- Δ > 0 → 2 reelle Lösungen
- Δ = 0 → 1 reelle Lösung (Doppelwurzel)
- Δ < 0 → keine reelle Lösung → L: ∅ (falls nur R)

------------------------------------------------------------
3E) Quadratische Ergänzung (Komplettierung) – wenn verlangt oder als Plan B
------------------------------------------------------------

Typ:
x^2 + px = -q  (oder nach umformen)

Methode:
- p halbieren → (p 2tel)
- (p 2tel)^2 hinzufügen auf beiden Seiten

Template:
D: R
Schritt 1
x^2 + px + q = 0   [umf]
x^2 + px = -q      [-q]
Schritt 2
x^2 + px + (p 2tel)^2 = -q + (p 2tel)^2   [+ (p 2tel)^2]
Schritt 3
(x + p 2tel)^2 = -q + (p 2tel)^2   [binom]
Schritt 4
x + p 2tel = ±√( -q + (p 2tel)^2 )   [√]
Schritt 5
x = -p 2tel ± √( -q + (p 2tel)^2 )   [-p 2tel]
L: {x1 = ..., x2 = ...}

============================================================
SECTION 4 — “VARIABLEN IM NENNER” (DANN IST ES OFT QUADRATISCH)
============================================================

Typ:
1/(x-3) = x
oder
(2)/(x) + 1 = 3x

Rules:
- Erst D: Nenner ≠ 0
- Dann Hauptnenner (HN) multiplizieren
- Dann normal umformen (oft quadratisch)

Template:
D: R \ {3}
Schritt 1
1 (x-3)tel = x   [gegeben]
Schritt 2
1 = x(x-3)   [·HN]
Schritt 3
1 = x^2 - 3x
0 = x^2 - 3x - 1   [-1]
Schritt 4
... (pq oder Mitternacht)
Schritt 5
L: {x1 = ..., x2 = ...}   [D check]

D-Check:
- Jede Lösung einsetzen: wenn verbotener Wert → streichen

============================================================
SECTION 5 — PARAMETER-AUFGABEN (a,b,c sind nicht nur Zahlen)
============================================================

Typ:
ax^2 + bx + c = 0, aber a/b/c enthalten Parameter (z.B. k)

Ziel:
- Bedingungen an Parameter für:
  - 2 Lösungen / 1 Lösung / keine Lösung

Standard:
Δ(k) = b(k)^2 - 4·a(k)·c(k)

Dann:
- Δ(k) > 0 → 2 Lösungen
- Δ(k) = 0 → 1 Lösung
- Δ(k) < 0 → ∅

Template (nur Struktur, AI soll konkret rechnen):
D: R  (plus Einschränkungen falls)
Schritt 1
a(k) x^2 + b(k) x + c(k) = 0
Schritt 2
Δ(k) = b(k)^2 - 4·a(k)·c(k)   [Δ]
Δ(k) = ...                    [ausmult]
Schritt 3
Δ(k) > 0   [2L]
Δ(k) = 0   [1L]
Δ(k) < 0   [0L]
Schritt 4
k-Bedingungen lösen (Ungleichungen)
L: ...
(Optional: x-Lösungen für bestimmte k)

============================================================
SECTION 6 — PRÜFUNG: TYPISCHE AUFGABENFORMEN (WAS KOMMT WIRKLICH?)
============================================================

High ROI Aufgaben (sehr wahrscheinlich):
1) “Löse: ax^2 + bx + c = 0” (Mitternacht oder pq)
2) “In Normalform bringen und lösen” (Klammern, Brüche, Verschieben)
3) “Faktorisieren und Nullprodukt” (wenn einfache Zahlen)
4) “(x+d)^2 = k” (Wurzelziehen)
5) “Parameter: wann 0/1/2 Lösungen?” (Δ-Check)

Medium ROI:
- Textaufgabe (Fläche, Weg, Zeit) führt auf Quadratik
- “Überprüfe Lösung” / “setze ein”

============================================================
SECTION 7 — 16-ZEICHEN PRO ZEILE (DEIN TASCHENRECHNER-LIFE)
============================================================

Wenn Ausgabe auf 16 Zeichen pro Zeile zerbricht:
- Wichtig ist die Reihenfolge, nicht das Layout.
- Du schreibst es sauber ins Heft, nicht 1:1 vom Display.

Tricks:
- Kurze Variablen: x, k
- Klammern sparsam, aber korrekt
- Lange Zeilen aufteilen:
  Statt: x = (-b + √Δ) (2a)tel
  Schreib in 2 Zeilen:
  x = (-b+√Δ)
  (2a)tel

============================================================
SECTION 8 — FOTO/OCR TIPS (DAMIT ES NICHT WIEDER 3.8 WIRD)
============================================================

- Kamera parallel zum Blatt, nicht schräg.
- Licht von der Seite, keine Spiegelung.
- Schneide alles Unnötige weg (nur Aufgabe).
- Wenn mehrere Teilaufgaben: lieber 2 Bilder statt 1 riesiges.
- Bei Brüchen: so nah, dass “-” und “+” klar sind.

============================================================
SECTION 9 — MINI-CHEAT SHEET (FÜR DICH)
============================================================

1) Immer D zuerst.
2) Immer auf 0 bringen (… = 0).
3) Schnell entscheiden:
   - faktorisiert? → Nullprodukt
   - (x+d)^2 = k? → √
   - a=1? → pq
   - sonst → Mitternacht
4) Δ entscheidet Anzahl Lösungen.
5) Am Ende: L sauber + D-Check.

Ende.

