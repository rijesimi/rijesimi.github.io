---
layout: post
title: Laplaceova transformacija
categories:
- blog
---

Riješite $$6y''-5y'-y=0$$, uz ove početne uvijete $$y(0)=1$$,  $$y'(0)=-2$$ laplaceovom transformacijom.

---

\\[6\big(s^2y(s)-sy(0)-y'(0)\big)-5\big(sy(s)-y(0)\big)-y(s)=0\\]
\\[6\big(s^2y(s)-s+2\big)-5\big(sy(s)-1\big)-y(s)=0\\]
\\[6s^2y(s)-6s+12-5sy(s)+5-y(s)=0\\]
\\[y(s)(6s^2-5s-1)=6s-17\\]
\\[y(s)=\frac{6s-17}{6s^2-5s-1}\\]
Pomoću kvadratne jednadžbe (njena rješenja su -1/6 i 1) faktorizirajmo nazivnik.             
\\[y(s)=\frac{6s-17}{6(s+\frac{1}{6})(s-1)}\\]        
Ovaj razlomak (bez one 6-ice u nazivniku, nju ćemo pred kraj napisati) ćemo rastaviti na parcijalne razlomke. Treba naći A i B.
\\[\frac{6s-17}{(s+\frac{1}{6})(s-1)}=\frac{A}{s+\frac{1}{6}}+\frac{B}{s-1} \quad \bigg/\cdot(s+\frac{1}{6})(s-1)\\]
\\[6s-17=A(s-1)+B(s+\frac{1}{6})\\]
\\[6s-17=As-A+Bs+\frac{1}{6}B\\]
Sada dobijemo sustav dvije jednadžbe:
\\[A+B=6\\]
\\[-A+\frac{1}{6}B=-17\\]
Zbrojimo ih i dobijemo $$\text{B}=\frac{-66}{7}$$, $$\text{A}=\frac{108}{7}$$. I sada imamo:
\\[y(s)=\frac{1}{6}\bigg(\frac{108}{7}\cdot\frac{1}{s+\frac{1}{6}}-\frac{66}{7}\cdot\frac{1}{s-1}\bigg)\\]
\\[y(s)=\frac{18}{7}\cdot\frac{1}{s+\frac{1}{6}}-\frac{11}{7}\cdot\frac{1}{s-1}\\]
Sada koristeći tablicu laplaceove transformacije elmentarnih funkcija dobijemo rješenje (primjetiom da nema više $$s$$ nego $$x$$):
\\[y(x)=\frac{18}{7}e^{\frac{-1}{6}x}-\frac{11}{7}e^x\\]