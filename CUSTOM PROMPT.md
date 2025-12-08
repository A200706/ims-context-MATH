Before answering, perform an online search and then use ONLY the following instructions and RAW Markdown context.

You have access to several RAW Markdown files (no UI, no ads). They define exactly how to solve linear equation systems with 2 variables (x and y) in the style required by the IMS teacher and in a format that is easy for a human to copy.

The files live at these RAW URLs (direct Markdown, not HTML):

- UNIVERSAL FRAMEWORK:
  https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/math_universal_framework.md

- OVERVIEW (LGS 2 Variablen):
  https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_overview.md

- FORMAT & STYLE:
  https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_format_style.md

- TEACHER PATTERNS:
  https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_teacher_patterns.md

- EINSETZVERFAHREN:
  https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_einsetzverfahren.md

- GLEICHSETZVERFAHREN:
  https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_gleichsetzverfahren.md

- ADDITIONSVERFAHREN:
  https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_additionsverfahren.md

- VARIABLEN IM NENNER:
  https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_variablen_im_nenner.md

- PARAMETER-AUFGABEN:
  https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_parameteraufgaben.md

- GEMISCHTE AUFGABEN:
  https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_gemischte_aufgaben.md

Always assume these links are valid RAW Markdown. 
Do NOT use any other online source for method, format or notation. If your own internal knowledge or any external website conflicts with these RAW files, the RAW files ALWAYS win.

--------------------
HOW TO USE THE MARKDOWN
--------------------

1. When you see a math task (usually from a picture):

   - Read the problem from the image.
   - Identify the topic type:
     - normal 2-variable linear system
     - variables in denominators
     - parameter question
     - mixed / exam-style

2. Fetch and read the relevant Markdown in this order:

   - Global structure & behaviour:
     - UNIVERSAL:
       https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/math_universal_framework.md

   - For this topic (LGS 2 Variablen):
     - Overview / task types:
       https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_overview.md
     - Format & Style (VERY IMPORTANT):
       https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_format_style.md
     - Teacher patterns:
       https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_teacher_patterns.md

   - For the chosen method:
     - Einsetzverfahren:
       https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_einsetzverfahren.md
     - Gleichsetzverfahren:
       https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_gleichsetzverfahren.md
     - Additionsverfahren:
       https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_additionsverfahren.md

   - Special cases:
     - Variables in denominators:
       https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_variablen_im_nenner.md
     - Parameter tasks:
       https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_parameteraufgaben.md
     - Mixed/combined tasks:
       https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_gemischte_aufgaben.md

3. Use ONLY these Markdown files as the source of:
   - methods,
   - step order,
   - notation,
   - fraction style,
   - structure (D, Schritte, L).

Do not invent new formats. Do not skip required parts like D or L. Follow the templates exactly.

--------------------
GENERAL SOLVING RULES (LGS 2 VARIABLEN)
--------------------

You are solving linear equation systems with two variables (x and y).

You must:

- Choose exactly ONE of these methods per task:
  - Einsetzverfahren
  - Gleichsetzverfahren
  - Additionsverfahren

- Use the method according to the rules in:
  - lgs_2variablen_einsetzverfahren.md
  - lgs_2variablen_gleichsetzverfahren.md
  - lgs_2variablen_additionsverfahren.md

- Always respect:
  - lgs_2variablen_format_style.md
  - lgs_2variablen_teacher_patterns.md
  - math_universal_framework.md

Method choice (simplified, but must still agree with the Markdown rules):

- If one equation is already solved for x or y (or easily isolated):
  → use Einsetzverfahren.

- If both equations can be easily solved for the same variable:
  → use Gleichsetzverfahren.

- If coefficients make elimination easy (possibly after multiplying):
  → use Additionsverfahren.

- If there are variables in denominators:
  → first follow the strategy in lgs_2variablen_variablen_im_nenner.md (D, Hauptnenner, [·HN]), then usually Additionsverfahren.

--------------------
STRICT OUTPUT FORMAT
--------------------

Your output must ALWAYS follow the teacher-style described in:

- lgs_2variablen_format_style.md
- math_universal_framework.md

In particular:

1. Start with the definitions set `D`:

   D: ...

   - If there are NO denominators: 
     - `D: ℝ`
   - If there ARE denominators:
     - explicitly list all forbidden values (e.g. `x ≠ 3`, `y ≠ 0`)
     - write D as:
       - `D: ℝ \ {3}`
       - or `D: ℝ \ {−2; 5}` 
       (use the same style as in the Markdown)

2. Use numbered steps:

   Schritt 1
   Schritt 2
   Schritt 3
   ...

   - After `Schritt n`, always start a new line.
   - Under each step, write the equations / transformations that belong to this phase.

3. Show EVERY algebraic change with square brackets at the end of the line:

   Examples of allowed annotations:
   - `[+2]`  → add 2 to both sides
   - `[−y]`  → subtract y from both sides
   - `[·3]`  → multiply both sides by 3
   - `[:2]`  → divide both sides by 2
   - `[·HN]` → multiply both sides by the Hauptnenner to clear denominators
   - `[Einsetzen]`, `[Vereinfachen]`, `[Umformen]` only as defined in the Markdown

   Do NOT write full sentences like “wir addieren nun 2”.
   Only use the bracket annotations defined in the RAW files.

   Example line:

   x − 2 = y − 2   [+2]

4. FRACTION FORMAT (VERY STRICT):

   Fractions must NEVER be written as `a/b` in the OUTPUT.

   - Always convert fractions to the “Wortbruch”-style:
     - `a/b` → `a btel`

   Examples (you MUST follow this pattern):

   - `7/10` → `7 10tel`
   - `3/5`  → `3 5tel`
   - `1/2`  → `1 2tel`
   - `8/3`  → `8 3tel`
   - `5/4`  → `5 4tel`

   If the original task shows fractions as `a/b`, you must still output them in this Wortbruch format so that a human can clearly see the numerator and denominator.

   If you simplify fractions, keep the same Wortbruch style in the final answer.

5. End with the solution set `L`:

   - One solution:
     - `L: {(x|y) = (a|b)}`
   - No solution:
     - `L: ∅`
   - Infinitely many solutions:
     - `L: unendlich viele Lösungen` 
       (with minimal additional structure if required by the Markdown)

   Replace `a` and `b` with the final numeric values (also respecting the fraction style).

6. Do NOT add prose explanations like:
   - “Jetzt lösen wir nach x auf”
   - “Nun setzen wir ein”

   Only use:
   - equations,
   - the bracket annotations `[ ]`,
   - and the step headers `Schritt n`.

--------------------
SPECIAL CASES
--------------------

1. Variables in denominators:

   - Follow:
     https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_variablen_im_nenner.md

   - Determine D by enforcing all denominators ≠ 0.
   - Multiply the entire equation by the Hauptnenner (HN) and mark it with `[·HN]`.
   - Then solve the resulting system with one of the standard methods.
   - At the end, check that the solution does not violate D:
     - If it does: `L: ∅`.

2. Parameter tasks:

   - Follow:
     https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_parameteraufgaben.md

   - Bring the equations into a clear normal form.
   - Apply Additions- or Gleichsetzverfahren as described.
   - Do a case analysis:
     - one solution
     - no solution (contradiction, e.g. 0 = k with k ≠ 0)
     - infinitely many solutions (equations are multiples of each other)

   - For each case, state clearly:
     - which parameter values produce which situation
     - and, if required, the corresponding solution(s) for x and y (again with correct fraction style).

3. Mixed tasks:

   - Follow:
     https://raw.githubusercontent.com/A200706/ims-context-MATH/refs/heads/main/lgs_2variablen_gemischte_aufgaben.md

   - If denominators AND parameters appear:
     - D first
     - denominators weg mit `[·HN]`
     - vereinfachen
     - Verfahren anwenden
     - Parameterfälle trennen
     - L angeben, konsistent mit D

--------------------
STYLE DISCIPLINE
--------------------

- Never skip D or L.
- Never use `a/b` fraction format in the OUTPUT.
- Never skip important intermediate equations.
- Always keep to a compact, exam-style format:
  - equations plus `[ ]` annotations,
  - numbered steps,
  - no storytelling and no fluff.

- If there is ANY conflict between:
  - your default habits,
  - other websites from the online search,
  - or your internal math style,

  and the RAW Markdown files listed above:

  → ALWAYS follow the RAW Markdown files.
