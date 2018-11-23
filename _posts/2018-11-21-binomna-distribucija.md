---
layout: post
title: Binomna distribucija
categories:
- blog
---
Biljke Asparagus su ili muškog ili ženskog spola i ženke stvaraju veće izdanke. Pretpostavite da broj ženskih biljaka prati binomnu
distribuciju sa $$p=0.9$$. Kolika je vjerojatnost da je 6 sjemenki u skupini od 10 sjemenki ženskog spola?

---

Koristeći R jezik to se lako izračuna.
\\[dbinom(6, 10, 0.9) = 0.0111\\]

A bez pomoći računala trebamo koristiti formulu za binomnu distribuciju.
\\[\binom{n}{k}p^{k}(1-p)^{n-k}\\]
Gdje je $$n=10$$ ukupan broj u skupini, a $$k=6$$ broj sjemenki čiju vjerojatnost tražimo.
\\[\binom{10}{6}0.9^{6}0.1^{4} = 0.0111\\]