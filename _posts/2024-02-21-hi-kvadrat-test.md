---
layout: post
title: Hi kvadrat test
categories:
- blog
---
Pretpostavimo da smo ispitali 74 učenika o tome koliko slobodnih aktivnosti imaju tjedno. Radi se učenicima drugih i četvrtih razreda osnovne škole. Znači imamo dvije kvalitativne varijable, razred i broj aktivnosti i imamo frekvencije učenika u svakoj kategoriji.

---
## Excel
1. Podatke rasporedimo u kontingencijsku tablicu očekivanih frekvencija. 
2. Izračunamo kontingencijsku tablicu očekivanih frekvencija.
3. Koristimo Excel funkciju `CHISQ.TEST raspon opaženih frekvencija raspon očekivanih frekvencija` da dobijemo p-vrijednost testa.

Pogledajmo sliku Excela.
![hikvadrat1](/assets/img/hikvadrat1.GIF){:class="img-responsive po-sredini"}

## R jezik