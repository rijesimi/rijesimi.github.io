---
layout: post
title: Logički sklop 1
categories:
- blog
---
Kako glasi do kraja pojednostavljeni logički izraz sklopa prikazanog na slici?
![Sklop1](/assets/img/sklop1.png){:class="img-responsive po-sredini"}

---
Pri pojednostavljivanju ću korititi DeMorgan-ove formule.
\\[\overline{A+B} \cdot (A+C)\\]
\\[\overline{A} \cdot \overline{B} \cdot (A+C)\\]
\\[\overline{A} \cdot \overline{B} \cdot A + \overline{A} \cdot \overline{B} \cdot C\\]
\\[\overline{A} \cdot A \cdot \overline{B} + \overline{A} \cdot \overline{B} \cdot C\\]
\\[0 \cdot \overline{B} + \overline{A} \cdot \overline{B} \cdot C\\]
\\[0 + \overline{A} \cdot \overline{B} \cdot C\\]
\\[\overline{A} \cdot \overline{B} \cdot C\\]
