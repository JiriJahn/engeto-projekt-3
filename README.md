# engeto-projekt-3

Election scraper
--------------------------------------------------------------------------------

Popis projektu
--------------------------------------------------------------------------------
Úkolem je vytvořit scraper výsledků voleb z roku 2017 dle
definovaného odkazu.

Instalace knihoven
--------------------------------------------------------------------------------
Knihovny použité v kódu jsou uložené v souboru requirements.txt

Spuštění projektu
--------------------------------------------------------------------------------
Soubor sumperk_volby.py se spouští z příkazového řádku 
a požaduje dva argumenty.

python sumperk_volby.py <odkaz_uzemniho_celku> <vystupni_soubor>

Výstupem je soubor csv s výsledkem voleb za daný územní celekm

Ukázka projektu
---------------------------------------------------------------------------------
Výsledek pro okres Šumperk:

argument 1 - https://volby.cz/pls/ps2017nss/ps32?xjazyk=CZ&xkraj=12&xnumnuts=7105
argument 2 - sumperk_volby.csv

Spuštění programu:

python sumperk_volby.py "https://volby.cz/pls/ps2017nss/ps32?xjazyk=CZ&xkraj=12&xnumnuts=7105"  "sumperk_volby.csv"

Část běhu programu:

STAHUJI DATA Z URL: https://volby.cz/pls/ps2017nss/ps32?xjazyk=CZ&xkraj=12&xnumnuts=7105
STAHUJI DATA Z URL: https://volby.cz/pls/ps2017nss/ps311?xjazyk=CZ&xkraj=12&xobec=525588&xvyber=7105
STAHUJI DATA Z URL: https://volby.cz/pls/ps2017nss/ps311?xjazyk=CZ&xkraj=12&xobec=525804&xvyber=7105
STAHUJI DATA Z URL: https://volby.cz/pls/ps2017nss/ps311?xjazyk=CZ&xkraj=12&xobec=525880&xvyber=7105
STAHUJI DATA Z URL: https://volby.cz/pls/ps2017nss/ps311?xjazyk=CZ&xkraj=12&xobec=525979&xvyber=7105
STAHUJI DATA Z URL: https://volby.cz/pls/ps2017nss/ps311?xjazyk=CZ&xkraj=12&xobec=526169&xvyber=7105
STAHUJI DATA Z URL: https://volby.cz/pls/ps2017nss/ps311?xjazyk=CZ&xkraj=12&xobec=569437&xvyber=7105
STAHUJI DATA Z URL: https://volby.cz/pls/ps2017nss/ps311?xjazyk=CZ&xkraj=12&xobec=530727&xvyber=7105
STAHUJI DATA Z URL: https://volby.cz/pls/ps2017nss/ps311?xjazyk=CZ&xkraj=12&xobec=532894&xvyber=7105
…….
STAHUJI DATA Z URL: https://volby.cz/pls/ps2017nss/ps311?xjazyk=CZ&xkraj=12&xobec=541478&xvyber=7105
UKLÁDÁM DATA DO SOUBORU: sumperk_volby.csv
UKONČUJI: sumperk_volby.py

Částečný výstup dat:

Kód obce,Název obce,Voliči v seznamu,Vydané obálky,Platné hlasy,Občanská demokratická strana,Řád národa - Vlastenecká unie,CESTA ODPOVĚDNÉ SPOLEČNOSTI,Česká str.sociálně demokrat.,Radostné Česko,STAROSTOVÉ A NEZÁVISLÍ,Komunistická str.Čech a Moravy,Strana zelených,"ROZUMNÍ-stop migraci,diktát.EU",Strana svobodných občanů,Blok proti islam.-Obran.domova,Občanská demokratická aliance,Česká pirátská strana,Referendum o Evropské unii,TOP 09,ANO 2011,Dobrá volba 2016,SPR-Republ.str.Čsl. M.Sládka,Křesť.demokr.unie-Čs.str.lid.,Česká strana národně sociální,REALISTÉ,SPORTOVCI,Dělnic.str.sociální spravedl.,Svob.a př.dem.-T.Okamura (SPD),Strana Práv Občanů
525588,Bludov,2 504,1 632,1 615,"11,02 %","0,00 %","0,00 %","7,61 %","0,06 %","8,23 %","6,93 %","1,17 %","1,05 %","0,61 %","0,06 %","0,00 %","6,81 %","0,18 %","2,35 %","31,76 %","0,06 %","0,00 %","8,42 %","0,00 %","0,18 %","0,18 %","0,12 %","12,87 %","0,24 %"
525804,Bohdíkov,1 103,640,634,"5,20 %","0,31 %","0,31 %","6,62 %","0,00 %","6,30 %","10,09 %","0,94 %","1,10 %","0,78 %","0,31 %","0,00 %","6,94 %","0,00 %","1,73 %","35,80 %","0,00 %","0,15 %","5,67 %","0,00 %","0,00 %","0,00 %","0,00 %","17,35 %","0,31 %"
525880,Bohuslavice,413,269,267,"2,99 %","0,00 %","0,00 %","6,74 %","0,00 %","4,49 %","9,73 %","0,37 %","0,37 %","2,99 %","0,37 %","0,00 %","6,74 %","0,00 %","1,49 %","37,82 %","0,00 %","0,00 %","13,85 %","0,00 %","0,37 %","0,37 %","0,00 %","11,23 %","0,00 %"

Chybový hláška v případě chybného zadání argumentů:

Zadali jte nesprávný počet argumentů. Argumenty musí být 3. Název souboru (python sumperk_volby.py), url adresa v uvozovkách a libovolný název výstupního .csv.
