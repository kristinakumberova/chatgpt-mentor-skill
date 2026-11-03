# Skills a skill-creator

Postup, který vám opakovaně funguje, uložíte jako skill, spustíte ho jedním výběrem a nasdílíte kolegům.

## Kde v aplikaci

- **Plugins › Skills**, záložky **Installed**, **Created by me**, **Shared with me** a **Shared by {název workspace}**.
- V chatu: skill vyberete přes **@** (například **@skill-creator**), přes **+** nebo **Plugins**.
- V Codexu se skill vyvolá názvem s **$** (`$skill-creator`, `17-CODEX.md`).
- Kam se skill uloží, záleží na tom, kde ho vytvoříte (krok 4).
- Skilly v účtu ChatGPT mají tarify Business, Enterprise, Healthcare a Edu. Na ostatních tarifech (Free, Go, Plus, Pro) je skill nejspíš jen místní: ve Work na desktopu a v Codexu (PŘEDPOKLAD).

Skill je složka. Povinný je jen soubor `SKILL.md` (název, popis, kdy ho použít, postup). Vedle něj mohou být:

| Podsložka | Co v ní je | Příklad |
|---|---|---|
| `references/` | podklady, ze kterých skill čerpá | pravidla školy, tabulka hodnot |
| `assets/` | šablony a vzory výstupu | šablona pracovního listu |
| `scripts/` | skripty, které skill spustí | převod tabulky do Excelu |

Skript ve Work na desktopu a v Codexu běží na počítači v chráněném prostředí a pracuje se soubory v přidané složce. Skill v ChatGPT v cloudu k počítači přístup nemá. Skill může v postupu jmenovat aplikaci (například „podklady najdi na Disku“), ale připojení obsahuje až plugin (`20-POJMY.md`).

## Postup

1) Vyberte postup, který už aspoň třikrát fungoval. Třeba „pracovní list z textu s klíčem zvlášť“ nebo „zápis z porady do tabulky úkolů“. Skill z postupu, který jste nevyzkoušeli, nedělejte.
2) Připravte si podklady: kroky postupu, šablonu nebo vzorový výsledek a co se má stát, když vstup chybí.
3) Vytvořte skill. Doporučujeme způsob a).
   a) Chatem (doporučeno): napište „vytvoř mi skill…“ (prompt v oddílu Příklad). ChatGPT k tomu samo použije **skill-creator**, který máte v účtu od začátku. Můžete ho vybrat i výslovně přes **@skill-creator**.
   b) V editoru: **Plugins › Skills** › vytvoření nového skillu a vyplnění popisu a pokynů.
   c) Pokročilé, zatím přeskočte: nahrání hotového skillu (složka se souborem `SKILL.md`). Nahraný skill ChatGPT proskenuje a označí **Needs Review** nebo **Blocked**.
4) Zkontrolujte, kam se skill uložil. Osobní skilly se mezi desktopem a webem nesynchronizují.

| Kde skill vytvoříte | Kam se uloží | Kde ho uvidíte |
|---|---|---|
| Work v desktopové aplikaci | složka na počítači (`.codex\skills` nebo `.agents\skills` v uživatelské složce) | jen desktopová aplikace a Codex na tomto počítači |
| Chat na webu | účet, **Plugins › Skills › Created by me** | web a mobil, jde sdílet ve workspace |
| Skill v pluginu (`@Plugin Creator`) | účet, jako plugin | Chat i Work na webu, desktopu i mobilu |

   Skill pro kolegy nebo pro víc zařízení proto tvořte na webu nebo jako plugin. U skillu z účtu si přečtěte v **Created by me** jeho popis: kdy se má použít a kdy ne.
5) Vyzkoušejte ho v novém chatu přes **@** na třech vstupech:
   a) běžný smyšlený podklad,
   b) podklad, ve kterém chybí důležitý údaj (skill se má zeptat, ne domýšlet),
   c) úplně jiný text (skill nemá převzít obsah z minulého příkladu).
6) Opravte, co nefunguje. Řekněte přesně, co změnit a co zachovat, a test zopakujte.
7) Sdílejte po krocích. Nejdřív skill používejte jen sami. Pak ho nasdílejte jedné osobě a nechte ji vyzkoušet krok 5. Až potom skupině nebo celému workspace. Sdílený skill kolegové najdou v **Shared with me** nebo **Shared by {workspace}**. Skill nesdílí vaše připojené účty. Každý kolega připojí svoje.
8) Skill si najde vhodný úkol i sám. Při prvních testech ho ale vybírejte výslovně, ať víte, že běží.

## Příklad

Vytvoření skillu (škola):

```
Vytvoř mi skill „Pracovní list z textu“.
Vstupy: text, ročník, počet otázek. Kroky: ověř, že máš všechny vstupy, navrhni otázky jen na informace z textu, zkontroluj každou odpověď proti textu, klíč dej jako samostatný soubor. Když chybí ročník nebo text, zeptej se. Nic si nevymýšlej a nepoužívej jména skutečných žáků.
Vzorový výsledek přikládám. Nejdřív mi ukaž návrh popisu, kdy skill použít a kdy ne.
```

Vytvoření skillu (kancelář):

```
Vytvoř mi skill „Zápis z porady“.
Vstup: poznámky z porady. Výstup: tabulka rozhodnutí, úkol, kdo, do kdy a pod ní seznam nejasností. Chybějící termín nebo jméno označ „neuvedeno“. Nic neodesílej a nesdílej.
Nejdřív mi ukaž návrh pokynů skillu ke kontrole.
```

Test chybějícího vstupu:

```
@[název skillu] Udělej pracovní list.
```

Správně: skill se zeptá na text a ročník a nic nevytvoří.

## Když to chybí

- Chybí **Skills** nebo **Plugins**: dostupnost závisí na tarifu, platformě a nastavení workspace. Uložte postup jako prompt a šablonu do projektu a vkládejte je do chatu. Je to plnohodnotná náhradní cesta.
- Skill je **Needs Review** nebo **Blocked**: obraťte se na správce workspace. Skill zatím nepoužívejte.
- Kolega skill nevidí: zkontrolujte, komu jste ho nasdíleli, a jestli správce sdílení v workspace dovoluje.
- ChatGPT tvrdí, že skill vytvořil, ale v **Created by me** není: když jste byli ve Work na desktopu, skill je místní na počítači (krok 4). Jinak nevznikl; nechte si vrátit text pokynů a vytvořte ho v editoru.
- Skill z desktopu nevidíte na webu: to je správně, osobní skilly se nesynchronizují. Vytvořte ho znovu na webu, nebo ho zabalte do pluginu.
- Místní skill se v novém chatu nenačte: zavřete a znovu otevřete aplikaci.

## Zdroj a stav

- Skills, záložky, skill-creator v účtu od začátku, tři způsoby vytvoření, sdílení, kontrola nahraného skillu: https://help.openai.com/en/articles/20001066, stav k 2. 11. 2026, FAKT.
- Vyvolání přes @, + nebo Plugins: https://help.openai.com/articles/20001256, stav k 2. 11. 2026, FAKT.
- Přesný název tlačítka pro nový skill v editoru: SIGNAL, ověřte na účtu.
- Skilly v ChatGPT pro Business, Enterprise, Healthcare a Edu; skill může obsahovat instrukce, příklady, podpůrné soubory a kód; vytvoření Create with chat, Create with editor, Upload from your computer: https://help.openai.com/en/articles/20001066, stav k 3. 11. 2026, FAKT (článek otevřený celý).
- Stavba složky `SKILL.md`, `scripts/`, `references/`, `assets/`; skill je formát, plugin je jednotka k šíření: https://learn.chatgpt.com/docs/customization/overview, stav k 3. 11. 2026, FAKT.
- Že skill v cloudu nemá přístup k počítači: PŘEDPOKLAD podle toho, jak cloud funguje.
- Že ostatní tarify mají skilly jen místně: PŘEDPOKLAD, nápověda jmenuje jen tarify se skilly v účtu.
- Osobní skilly se mezi desktopem a webem nebo mobilem nesynchronizují: https://help.openai.com/en/articles/20001066, stav k 3. 11. 2026, FAKT.
- Samostatný skill jen v desktopové aplikaci, Codex CLI a IDE; skill v pluginu i v Chat a Work na webu, desktopu a mobilu: https://learn.chatgpt.com/docs/build-skills, stav k 3. 11. 2026, FAKT pro místní skilly. ROZPOR s nápovědou 20001066, podle které skill vytvořený v účtu (Business a vyšší) funguje i na webu; platí nápověda, dokumentace popisuje skilly Codexu.
- Skill vytvořený ve Work na desktopu se uložil do `.codex\skills` na počítači: zkouška 3. 11. 2026, FAKT pro tento počítač; dokumentace uvádí `.agents/skills`.
- Pravidlo „aspoň třikrát vyzkoušený postup“ je doporučení příručky.
