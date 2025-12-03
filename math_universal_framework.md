# Universelles Math-Framework – Struktur, Stil & Automatisierung

Dieses Dokument definiert **allgemeine Regeln**, die für **alle zukünftigen Mathe-Themen** gelten sollen.

Es ist NICHT an ein bestimmtes Thema gebunden.  
Es beschreibt nur:

- wie Dateien benannt werden
- wie Lösungen aufgebaut sind
- wie ein KI-Modell Aufgaben lesen, einordnen und im richtigen Stil lösen soll

Ziel:  
Einmal festlegen, dann für jedes Thema nur noch Inhalte nachfüllen.

---

## 1. Ziele dieses Frameworks

1. **Einheitlicher Schreibstil**  
   Alle Themen sehen gleich strukturiert aus:
   - klare Schritte
   - konsistente Notation
   - gut korrigierbar für Lehrpersonen

2. **KI-kompatibel**  
   Ein generisches Modell soll:
   - den Stil sofort erkennen
   - Dateien gezielt nach Thema/Subthema laden
   - Antworten im gleichen Layout ausgeben

3. **Wiederverwendbarkeit**  
   Für jedes neue Thema müssen nur:
   - themenspezifische Formeln / Methoden ergänzt werden
   - Beispiele im gleichen Format geschrieben werden

4. **Minimaler Overhead**  
   Kein gigantisches Chaos-Repo, sondern:
   - kleine, gezielte Markdown-Dateien
   - klare Namenskonvention
   - klare Regeln für „was gehört wohin?“

---

## 2. Namenskonventionen für Themen

Jedes Mathe-Thema bekommt einen **kurzen Code-Namen**:

- nur Kleinbuchstaben
- keine Umlaute (ä → ae, ö → oe, ü → ue)
- keine Leerzeichen (Unterstrich `_` erlaubt)

Beispiele für Code-Namen (nur als Form, keine echten Inhalte):
- `thema_a`
- `thema_b_grundlagen`
- `thema_b_advanced`

Diesen Code-Namen nennen wir hier `{{T}}`.

---

## 3. Dateistruktur pro Thema

Für jedes Thema `{{T}}` gilt:

Pflicht-Dateien:

1. `{{T}}_overview.md`  
   - Überblick
   - welche Arten von Aufgaben es in diesem Thema gibt
   - kurze Beschreibung der wichtigsten Methoden

2. `{{T}}_format_style.md`  
   - wie die **Lösungen** in diesem Thema formal aussehen sollen
   - z.B.:
     - Schritt-Nummerierung
     - Schreibweise von Brüchen / Intervallen / Mengen
     - spezielle Notationen, die überall gleich bleiben

3. `{{T}}_teacher_patterns.md`  
   - beobachtete Vorlieben der Lehrperson
   - typische Fehler, die sie oft markiert
   - Bewertungs-Schwerpunkte

Optionale Dateien (empfohlen):

4. `{{T}}_subtopic_1.md`  
5. `{{T}}_subtopic_2.md`  
6. `{{T}}_subtopic_3.md`  
   - jeweils für einen klaren Unterbereich (z.B. spezielle Aufgabentypen)
   - jeder Unterbereich mit Schema + Beispielen

7. `{{T}}_mixed_tasks.md`  
   - gemischte / Prüfungsnahe Aufgaben
   - Kombination mehrerer Unterthemen

---

## 4. Allgemeiner Lösungsstil (für ALLE Themen)

Dieser Teil ist **themenunabhängig** und beschreibt, wie eine „saubere Mathe-Lösung“ generell aussehen soll.  
Diese Regeln können in jeder `{{T}}_format_style.md` wiederholt oder verlinkt werden.

### 4.1 Struktur: Kopf – Schritte – Abschluss

Standard-Aufbau:

1. **Kopfbereich**
   - optional: Definitionsmenge / Bedingungen
   - evtl. gegebene Größen kurz sauber neu notiert

2. **Mittelteil mit nummerierten Schritten**
   - `Schritt 1`
   - `Schritt 2`
   - `Schritt 3`
   - …

3. **Abschluss**
   - finale Antwort / Ergebnis in klarer Form
   - optional: Lösungsmenge, Intervall, Vektor, etc.
   - ggf. kurze Kontrolle, ob Bedingungen erfüllt sind

Beispiel-Gerüst (ohne Thema):

```text
Schritt 1
... Ausgangssituation, eventuell einfache Umformung ...

Schritt 2
... zentrale Rechnung / Transformation ...

Schritt 3
... Auflösen / Vereinfachen ...

Schritt 4
... Ergebnis sauber schreiben ...

Ergebnis:
...
Falls das Thema eine spezielle Notation für Anfang/Ende hat (z.B. D / L), wird das in {{T}}_format_style.md präzisiert.

4.2 Schritt-Nummerierung
Grundregeln:

Jeder „Block“ bekommt eine Überschrift:

text
Code kopieren
Schritt 1
Nach Schritt n IMMER eine neue Zeile.

Unter einem Schritt stehen nur die Gleichungen / Rechnungen, die logisch zusammengehören:

z.B. Umformen

Einsetzen

Addieren

Auflösen eines Terms

Beispiel-Struktur:

text
Code kopieren
Schritt 1
... Startnotation / Umschreiben ...

Schritt 2
... zentrale Umformung ...

Schritt 3
... letzte Rechenschritte ...

Ergebnis:
...
4.3 Kennzeichnung von Umformungen mit [ ]
Jede Änderung, die auf beide Seiten eines Ausdrucks angewendet wird oder eine klar benannte Operation ist, wird mit eckigen Klammern kommentiert.

Universelles Muster:

text
Code kopieren
Ausgangsausdruck   [Operation]
Typische Operationen:

[+c] → Addition einer Konstante c

[−c] → Subtraktion einer Konstante c

[·c] → Multiplikation mit c

[:c] → Division durch c

[Einsetzen] → wenn ein Ausdruck an einer Stelle eingesetzt wird

[Vereinfachen] → wenn Ausdrücke zusammengefasst werden

[Umformen] → allgemeine Umformung, falls nichts Spezielleres passt

Beispiel (themenunabhängig):

text
Code kopieren
... = ... + c      [−c]
... = ...          [:k]
Ziel:

Lehre sieht, was gemacht wurde, ohne Textroman.

KI kann den Schritt als Transformation erkennen.

4.4 Schreibweise von Brüchen / Dezimalzahlen
Dieses Framework legt nur allgemeine Regeln fest, konkrete Details pro Thema stehen in {{T}}_format_style.md.

Beispiele für allgemeine Richtlinien:

Brüche möglichst in einheitlicher Form schreiben

Dezimalzahlen nur dann verwenden, wenn:

das Thema explizit damit arbeitet

oder Rundung verlangt ist

Optionale Regel (falls gewünscht, pro Repo konsistent):

a/b wird in Text-Output nicht als Bruchstrich geschrieben,
sondern in einer alternativ festgelegten Schreibweise
(z.B. Wortbruch, gemischte Zahl, etc.).

Die genaue Entscheidung gehört in {{T}}_format_style.md.

4.5 Schreibweise von Mengen / Intervallen / Vektoren
Allgemein:

Mengen können z.B. mit { } geschrieben werden.

Intervalle können in der Form (a; b) oder [a; b] o.ä. geschrieben werden.

Vektoren können z.B. als (x|y) oder (x, y) oder als Spaltenvektor geschrieben werden.

Die konkrete Notation:

wird pro Thema (und passend zur Lehrperson) in {{T}}_format_style.md festgelegt

soll für alle Aufgaben in diesem Thema identisch beibehalten werden

5. Universal-Templates für Rechenwege
Die folgenden Templates sind bewusst abstrakt gehalten.
Sie können für sehr viele Arten von Aufgaben verwendet werden: Umformen, Lösen, Einsetzen, Fallunterscheidungen, etc.

5.1 Template A – „Etwas umformen“
Ziel: Einen Ausdruck von einer Form in eine andere bringen.

text
Code kopieren
Schritt 1
Ausgangsausdruck notieren:
...

Schritt 2
Erste Umformung:
...   [Operation 1]

Schritt 3
Weitere Umformung:
...   [Operation 2]

Schritt 4
Endform:
...

Ergebnis:
...
5.2 Template B – „Etwas lösen“ (z.B. nach einer Unbekannten)
Ziel: Eine Unbekannte (oder mehrere) aus einem Zusammenhang bestimmen.

text
Code kopieren
Schritt 1
Ausgangsgleichung(en) notieren:
...

Schritt 2
Umformungen durchführen, um die gesuchte Größe zu isolieren:
...   [Operation]
...   [Operation]

Schritt 3
Weiter vereinfachen, bis die gesuchte Größe alleine steht:
...   [Operation]

Schritt 4
Ergebnis sauber schreiben:
...

Ergebnis:
...   (gesuchte Größe in expliziter Form)
5.3 Template C – „Mehrschrittige Textaufgabe“
Ziel: Eine Aufgabenstellung mit Text in eine Rechnung übersetzen.

text
Code kopieren
Schritt 1
Wichtige Angaben aus dem Text in mathematische Größen übersetzen:
- ...
- ...
- ...

Schritt 2
Gleichung(en) oder Beziehung(en) aufstellen:
...

Schritt 3
Die Gleichung(en) nach den gesuchten Größen lösen:
...   [Operation]
...   [Operation]

Schritt 4
Ergebnis in sinnvoller Form schreiben:
...

Ergebnis:
...   (wenn nötig mit Einheiten / Interpretation)
5.4 Template D – „Fallunterscheidung“
Ziel: Unterschiedliche Fälle abhängig von einer Bedingung (z.B. Parameter, Vorzeichen, etc.).

text
Code kopieren
Schritt 1
Allgemeine Form / Ausgangssituation notieren:
...

Schritt 2
Bedingungen identifizieren, die zu verschiedenen Fällen führen:
- Fall 1: ...
- Fall 2: ...
- Fall 3: ...

Schritt 3
Fall 1 detailliert bearbeiten:
...   [Rechnungen / Umformungen]
Ergebnis Fall 1: ...

Schritt 4
Fall 2 detailliert bearbeiten:
...   [Rechnungen / Umformungen]
Ergebnis Fall 2: ...

Schritt 5
Fall 3 detailliert bearbeiten:
...   [Rechnungen / Umformungen]
Ergebnis Fall 3: ...

Zusammenfassung:
- Fall 1: ...
- Fall 2: ...
- Fall 3: ...
5.5 Template E – „Prüfungsnahe gemischte Aufgabe“
Ziel: Aufgaben lösen, bei denen mehrere Techniken / Unterthemen gleichzeitig vorkommen.

text
Code kopieren
Schritt 1
Aufgabentypen erkennen und strukturieren:
- Teil a): ...
- Teil b): ...
- Teil c): ...

Schritt 2
Teil a) bearbeiten:
...   [Operationen / Umformungen]
Ergebnis a): ...

Schritt 3
Teil b) bearbeiten:
...   [Operationen / Umformungen]
Ergebnis b): ...

Schritt 4
Teil c) bearbeiten, eventuell mit Nutzung der Ergebnisse aus a) oder b):
...   [Operationen / Verweise auf frühere Ergebnisse]
Ergebnis c): ...

Gesamtergebnis:
- a) ...
- b) ...
- c) ...
6. Universal-Regeln für KI-Modelle (z.B. 7cal)
Dieses Framework ist speziell geschrieben, damit ein generisches KI-Modell es leicht nutzen kann.

6.1 Allgemeine Arbeitsreihenfolge für KI
Aufgabe lesen

Aufgabe wird als Bild oder Text geliefert.

Relevante Informationen herausfiltern.

Thema erkennen

Welches Thema {{T}} ist betroffen?

Falls mehrere Themen relevant sind → Hauptthema bestimmen.

Passende Dateien laden

{{T}}_overview.md

{{T}}_format_style.md

{{T}}_teacher_patterns.md

ggf. spezifische Unterdateien wie {{T}}_subtopic_1.md, {{T}}_mixed_tasks.md

Lösungsstrategie festlegen

anhand der Overview- und Subtopic-Dateien

passendes Template aus Abschnitt 5 wählen (A–E oder eigenes Schema aus Thema)

Lösung im definierten Format ausgeben

Schritt-Nummerierung

Umformungen mit [ ]

Notation aus {{T}}_format_style.md verwenden

Konsistenz prüfen

Stimmt das Ergebnis mit allen Voraussetzungen überein?

Wurden alle geforderten Teile beantwortet (a, b, c, …)?

Ist das Format vollständig (Kopf, Schritte, Ergebnis)?

6.2 Verbote für das KI-Modell
Keine langen Fließtexte wie Aufsatz

Keine spontanen Stiländerungen pro Aufgabe

Keine andere Bruch- oder Mengenschreibweise als in {{T}}_format_style.md

Keine Schritte überspringen, wenn diese wichtig für Verständnis / Korrektur sind

Keine erfundenen Konventionen, die nicht im Repo definiert sind

Falls das Modell unsicher ist, soll es:

lieber einen klar markierten Zwischenschritt mehr zeigen

NICHT komplett neue Notation erfinden

7. Checkliste für neue Themen
Wenn ein neues Mathe-Thema hinzugefügt wird:

Thema-Code {{T}} wählen

kurz, ohne Umlaute, ohne Leerzeichen

Basis-Dateien anlegen

{{T}}_overview.md

{{T}}_format_style.md

{{T}}_teacher_patterns.md

Subtopic-Dateien anlegen

je nach Bedarf: {{T}}_subtopic_x.md

Fokus auf:

einen Aufgabentyp pro Datei

klares Schema + 1–3 Beispielaufgaben

Mixed-Tasks-Datei (optional)

{{T}}_mixed_tasks.md

enthält prüfungsähnliche Aufgaben

Format-Regeln anpassen

allgemeine Regeln aus diesem Framework übernehmen

ggf. Themen-spezifische Notation ergänzen:

wie werden spezielle Größen geschrieben?

wie sieht das Endergebnis typischerweise aus?

Teacher-Patterns ergänzen

was mag / hasst die Lehrperson bei diesem Thema?

typische Fehler der Klasse

extra Bonuspunkte (z.B. saubere Skizzen, klare Falltrennung)

8. Ziel dieses Frameworks
Wenn dieses Dokument respektiert wird, dann gilt:

Jedes Thema hat:

klaren Überblick

definierte formale Regeln

saubere Beispiele

Jede neue Aufgabe kann:

vom KI-Modell schnell erkannt werden

im gleichen Stil gelöst werden

Der Mensch, der abschreibt:

weiß immer, wo Kopfbereich, Schritte und Ergebnis sind

muss nichts interpretieren, nur sauber übertragen

Die Lehrperson:

sieht konsistente, transparente Lösungswege

hat wenig Angriffsfläche für „keine Rechenwege sichtbar“

Dieses Framework ist bewusst themenneutral.
Alle inhaltlichen Details (Formeln, Definitionen, spezielle Verfahren) kommen pro Thema in eigenen Dateien, die dieses Grundgerüst verwenden.

bash
Code kopieren

Da hast du dein universelles Skelett.  
Damit kannst du jedes neue Math-Thema in den gleichen Rahmen zwingen und dein zukünftiges Ich muss weniger denken und mehr nur noch kopieren.
