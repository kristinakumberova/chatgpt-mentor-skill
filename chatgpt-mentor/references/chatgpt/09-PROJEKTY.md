# Projekty a sdílené projekty

Opakované téma budete mít na jednom místě: chaty, soubory a pokyny, případně sdílené s kolegy.

## Kde v aplikaci

- Postranní panel › **Projects** › **New project**.
- V projektu: **Chats**, **Sources** (soubory), **Instructions**, sdílení projektu.
- Nastavení projektu › **Zdrojové složky** › **Add folder** (česky **Přidat složku**): složka z počítače pro místní chaty (desktopová aplikace).

## Postup

1) Založte projekt pro jedno trvalé téma: „Pracovní listy 4. A“, „Porady oddělení“, „Příprava výročky“. Jeden projekt pro všechno nedělejte.
2) Při založení zvolte paměť.
   a) **project-only memory**: chaty v projektu čerpají jen z projektu a nemíchají se s ostatními chaty. Doporučeno pro třídu, klienta nebo citlivější téma.
   b) Výchozí paměť: projekt může čerpat i z vaší obecné paměti.
   Volba se dělá při založení projektu.
3) Nahrajte do **Sources** jen ověřené podklady: šablonu, vzorový výsledek, pravidla. Business dovoluje 40 souborů na projekt.
4) Do **Instructions** napište pravidla tématu: pro koho, jaký formát, co nikdy nedělat.
5) Pro každý nový výsledek otevřete nový chat v projektu. Opravy jednoho dokumentu dělejte ve stejném chatu.
6) Když chcete projekt sdílet, otevřete v projektu nabídku sdílení (obvykle tlačítko **Share** u názvu projektu, umístění ověřte na účtu) a přidejte kolegy. Všichni ve sdíleném projektu vidí změny hned. Než ho nasdílíte, projděte soubory a chaty: kolegové uvidí i to, co jste tam dali dřív. **Projekt, ve kterém jsou údaje o žácích, klientech nebo kolezích, sdílejte jen s těmi, kdo s nimi smějí pracovat** (`03-BEZPECNE-S-DATY.md`).
7) Ověřte, že projekt soubory používá. V novém chatu se zeptejte na údaj, který je jen v nahraném souboru.
8) Rozhodněte, jestli chcete cloudový, nebo místní projekt. Aplikace to píše přímo v nastavení: pokyny, zdroje a paměť projektu platí jen pro cloudové chaty, složky jen pro místní chaty na tomto počítači.

| | Cloudový projekt | Místní projekt nad složkou |
|---|---|---|
| Kde běží | na serveru OpenAI | na vašem počítači |
| Co vidí | soubory nahrané do **Sources** | celou přidanou složku, i co v ní přibude |
| Pravidla | pole pokynů projektu | soubor `AGENTS.md` ve složce, pole pokynů chybí |
| Paměť projektu | ano | ne |
| Kolegové | projekt jde sdílet | složka je jen na vašem počítači |

   Projekt může mít obojí. Pokyny a zdroje pak platí pro cloudové chaty, složka pro místní. Pro týmovou práci a sdílení stavte cloudový projekt. Místní projekt se hodí na práci nad soubory jednoho člověka (`17-CODEX.md`, `AGENTS.md`).
9) Místní projekt nepodporuje Chat, jen Work. Místní chat v přidané složce soubory čte, mění i vytváří, často bez ptaní. Dejte mu proto složku určenou pro úkol, nebo kopii originálů, a napište, kam ukládat výstupy (například do podsložky „vystup“).
10) Složek může být víc. `AGENTS.md`, skilly a nastavení se hledají jen v hlavní (první) složce. Ostatní složky jsou jen k hledání, čtení a úpravám.
11) Když má projekt obě části (krok 8), pokyny se udržují na dvou místech. Aby se nepsaly dvakrát:
   a) pravidla napište jednou do souboru `POKYNY.md` ve složce,
   b) do `AGENTS.md` dejte jen „Řiď se souborem POKYNY.md v této složce.“,
   c) stejný `POKYNY.md` nahrajte do **Sources** a do pole pokynů napište „Řiď se souborem POKYNY.md ve zdrojích.“,
   d) po změně `POKYNY.md` znovu nahrajte do **Sources**, zdroje se samy neaktualizují.
   Postup je návrh příručky, nevyzkoušený. Ověřte otázkou v cloudovém i místním chatu: „Podle jakých pravidel pracuješ a ze kterého souboru je máš?“
12) Znalostní složka (příručka, metodika) jako místní projekt: ve složce musí ležet `AGENTS.md` s pokyny, jak podle souborů odpovídat. Bez něj místní chat soubory vidí, ale odpovídá z obecných znalostí nebo z webu. Pro tuto příručku je `AGENTS.md` připravený (`00-NAVIGATOR.md`, krok 6). V Codexu nad balíčkem 3. 11. 2026 fungoval (vykal, citoval soubor a krok), v aplikaci ChatGPT SIGNAL.

## Příklad

Instrukce projektu (škola):

```
Projekt: pracovní listy pro 4. třídu, čeština.
Pracovní list je na jednu stranu A4, otázky jen na informace z dodaného textu, klíč vždy jako samostatný soubor.
Šablona je v souboru „sablona-pracovni-list.docx“. Drž její strukturu.
Nikdy nepoužívej jména skutečných žáků. Když chybí cíl hodiny nebo věk, zeptej se.
```

Instrukce projektu (kancelář):

```
Projekt: týdenní porady oddělení.
Zápis vždy jako tabulka rozhodnutí, úkol, kdo, do kdy. Chybějící termín označ „neuvedeno“.
Seznam rolí v oddělení je v souboru „role.md“. Jména přebírej jen ze zápisu.
Na konci každého zápisu vypiš úkoly z minulého týdne, které nejsou uzavřené.
```

Kontrola, že projekt čte soubory:

```
Jaká pravidla platí pro tento projekt a ze kterého souboru je máš? Uveď název souboru.
```

## Když to chybí

- Chybí **Projects**: pracujte v jednom pojmenovaném chatu a pokyny i šablonu vložte na začátek každého nového chatu.
- Nejde nastavit sdílení: tarif to nemá, nebo správce sdílení omezil.
- Projekt je plný: sloučte malé soubory do jednoho, staré verze odstraňte. Úložiště je omezené i na uživatele (25 GB) a organizaci (100 GB).
- Obrázek z PDF v projektu se nenačte: přiložte PDF přímo do chatu (`05-SOUBORY.md`).
- Místní chat nedrží pokyny projektu: to je správně, místní chaty pokyny nepoužívají. Pravidla dejte do souboru `AGENTS.md` v přidané složce.
- Místní chat nad příručkou necituje soubory a odpovídá z webu: ve složce chybí `AGENTS.md` (krok 12).
- Místní chat v projektu nejde založit (Windows): přidejte složku hned při zakládání chatu (hlášení uživatelů, SIGNAL).

## Zdroj a stav

- 40 souborů na projekt v Business, úložiště 25 GB na uživatele a 100 GB na organizaci, sdílené projekty se změnami živě, project-only memory při založení: https://help.openai.com/en/articles/8555545, stav k 2. 11. 2026, FAKT.
- Projekty v praxi: https://openai.com/academy/projects, stav k 2. 11. 2026.
- Přesný název a umístění tlačítka sdílení projektu v aplikaci: SIGNAL, ověřte na účtu.
- Pokyny, zdroje a paměť jen pro cloudové chaty, složky jen pro místní: text v nastavení projektu v desktopové aplikaci, snímek obrazovky 2. 11. 2026, FAKT.
- Místní projekt nepodporuje Chat, víc složek, `AGENTS.md` a skilly jen v hlavní složce, čtení a změny souborů ve všech přidaných složkách, synchronizace chatu složku nenahrává: https://learn.chatgpt.com/docs/projects, stav k 3. 11. 2026, FAKT.
- Příručka jako místní projekt bez `AGENTS.md` odpovídala z webu a necitovala soubory: zkouška 3. 11. 2026, FAKT pro tento případ. S `AGENTS.md` v Codexu nad balíčkem odpověď vykala a citovala soubor a krok: zkouška 3. 11. 2026, FAKT pro Codex.
- Rady z praxe (vyhrazená složka nebo kopie, říct, kam ukládat): https://www.bigprompthub.com/chatgpt-work-local-files-permissions-privacy/, https://stashbase.ai/blog/can-chatgpt-access-local-files/, chyba na Windows https://github.com/openai/codex/issues/34499, stav k 3. 11. 2026, SIGNAL.
- Místní běh čte `AGENTS.md` ze složky: test 2. 11. 2026, Codex nad testovací složkou na českou otázku odpověděl anglicky podle `AGENTS.md`, FAKT pro Codex. Pro místní chat v aplikaci ChatGPT SIGNAL (stejné jádro, v aplikaci zatím nezkoušeno).
