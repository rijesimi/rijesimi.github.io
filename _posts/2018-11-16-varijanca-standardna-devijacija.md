---
layout: post
title: Varijanca i standardna devijacija
categories:
- blog
---
Sa biljke su nasumično prikupljena četiri lista i određen im je sadržaj nitrata 2, 1, 6 i 2. Kolika je standardna devijacija ovog uzorka
(na 1 decimalna mjesta)?

---

Koristeći R jezik to se izračuna brzo sa ove dvije naredbe.
\\[x=c(2,1,6,2)\\]
\\[sd(x)\\]
Ili će te na starinski način pomoću formule za varijancu ali zato prvo treba izračunati prosjek $$\overline{x}$$.
\\[\overline{x} = \frac{2+1+6+2}{4} = 2.75\\]
\\[\sigma^2 = var = \frac{1}{n-1}\sum_{}^{}(x_{i}-\overline{x})\\]
\\[= \frac{1}{4-1}\Big((2-2.75)^2+(1-2.75)^2+(6-2.75)^2+(2-2.75)^2\Big) = 4.92\\]
Sada je standardna devijacija $$\sigma$$, znači korjen od varijance.
\\[\sigma = \sqrt{4.92} = 2.2\\]