# Naplánované úlohy

Ověřený postup necháte běžet pravidelně, třeba každé pondělí ráno, a víte, jak úlohu pozastavit.

## Kde v aplikaci

- Seznam úloh: postranní panel › **Scheduled**.
- Nová úloha: **Scheduled** › tlačítko pro novou úlohu (název ověřte na účtu). Úlohu jde vytvořit i v chatu: napíšete, co a kdy se má opakovat.
- Úlohy spouštěné událostí (nový e-mail v Gmailu, zpráva ve Slacku): pokročilé, zatím přeskočte.

## Postup

1) Vyberte úkol, který už ručně funguje. Prompt nejdřív spusťte aspoň dvakrát sami a výsledek zkontrolujte.
2) Napište zadání úlohy celé:
   a) co přesně udělat a z jakých zdrojů,
   b) kdy: den a čas,
   c) jak má výsledek vypadat,
   d) co dělat, když zdroj není dostupný nebo je prázdný (nic neměnit, jen napsat),
   e) kdy úloha skončí.
3) Úloha pracuje bez vás. Dejte jí jen čtení. Odesílání, mazání a změny v dokumentech do pravidelné úlohy nedávejte, dokud první běhy nezkontrolujete.
4) Vytvořte úlohu v **Scheduled** tlačítkem pro novou úlohu, nebo v chatu.
5) Zkontrolujte čas a časové pásmo. V úloze má být váš místní čas (pro Česko Europe/Prague). Když úloha ukazuje jiný čas, napište pásmo do zadání.
6) Nastavte upozornění: zkontrolujte, jestli vám o výsledku přijde oznámení v aplikaci nebo e-mail, a v nastavení oznámení ho případně zapněte (přesné místo ověřte na účtu). Bez upozornění výsledek najdete jen v **Scheduled**.
7) Spusťte úlohu jednou ručně, pokud to nabídka dovolí, a pak počkejte na první naplánovaný běh. Teprve potom ji nechte běžet dál.
8) Po prvních dvou bězích výsledky zkontrolujte. Když něco nesedí, úlohu pozastavte a zadání opravte.
9) Hlídejte strop: Business má nejvýš 10 aktivních úloh. Nepotřebné úlohy smažte nebo pozastavte.
10) Úloha nejspíš používá oprávnění, která máte v době běhu (SIGNAL). Když se odpojíte od Google Drive nebo SharePointu, úloha zdroj neotevře. Proto krok 7: první běh ukáže, jestli přístup funguje.

## Příklad

Školní týden:

```
Každý pátek v 15:00 (Europe/Prague) mi připrav návrh tří krátkých rozcviček na čtení s porozuměním pro 4. třídu na příští týden, každou na jednu minutu. Témata střídej, ať se neopakují s minulým týdnem. Jen návrh do chatu.
```

Přehled novinek:

```
Každé pondělí v 7:00 (Europe/Prague) vyhledej novinky k [tématu] za poslední týden. Nejvýš tři položky, u každé oficiální zdroj s odkazem a datem. Když nic nového není, napiš „beze změny“. Úloha končí 31. 1. 2027.
```

Týdenní přehled ze SharePointu (SIGNAL, na účtu nevyzkoušené, jen když máte SharePoint připojený, `13-KONEKTORY-GOOGLE-MICROSOFT.md`):

```
Každé pondělí v 7:30 (Europe/Prague) projdi na SharePointu složku [Porady] a vypiš úkoly z posledního zápisu, které mají termín tento týden: úkol, kdo, do kdy. Jen čti, nic neměň a nikomu nic neposílej. Když zápis nenajdeš, napiš „zápis nenalezen“ a skonči. Úloha končí 31. 1. 2027.
```

## Když to chybí

- Chybí **Scheduled**: tarif nebo správce úlohy nemá zapnuté. Prompt si uložte do projektu a spouštějte ho ručně.
- Nejde vytvořit další úlohu: máte 10 aktivních úloh. Jednu pozastavte nebo smažte.
- Úloha neběží nebo hlásí chybu přístupu: zkontrolujte připojení konektoru (`13-KONEKTORY-GOOGLE-MICROSOFT.md`).
- Úloha běží v jiný čas: v zadání chybí časové pásmo (krok 5).
- Nepřišlo upozornění: zkontrolujte nastavení oznámení (krok 6) a výsledek najděte v **Scheduled**.

## Zdroj a stav

- Naplánované úlohy, strop 10 aktivních úloh v Business, úlohy spouštěné událostí ve Work, umístění Scheduled: https://help.openai.com/en/articles/10291617, stav k 2. 11. 2026, FAKT. Starší verze nápovědy uváděla 15 úloh, platí 10.
- Název tlačítka nové úlohy, místo nastavení oznámení a ruční spuštění úlohy: SIGNAL, ověřte na účtu.
- Oprávnění v době běhu: SIGNAL, podle starší nápovědy používá úloha na pozadí nastavená oprávnění.
- Přehled jako stránka, kterou úloha každé ráno obnoví: praktik Ben AI, https://www.youtube.com/watch?v=EKZka39wD3w, SIGNAL (`16-SITES-A-PAGES.md`).
