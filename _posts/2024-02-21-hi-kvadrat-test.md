---
layout: post
title: Hi kvadrat test
categories:
- blog
---
Pretpostavimo da smo ispitali 74 učenika o tome koliko slobodnih aktivnosti imaju tjedno. Radi se učenicima drugih i četvrtih razreda osnovne škole. Znači imamo dvije kvalitativne varijable, razred i broj aktivnosti i imamo frekvencije učenika u svakoj kategoriji.

---
EXCEL
1. Podatke rasporedimo u kontingencijsku tablicu očekivanih frekvencija. 
2. Izračunamo kontingencijsku tablicu očekivanih frekvencija.
3. Koristimo Excel funkciju `CHISQ.TEST raspon opaženih frekvencija raspon očekivanih frekvencija` da dobijemo p-vrijednost testa.

![hikvadrat](/assets/img/hikvadrat.PNG){:class="img-responsive po-sredini"}

R jezik
1. Radimo tablicu

`M <- as.table(rbind(c(8, 10), c(4, 12), c(10, 3), c(21, 6)))`

2. Dajemo imena redovima i stupcima

`dimnames(M) <- list(aktivnosti = c("1akt", "2akt", "3akt", "više od 3"),
                    razred = c("drugi","četvrti"))`

3. Kako izgleda kontingencijska tablica?

`(M)`

4. Rezultat testa. Dalje s varijablom hi možemo dodatne stvari raditi.

`(hi <- chisq.test(M))`