# Verze, návrat zpět a šablony

Kapitola vás naučí najít a vrátit dřívější stav souboru a uložit si šablonu. Než AI poprvé zapíše do souboru, musíte umět změnu vrátit.

## Kde

- Nativní Google dokument: **Soubor** › **Historie verzí**, nebo ikona hodin vpravo nahoře.
- Nahraný soubor (PDF, Word): Disk Google na počítači › pravé tlačítko na souboru › **Spravovat verze** (podle rozložení může být pod **Informace o souboru**).
- Obojí jen v prohlížeči na počítači. Mobilní aplikace tyto nabídky nemusí mít.

## Postup

1) Před každým zápisem AI pojmenujte aktuální verzi.
   a) **Nativní soubor:** **Soubor** › **Historie verzí** › **Pojmenovat aktuální verzi** › například „Před úpravou AI 2. 11.“.
   b) **Nahraný soubor:** stáhněte si kopii, nebo pracujte rovnou na kopii (krok 4).

2) Najděte dřívější stav nativního souboru: **Soubor** › **Historie verzí** › **Zobrazit historii verzí** › vpravo vyberte verzi. Změny jsou barevně vyznačené. K historii potřebujete právo upravovat.

3) Vraťte dřívější stav.
   a) **Celý soubor:** u verze nabídka se třemi tečkami › **Obnovit tuto verzi** › potvrďte. Novější verze v historii zůstanou.
   b) **Jen část:** u verze **Vytvořit kopii**, z kopie zkopírujte potřebný odstavec zpět.
   c) **Nahraný soubor:** **Spravovat verze** › starší verzi stáhněte › nahrajte ji jako **Nahrát novou verzi**. Důležitou verzi označte **Zachovat navždy**. Jinak ji Disk smaže po 30 dnech nebo když přibude 100 novějších verzí.

4) Pro cvičení a první zápisy AI pracujte na kopii: **Soubor** › **Vytvořit kopii** › název s `_kopie` › složka **02_Rozpracovane**.

5) Schválenou verzi pojmenujte, například „Schváleno vedoucí 2. 11.“. Název souboru „finální“ schválení nedokazuje.

6) Šablonu uložte takhle:
   a) Vezměte schválený výsledek (zápis z porady, pracovní list, nabídku).
   b) Nechte AI odstranit konkrétní údaje promptem níž.
   c) Výslednou prázdnou šablonu uložte do složky **Sablony**.
   d) Při použití: **Soubor** › **Vytvořit kopii** šablony, nikdy nepište do šablony samotné.

## Příklad

Škola: pracovní list s názvem, cílovou skupinou, textem a třemi otázkami. Klíč s odpověďmi je v samostatném souboru.
Kancelář: zápis z porady s částmi rozhodnutí, úkol, kdo, termín. Chybějící údaj se píše „neuvedeno“.

```
Vytvoř šablonu z tohoto schváleného dokumentu: [odkaz nebo vložený text].
Zachovej: nadpisy, pořadí částí, formát tabulek a rozsah.
Konkrétní údaje (jména, data, čísla, odpovědi, odkazy) nahraď zástupnými poli v hranatých závorkách, například [termín].
Vrať prázdnou šablonu a seznam vstupů, které bude potřeba vyplnit.
Původní dokument neměň. Když není jasné, co zachovat, zeptej se.
```

Kontrola: v šabloně nesmí zůstat žádné jméno ani číslo z původního dokumentu. Zkuste šablonu použít s neúplným podkladem. AI má říct, co chybí, a nedoplnit si to sama.

## Když to chybí

| Co vidíte | Co udělat |
|---|---|
| Historie verzí je šedá | Nemáte právo upravovat. Požádejte vlastníka, nebo si vytvořte kopii. |
| Není Spravovat verze | Je to nativní Google soubor, použijte Historii verzí (krok 2). |
| Hledaná verze nahraného souboru zmizela | Uplynulo 30 dní bez Zachovat navždy. Obnovit ji nejde, hledejte staženou kopii. |
| AI přepsala šablonu | Obnovte šablonu z historie (krok 3a) a v promptu pište „vytvoř kopii šablony“. |

## Zdroj a stav

- Historie verzí dokumentů: https://support.google.com/docs/answer/190843 (FAKT)
- Verze nahraných souborů, 30 dní a 100 verzí: https://support.google.com/drive/answer/2409045 (FAKT)
- Vytvoření kopie: https://support.google.com/docs/answer/49114
- Stav k 2. 11. 2026. Popisky Pojmenovat aktuální verzi a Obnovit tuto verzi ověřte na svém účtu.
