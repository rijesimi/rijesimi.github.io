---
layout: post
title: Zapis dekadskog broja u računalu 1
categories:
- blog
---
Za prikaz brojeva koristi se registar duljine $$1$$B ($$8$$ bitova) i metoda dvojnog komplementa. Koji će biti prikaz broja $$-35$$?

---
Prvo moramo 35 (bez minusa) prikazati u binarnom obliku.
\\[35 = 2 \cdot 17 + 1\\]
\\[17 = 2 \cdot 8 + 1\\]
\\[8 = 2 \cdot 4 + 0\\]
\\[4 = 2 \cdot 2 + 0\\]
\\[2 = 2 \cdot 1 + 0\\]
\\[1 = 2 \cdot 0 + 1\\]

Ostatke čitamo od dolje prema gore i dobijemo da je dekadski $$35$$ jednak binarni $$100011$$.
Treba biti $$8$$ bitova, a mi imamo $$6$$. To znači da trebamo dodati još $$2$$ nulice i dobijemo
$$00100011$$. Zbog toga što $$-35$$ treba prikazati onda ona prva nulica treba biti jedinica pa dobijemo
$$10100011$$, jer znamo da negativni brojevi imaju na početku jednicu.

Sada onih $$7$$ bitova s desne strane treba komplementirati ($$0$$ u $$1$$ i obrnuto) i dobijemo $$11011100$$.

Još na kraju ovo treba zbrojiti s $$1$$ i dobijemo rješenje.

\\[11011100 + 1 = 11011101\\]

NAPOMENA: da se radilo o 35 (pozitivan broj) onda imamo puno manje posla, jer ne trebamo ono komplementiranje i zbrajanje s 1.