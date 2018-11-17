---
layout: post
title: Osjetljivost, specifičnost, učestalost, FPR, FNR, PPV i NPV statističkog testa
categories:
- blog
---
Veliki broj ljudi napravio je krvni test na prisutnost steroida. Među svim ljudima koji su napravili test 0.0098 su
pozitivni na testu i uzimali su steroide, 0.34 ih je pozitivno na testu ali nisu uzimali steroide, 0.0002 su negativni na testu
iako su uzimali steroide i 0.65 je negativno na testu i nisu uzimali steroide.

---

Neka je T pozitivan test, T' negativan test, C (eng. condition tj. stanje) da je uzimao steroide, a C' da nije uzimao steroide. 
Pa napravimo tablicu.
![osjetljivost_testa](/assets/img/osjetljivost_testa.png){:class="img-responsive po-sredini"}
Stavio sam A, B, C i D da lakše pratite rješavanje. 

Osjetljivost (Sensitivity, često se još zove i Power tj. snaga) je vjerojatnost da će test biti pozitivan za one koji
su oboljeli, pa se računa $$A/(A+C)$$.
\\[osjetljivost = \frac{0.0098}{0.0098+0.0002} = 0.98\\]
Specifičnost (Specificity) je udio (vjerojatnost) zdravih (C) koji su imali negativni test. U našem slućaju udio onih
koji nisu uzimali steroide i da im je test bio negativan, pa se računa ovako $$D/(D+B)$$.
\\[specificnost = \frac{0.65}{0.65+0.34} = 0.6565657\\]
Učestalost (eng. Prevalence) oboljelih tj. u našem slučaju onih koji su uzimali steroide je $$A+C= 0.0098+0.0002 = 0.01$$

I sada ako se npr. 1000 ljudi testiralo koliko će ih biti pozitivno na steroide? Rješenje je $$ucestalost*1000 = 0.01*1000 = 10$$ ljudi.

Alfa vrijednost testa je $$\alpha = 1-specificnost = 1-0.6565657 = 0.3434343$$ i to je ujedno FPR (false positive rate) 
tj. lažno pozitivna stopa.

Beta vrijednost testa je $$\beta = 1-osjetljivost = 1-0.98 = 0.02$$ i to je ujedno FNR (false negative rate) tj. lažno negativna
stopa.

Valja još izračunati PPV (positive predictive value) tj. vjerojatnost da će osoba s pozitivnim testom osoba uistinu biti
oboljela tj. u našem slućaju da je uzimala steroide. 
\\[PPV = \frac{A}{A+B} = \frac{0.0098}{0.0098+0.34} = 0.028\\]
Tako možemo i izračunati NPV (negative predictive value) tj. vjerojatnost da osoba koja je imala neagtivan test da uistinu bude
zdrava, a u našem slučaju da nije uzimala steroide.
\\[NPV = \frac{D}{D+C} = \frac{0.65}{0.65+0.0002} = 0.9996924\\]
