---
layout: post
title: Zapis dekadskog broja u računalu 3
categories:
- blog
---
Pretpostavimo da se cijeli brojevi u memoriji računala zapisuju u 8-bitovnim registrima metodom dvojnog komplementa.
U dvama registrima zapisane su dekadske vrijednosti $$93$$ i $$49$$. U treći registar treba spremiti zbroj sadržaja
ovih registara. Koji je sadržaj trećeg registra?

---

\\[93 + 49 = 142\\]
Sada moramo 142 prikazati u binarnom obliku.
\\[142 = 2 \cdot 71 + 0\\]
\\[71 = 2 \cdot 35 + 1\\]
\\[35 = 2 \cdot 17 + 1\\]
\\[17 = 2 \cdot 8 + 1\\]
\\[8 = 2 \cdot 4 + 0\\]
\\[4 = 2 \cdot 2 + 0\\]
\\[2 = 2 \cdot 1 + 0\\]
\\[1 = 2 \cdot 0 + 1\\]

Ostatke čitamo od dolje prema gore i dobijemo da je dekadski $$142$$ jednak binarni $$10001110$$.

Primjetimo da je na prvom (najteži bit) mjestu jedinica, a to znaći da je ovaj broj negativan.
Jer znamo da negativni brojevi imaju na početku jednicu. To ćemo uzeti u obzir na kraju. 

Sada $$10001110$$ treba komplementirati ($$0$$ u $$1$$ i obrnuto) i dobijemo $$01110001$$.

Još ovo treba zbrojiti s $$1$$.

\\[01110001 + 1 = 01110010\\]

Sada $$01110010$$ treba prebaciti u dekadski broj isto kao u zadatku Zapis dekadskog broja u računalu 2.

\\[-0 \cdot 2^7 + 1 \cdot 2^6 + 1 \cdot 2^5 + 1 \cdot 2^4 + 0 \cdot 2^3 + 0 \cdot 2^2 + 1 \cdot 2^1 + 0 \cdot 2^0\\]
\\[-0 + 64 + 32 + 16 + 0 + 0 + 2 + 0= 114\\]

Rješenje je $$-114$$ jer smo rekli da je broj negativan. 