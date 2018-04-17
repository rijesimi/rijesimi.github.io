---
layout: post
title: Logički sklop 2
categories:
- blog
---
Kako glasi do kraja pojednostavljeni logički izraz sklopa prikazanog na slici?
![Sklop1](/assets/img/sklop2.png){:class="img-responsive po-sredini"}

---
Pri pojednostavljivanju ću korititi DeMorgan-ove formule.
\\[\overline{\overline{A+C}+\overline{C} \cdot B} + (B \cdot C)\\]
\\[\overline{\overline{A} \cdot \overline{C}+\overline{C} \cdot B} + (B \cdot C)\\]
\\[\overline{\overline{C} \cdot (\overline{A}+B)} + (B \cdot C)\\]
\\[\overline{\overline{C}} + \overline{(\overline{A}+B)} + (B \cdot C)\\]
\\[C + \overline{\overline{A}} \cdot \overline{B} + (B \cdot C)\\]
\\[C + A \cdot \overline{B} + (B \cdot C)\\]
\\[C + B \cdot C + A \cdot \overline{B}\\]
\\[C \cdot (1+B) + A \cdot \overline{B}\\]
\\[C \cdot 1 + A \cdot \overline{B}\\]
\\[C + A \cdot \overline{B}\\]