# Pole
Nyní už známe základy alokování paměti v jazyce *C*, zatím ale stále umíme pracovat pouze
s jednotkami proměnných. Počítače slouží k (rychlému) zpracování velkého objemu dat, a abychom je
tak naplno využili, chtěli bychom zpracovávat mnoho proměnných najednou. Například:
- V dokumentu otevřeném ve Wordu můžeme mít uložené tisíce různých znaků.
- Na server v online hře může v danou chvíli být připojené velké množství hráčů a všem musíme
posílat informace o stavu hry.
- Obrázky se běžně v programech reprezentují jako dvourozměrná mřížka pixelů. Například obrázek
ve stupních šedi s rozměry `1024x1024` vyžaduje držet v paměti `1048576` bytů (čísel) reprezentujících
jednotlivé pixely.

Asi si dovedete představit, že například pro reprezentaci obrázku bychom si s proměnnými, které jsme
používali doposud, nevystačili. Pokud bychom po jedné vytvářeli proměnné `pixel1`, `pixel2`,
`pixel3`, tak by jednak byl náš zdrojový kód obrovský a nedalo by se v něm vyznat, a také bychom
nemohli mít velikost obrázku závislou na vstupu programu, protože počet proměnných (pixelů) by byl
"zadrátovaný" ve zdrojovém kódu programu. Chtěli bychom tak mít možnost napsat kód, který bude umět
zpracovat 1, 2, 100 nebo třeba 1000 hodnot bez toho, abychom tento kód museli jakkoliv měnit.

Asi nejběžnějším a nejjednodušším způsobem, jak v paměti počítače uchovávat větší množství hodnot,
je uložit všechny hodnoty jednu po druhé za sebou v paměti. Tento koncept uložení dat se nazývá
**pole** (*array*)[^1] a je tak běžný, že ho programovací jazyky obvykle přímo podporují ve své syntaxi,
a jazyk *C* není výjimkou.

[^1]: Způsoby, jak v paměti počítače uchovávat komplexní a rozsáhlá data, se nazývají
[datové struktury](https://cs.wikipedia.org/wiki/Datov%C3%A1_struktura). Pole je jednou z
nejjednodušších datových struktur.

V následujících sekcích se dozvíte, jak s poli pracovat, jak je vytvořit v
[automatické](staticka_pole.md) a [dynamické paměti](dynamicka_pole.md) a jak lze v počítači
reprezentovat [vícerozměrná pole](vicerozmerna_pole.md).
