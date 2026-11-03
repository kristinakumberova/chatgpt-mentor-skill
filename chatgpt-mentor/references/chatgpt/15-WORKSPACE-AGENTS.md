# Workspace agents a práce v týmu

Sdílený agent bude dělat opakovanou týmovou práci, i podle plánu, a zápisy předtím schválíte.

## Kde v aplikaci

- Postranní panel › **Agents**: části **Recently used**, **Built by me**, **Team directory**.
- Nový agent: **Agents › Create** (popis nebo **Start blank**), nebo **Browse templates › Use template**.
- V editoru agenta: **Preview** (vyzkoušení), **Tools › + Add tool**, **Channels**, **Create** a u hotového agenta **Update**.
- Jen Business a Enterprise. V Enterprise jsou agenti po spuštění vypnutí a zapíná je správce.
- Co dalšího jde v týmu sdílet: projekty (`09-PROJEKTY.md`), skills (`11-SKILLS.md`), Sites (`16-SITES-A-PAGES.md`).

Agent je o stupeň dál než skill a plugin (`20-POJMY.md`): má vlastní pokyny, model, nástroje, plán a kanály.

## Postup

1) Vyberte práci, kterou tým opakuje a kterou už umíte udělat ručně nebo skillem. Například týdenní souhrn úkolů z porad, kontrola, jestli každá třída odevzdala plán, nebo odpovědi na časté dotazy kolegů.
2) Založte agenta: **Agents › Create**, popište, co má dělat, projděte navržený plán a zvolte **Build this agent**. Nebo začněte šablonou (**Browse templates**).
3) V editoru zvolte model a míru přemýšlení a dejte agentovi jen to, co úkol potřebuje:
   a) skills s postupem,
   b) aplikace jen pro potřebné zdroje (například jedna složka na Google Drive nebo SharePointu), případně vlastní MCP nebo soubory,
   c) další nástroje jen když je úkol potřebuje (vyhledávání na webu, generování obrázků),
   d) pokyny: co dělat, co nikdy nedělat, komu výsledek patří.
4) U každé aplikace zvolte, pod čím agent pracuje:
   a) **End-user account**: každý, kdo agenta spustí, se přihlásí svým účtem. Doporučeno.
   b) **Agent-owned account**: agent používá jedno sdílené připojení. Použijte servisní účet, ne osobní, a jen s nutným přístupem.
5) Zápisy nechte na **Always ask** (výchozí). Agent se před úpravou nebo odesláním zeptá. **Never ask** nebo vlastní schvalování jen u neškodných akcí.
6) Přidejte omezení akcí (action constraints): popište pravidlo v editoru, například „e-mail posílej jen na adresy v doméně školy“ nebo „čti jen dokument Rozvrh“. Omezení hlídá, co agent po aplikaci chce, ne co mu aplikace vrátí.
7) Vyzkoušejte agenta v **Preview** na smyšlených nebo cvičných datech. První běh berte nanečisto: nic se nemá zapsat, jen navrhnout.
8) Plán: **Channels › ChatGPT › Add schedule**, typ a četnost. Před plánem aspoň dva ruční běhy se zkontrolovaným výsledkem.
9) Přístup: **Private to me**, **Anyone at [organizace] with the link**, nebo **Publish to [organizace] directory**. Začněte soukromě, pak odkaz pro jednoho kolegu, až potom adresář.
10) Volitelně: **Add channel** pro Slack (může schvalovat správce Slacku), nebo spouštění přes API z jiného systému (token vytváří správce).
11) Určete člověka, který za agenta odpovídá: kontroluje výsledky, upravuje pokyny a ví, kdy agenta vypnout.
12) Počítejte s náklady. Agenti se v Business platí kredity. Kolik to stojí, ověřte u správce.

## Příklad

Pokyny agenta (kancelář):

```
Jsi agent „Souhrn porad“ pro oddělení [název].
Každé pondělí v 8:00 přečti na SharePointu ve složce [Porady] zápisy z minulého týdne a připrav souhrn: rozhodnutí, otevřené úkoly, kdo, do kdy. Úkol bez termínu označ „neuvedeno“.
Smíš jen číst. Souhrn ulož do dokumentu „Souhrn porad – [týden]“ jen po mém schválení. Nikomu nic neposílej. Když složku neotevřeš, napiš to a skonči.
```

Pokyny agenta (škola):

```
Jsi agent „Kontrola plánů“ pro sborovnu.
Na požádání projdi na Google Disku složku [Tematické plány 2026/27] a vypiš tabulku: předmět, ročník, plán nahrán ano/ne, datum poslední změny. Obsah plánů nehodnoť a neměň. Údaje o žácích ve výstupu nepoužívej.
```

Omezení akce (napište v editoru):

```
Přidej omezení: e-mail smí agent poslat jen na adresy v doméně [skola.cz]. Čtení na Disku jen ve složce [Tematické plány 2026/27].
```

Test nanečisto:

```
Spusť se nanečisto: řekni, co bys udělal, které soubory bys otevřel a co bys kam zapsal. Nic nezapisuj.
```

## Když to chybí

- Chybí **Agents**: tarif nebo správce je nemá zapnuté. Použijte skill a naplánovanou úlohu (`11-SKILLS.md`, `14-NAPLANOVANE-ULOHY.md`).
- Agent neotevře složku: aplikace není připojená, nebo nemáte k souboru oprávnění (`13-KONEKTORY-GOOGLE-MICROSOFT.md`).
- Kolega agenta nevidí: zkontrolujte přístup (krok 9) a jestli je kolega ve stejném workspace.
- Agenta s plánem jste upravili, ale běží postaru: u hotového agenta uložte změny přes **Update**.
- Nemáte kredity: zeptejte se správce workspace.

## Zdroj a stav

- Agents, části Recently used, Built by me, Team directory, šablony, Create a Build this agent, Preview, Update, model a míra přemýšlení, nástroje (aplikace, vlastní MCP, skills, soubory, web, obrázky), End-user a Agent-owned account, Always ask a Never ask, action constraints, Add schedule, přístup Private / odkaz / adresář, Slack, API, v Enterprise vypnuté po spuštění: https://help.openai.com/en/articles/20001143, stav k 3. 11. 2026, FAKT (článek otevřený celý).
- Všeobecná dostupnost v Business od 22. 4. 2026 a placení kredity od 6. 5. 2026: https://openai.com/index/introducing-workspace-agents-in-chatgpt, stav k 2. 11. 2026, SIGNAL. Aktuální cenu ověřte na https://chatgpt.com/pricing.
- Dřívější popisky sdílení **Can chat** a **Can edit** nápověda 3. 11. 2026 neuvádí; platí volby z kroku 9.
- Ukázky agentů z praxe zatím nejsou. Příklady jsou návrh příručky, na účtu nevyzkoušené, SIGNAL.
