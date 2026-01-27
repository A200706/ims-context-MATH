---
# Super MD: Kapitel 6 & 7 — Quadratische Gleichungen & Textaufgaben

---

## **1. Übersicht & Struktur**
Dieses Dokument dient als zentrales Nachschlagewerk für die Kapitel 6 (Quadratische Gleichungen) und 7 (Textaufgaben) für eine KI, die Prüfungsfragen beantwortet. Es ist für den Einsatz auf GitHub optimiert und enthält alle relevanten Inhalte für schnelle, präzise Antworten.

---

## **2. Ausgabeformat für 7cal (STRIKT EINHALTEN!)**
- **Kein LaTeX, kein Markdown** – nur Plain Text.
- **Jede Zeile beginnt mit einer Nummer** (1), 2), 3), ...).
- **Brüche** immer als "a btel" schreiben (z. B. "3 4tel" statt 3/4).
- **Operationen** in eckigen Klammern am Zeilenende (z. B. `[+5]`, `[·2]`, `[√]`).
- **Lösungsmenge** am Ende mit `L: {}`.
- **Variablen** immer aussagekräftig benennen (z. B. `x hoch 2` statt x²).

### Beispiel (pq-Formel):
```
D: R
*1)* x hoch 2 - 6x + 5 = 0
*2)* p = -6
*3)* q = 5
*4)* x = (-p 2tel) + sqrt((p 2tel) hoch 2 - q)   [pq]
*5)* x = (-p 2tel) - sqrt((p 2tel) hoch 2 - q)   [pq]
*6)* x = 3 + sqrt(9 - 5)   [rechnen]
*7)* x = 3 - sqrt(9 - 5)   [rechnen]
*8)* x = 5
*9)* x = 1
L: {x1=5, x2=1}
```

---

## **3. Kapitel 6: Quadratische Gleichungen**

### **3.1 Definitionen & Grundlagen**
1) **Quadratische Gleichung**: Gleichung der Form ax hoch 2 + bx + c = 0 (a ≠ 0).
2) **Reinquadratische Gleichung**: ax hoch 2 + c = 0 (b = 0).
3) **Normierte Form**: x hoch 2 + px + q = 0 (a = 1).
4) **Lösungsmenge**: Alle x ∈ ℝ, die die Gleichung erfüllen.

### **3.2 Lösungsmethoden**

#### **3.2.1 Faktorzerlegung**
1) Gleichung in faktorisierter Form: (x - x1)(x - x2) = 0.
2) Lösungen: x1 und x2.
3) Beispiel:
   ```
   D: R
   *1)* x hoch 2 - 5x + 6 = 0
   *2)* (x - 2)(x - 3) = 0   [faktor]
   *3)* x = 2   [loesen]
   *4)* x = 3   [loesen]
   L: {x1=2, x2=3}
   ```

#### **3.2.2 Quadratische Ergänzung**
1) Umformung: x hoch 2 + px = (x + p 2tel) hoch 2 - (p 2tel) hoch 2.
2) Beispiel:
   ```
   D: R
   *1)* x hoch 2 - 6x + 5 = 0
   *2)* (x - 3) hoch 2 - 4 = 0   [ergänzen]
   *3)* x - 3 = ±2   [√]
   *4)* x = 3 + 2   [+2]
   *5)* x = 3 - 2   [-2]
   L: {x1=5, x2=1}
   ```

#### **3.2.3 pq-Formel**
1) Für x hoch 2 + px + q = 0: x = -p 2tel ± sqrt((p 2tel) hoch 2 - q).
2) Beispiel:
   ```
   D: R
   *1)* x hoch 2 - 6x + 5 = 0
   *2)* p = -6
   *3)* q = 5
   *4)* x = 3 + sqrt(9 - 5)   [pq]
   *5)* x = 3 - sqrt(9 - 5)   [pq]
   L: {x1=5, x2=1}
   ```

#### **3.2.4 abc-Formel (Mitternachtsformel)**
1) Für ax hoch 2 + bx + c = 0: x = (-b ± sqrt(b hoch 2 - 4ac)) / (2a).
2) Beispiel:
   ```
   D: R
   *1)* 2x hoch 2 - 8x + 6 = 0
   *2)* a = 2, b = -8, c = 6
   *3)* x = (8 ± sqrt(64 - 48)) / 4   [abc]
   *4)* x = (8 + 4) / 4   [+]
   *5)* x = (8 - 4) / 4   [-]
   L: {x1=3, x2=1}
   ```

#### **3.2.5 Vieta’sche Formeln**
1) Summe der Lösungen: x1 + x2 = -p.
2) Produkt der Lösungen: x1 · x2 = q.

---

## **4. Kapitel 7: Textaufgaben**
*(Struktur analog zu Kapitel 6, mit Beispielen im 7cal-Format)*

### **4.1 Allgemeiner Lösungsansatz**
1) Text analysieren und Variablen definieren.
2) Gleichung aufstellen.
3) Gleichung lösen (gemäß 7cal-Format).
4) Lösung im Kontext prüfen.

### **4.2 Typische Aufgabentypen**

#### **4.2.1 Zahlenaufgaben**
1) Beispiel:
   ```
   D: x ∈ ℕ
   *1)* x hoch 2 = x + 5   [gleich]
   *2)* x hoch 2 - x - 5 = 0   [umformen]
   *3)* p = -1, q = -5
   *4)* x = 0.5 ± sqrt(0.25 + 5)   [pq]
   L: {x1=2.79, x2=-2.29} → Nur x1=3 gültig (ℕ)
   ```

#### **4.2.2 Altersaufgaben**
1) Beispiel:
   ```
   D: Alter in Jahren, x > 0
   *1)* (A - 5) = 2(B - 5)   [gleich]
   *2)* A = 2B - 5   [umstellen]
   ```

---

## **5. Lehrer-Muster & Fallen**
1) **Häufige Fehler**:
   - Vorzeichenfehler bei der pq-Formel (z. B. `p = 6` statt `p = -6`).
   - Brüche falsch geschrieben (z. B. "3/4" statt "3 4tel").
2) **Lieblingsfragen**:
   - "Wann hat die Parabel ihren Scheitelpunkt?" → Scheitelform berechnen.
   - "Wie hoch ist der Zinssatz?" → Zinsformel anwenden.

---

## **6. Antwort-Templates für KI (QT-*)**
### **QT-Definition**
1) D: [Definition in 1–2 Sätzen].
2) Beispiel: [Kurzes Beispiel im 7cal-Format].

### **QT-Rechnung**
1) D: [Aufgabenstellung].
2) [Schritt-für-Schritt-Rechnung mit Tags].
3) L: [Lösung].

---

## **7. Glossar & Symbole**
1) **D**: Definitionsmenge.
2) **L**: Lösungsmenge.
3) **√**: Quadratwurzel (`sqrt`).
4) **±**: Plus/Minus (`±`).
5) **hoch 2**: Quadrat (x² → `x hoch 2`).

---
