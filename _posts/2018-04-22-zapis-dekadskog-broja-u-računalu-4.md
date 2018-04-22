---
layout: post
title: Zapis dekadskog broja u računalu 4
categories:
- blog
---
Pretpostavimo da se cijeli brojevi u memoriji računala zapisuju u 8-bitovnim registrima metodom dvojnog komplementa.
U dvama registrima zapisane su dekadske vrijednosti $$-73$$ i $$-83$$. U treći registar treba spremiti zbroj sadržaja
ovih registara. Koji je sadržaj trećeg registra?

---

Ovaj zadatak je isti kao zadatak Zapis dekadskog broja u računalu 3, samo što sad imamo negativne brojeve.
\\[-73 + (-83) = -156\\]
Sada moramo 156 (bez minusa) prikazati u binarnom obliku.
\\[156 = 2 \cdot 78 + 0\\]
\\[78 = 2 \cdot 39 + 0\\]
\\[39 = 2 \cdot 19 + 1\\]
\\[19 = 2 \cdot 9 + 1\\]
\\[9 = 2 \cdot 4 + 1\\]
\\[4 = 2 \cdot 2 + 0\\]
\\[2 = 2 \cdot 1 + 0\\]
\\[1 = 2 \cdot 0 + 1\\]

Ostatke čitamo od dolje prema gore i dobijemo da je dekadski $$156$$ jednak binarni $$10011100$$.

Ne trebamo dodavati nikakve nulice jer imamo 8 bitova.

Primjetimo da je na prvom (najteži bit) mjestu jedinica, a to znaći da je ovaj broj negativan.
Jer znamo da negativni brojevi imaju na početku jednicu. To ćemo uzeti u obzir na kraju. 

Sada $$10011100$$ treba komplementirati ($$0$$ u $$1$$ i obrnuto) i dobijemo $$01100011$$.

Još ovo treba zbrojiti s $$1$$.

\\[01100011 + 1 = 01100100\\]

Ako traži zadatak dekadsko rješenje onda $$01110010$$ treba prebaciti u dekadski broj isto kao u zadatku 
Zapis dekadskog broja u računalu 2.

\\[-0 \cdot 2^7 + 1 \cdot 2^6 + 1 \cdot 2^5 + 0 \cdot 2^4 + 0 \cdot 2^3 + 1 \cdot 2^2 + 0 \cdot 2^1 + 0 \cdot 2^0\\]
\\[-0 + 64 + 32 + 0 + 0 + 4 + 0 + 0= 100\\]

Rješenje je $$-100$$ jer smo rekli da je broj negativan. 