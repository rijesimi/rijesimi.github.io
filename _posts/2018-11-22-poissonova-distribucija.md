---
layout: post
title: Poissonova distribucija
categories:
- blog
---
Pretpostavite da broj novih mutacija genoma pšenice prati Poissonovu distribuciju sa srednjom vrijednosti 8. Kolika je vjerojatnost
da će pšenica imati 5 novih mutacija? Kolika je vjerojatnost da će pšenica imati $$\le 5$$ novih mutacija?

---

Koristeći R jezik ta dva pitanja se lako izračunaju.
\\[dpois(5,8) = 0.0916\\]
\\[ppois(5,8) = 0.1912\\]

A bez pomoći računala trebamo koristiti formulu za poissonovu distribuciju.
\\[P(k, \lambda)= \frac{\lambda^{k}e^{-\lambda}}{k!}\\]
Gdje je $$k=5$$ broj mutacija pšenice, a $$\lambda=8$$ srednja vrijednost. Odgovor na prvo pitanje je:
\\[P(5, 8)= \frac{8^{5}e^{-8}}{5!} = 0.0916\\]
Odgovor na drugo pitanje je:
\\[P(0, 8)+P(1, 8)+P(2, 8)+P(3, 8)+P(4, 8)+P(5, 8)\\]
\\[= 0.0003+0.0026+0.0107+0.0286+0.0572+0.0916\\]
\\[= 0.191\\]