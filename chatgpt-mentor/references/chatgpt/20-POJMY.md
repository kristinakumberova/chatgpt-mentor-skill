# Pojmy: projekt, skill, plugin, GPT, MCP a hooky

Rozlišíte, co který pojem znamená, kde funguje a kdy po něm sáhnout.

## Kde v aplikaci

- Projekty: postranní panel › **Projects** (`09-PROJEKTY.md`).
- Skilly: **Plugins › Skills** (`11-SKILLS.md`).
- Pluginy: postranní panel › **Plugins**, v chatu přes **@**, **+** nebo **Plugins** v poli zadání.
- Hooky: jen Codex, v desktopové aplikaci **Settings › Hooks** nebo **Review hooks** (`17-CODEX.md`).

| Pojem | Co to je | Kde funguje | Jak se sdílí | Kdy po něm sáhnout |
|---|---|---|---|---|
| **Projekt** | místo pro jedno téma: chaty, soubory, pokyny, paměť | cloudová část v Chatu na webu, desktopu i mobilu; místní složka jen v místních chatech | sdílený projekt s kolegy | opakovaně pracujete nad stejnými podklady |
| **Skill** | složka s postupem: `SKILL.md`, případně podklady, šablony, skripty | v účtu jen Business, Enterprise, Healthcare, Edu; vytvořený ve Work na desktopu jen na tom počítači | z účtu přes **Share**; místní ne | opakujete stejný postup |
| **Plugin** | balíček skillů, připojených aplikací a šablon | Chat, Work i Codex na webu, desktopu i mobilu, podle tarifu a workspace | adresář **Plugins**: veřejné, workspace, osobní | skill má fungovat všude nebo pro tým, nebo potřebuje připojenou službu |
| **Agent workspace** | pracovník s vlastními pokyny, modelem, nástroji, plánem a kanály (Slack, API) | jen Business a Enterprise | soukromý, odkazem, nebo v adresáři organizace | práce má běžet sama podle plánu nebo pro celý tým (`15-WORKSPACE-AGENTS.md`) |
| **Vlastní GPT** | starší asistent s instrukcemi | končí 11. 12. 2026 | převod na plugin se skillem | nové nestavte (`12-VLASTNI-GPT-PREVOD.md`) |
| **MCP** | připojení ChatGPT k vlastnímu systému firmy (CRM, úkoly, databáze) | Business, Enterprise a Edu na webu | v Business ho přidává a zveřejňuje jen správce nebo vlastník | firma má systém, který žádná hotová aplikace nepokrývá |
| **Hooky** | skripty, které se spustí při události, například před použitím nástroje nebo na konci práce | jen Codex (příkazová řádka a desktopová aplikace) | soubor `hooks.json`; správce je může nastavit všem | hlídání a automatizace pro vývojáře; běžný uživatel je nepotřebuje |

## Jak to do sebe zapadá

- Plugin skill nenahrazuje, plugin skill obsahuje. Spouští se stejně, podle popisu skillu nebo přes **@**.
- Plugin může být i bez skillu, jen s připojenou aplikací.
- Hotové aplikace (Gmail, Google Drive, Slack) dostanete jako plugin z adresáře. Uvnitř aplikace běží přes MCP (SIGNAL), vy MCP neřešíte. Vlastní MCP server přidáváte, jen když chcete připojit systém, který v adresáři není.
- Přirovnání: skill je role nebo postup, plugin je sada rolí pro tým nebo klienta, agent workspace je role, která pracuje sama (plán, nástroje, schvalování zápisu).
- Hooky jsou pojistka, ne zámek. Hlídají jen to, na co jsou napojené. Uživatel je může vypnout; nevypnutelné jsou jen hooky, které nastaví správce. Nejbližší obdoba v ChatGPT jsou omezení akcí u agenta workspace (`15-WORKSPACE-AGENTS.md`, krok 6).

## Postup

1) Rozhodněte, co opakujete.
   a) Stejné podklady: projekt.
   b) Stejný postup: skill.
   c) Obojí: projekt a v něm skill.
2) Rozhodněte, kde to má fungovat (tarify u řádku Skill v tabulce).
   a) Jen pro vás na jednom počítači: skill z Work na desktopu stačí.
   b) Na webu a v mobilu: skill vytvořte na webu, nebo jako plugin.
   c) Pro kolegy: sdílený projekt, sdílený skill z účtu, nebo plugin ve workspace.
3) Potřebujete data z jiné služby (Disk, Slack, e-mail): hledejte plugin nebo aplikaci v **Plugins** (`13-KONEKTORY-GOOGLE-MICROSOFT.md`). Vlastní systém firmy přes MCP řeší správce.
4) Vlastní GPT nezakládejte. Existující převeďte do skillu nebo pluginu.
5) Hooky a MCP nechte správci nebo vývojáři.
6) Nový postup nejdřív odlaďte jako samostatný skill: upravíte ho v chatu a hned zkusíte. Až funguje na třech testech, zabalte ho do pluginu. Rovnou plugin jde také: `@Plugin Creator` a popis, co má umět.
7) Práce, která má běžet sama podle plánu nebo pro tým: agent workspace (`15-WORKSPACE-AGENTS.md`).

## Příklad

Otázka pro ChatGPT, když nevíte, co zvolit:

```
Popíšu ti práci, kterou opakuji. Doporuč, jestli z ní udělat projekt, skill, nebo plugin, a jednou větou proč. Zohledni, že ji chci používat [jen já na počítači / i v mobilu / s kolegy].
[popis práce]
```

## Na co lidé narážejí

- Slovo „plugin“ znamenalo v roce 2023 něco jiného. Starší články a videa popisují zaniklou funkci (SIGNAL).
- Lidé zaměňují projekt a skill. Projekt drží podklady, skill drží postup (SIGNAL, blogy).
- Návody na internetu si odporují v tom, který tarif co má. Platí aktuální článek nápovědy (SIGNAL).
- Skill z desktopu chybí na webu: osobní skilly se nesynchronizují (`11-SKILLS.md`, krok 4).

## Když to chybí

- Chybí **Plugins** nebo **Skills**: tarif nebo správce je nezapnul. Postup uložte do instrukcí projektu.
- Chybí volba přidat vlastní MCP server: v Business ho přidává jen správce nebo vlastník.
- Hooky v ChatGPT nenajdete: jsou jen v Codexu.

## Zdroj a stav

- Plugin obsahuje skilly, připojené aplikace, šablony a rozšíření; adresář na webu, desktopu i mobilu; záložky Public, Your workspace, Personal, Installed; vyvolání přes @, + nebo Plugins: https://help.openai.com/en/articles/20001256, stav k 3. 11. 2026, FAKT.
- Skilly, sdílení, osobní skilly se mezi desktopem a webem nesynchronizují: https://help.openai.com/en/articles/20001066, stav k 3. 11. 2026, FAKT.
- Vlastní MCP servery: Business, Enterprise a Edu na webu, v Business je vytváří a zveřejňuje jen správce nebo vlastník, přidání přes **Plugins › + › Add custom MCP server**: https://help.openai.com/en/articles/12584461, stav k 3. 11. 2026, FAKT.
- Hooky jsou „useful guardrail, not a complete enforcement boundary“, projektové hooky běží až po důvěře, uživatel je může vypnout, správce je nastaví v `requirements.toml`: https://learn.chatgpt.com/docs/hooks, stav k 3. 11. 2026, FAKT.
- Plugin může obsahovat jen skilly, jen aplikace, nebo obojí: https://help.openai.com/en/articles/20001256, stav k 3. 11. 2026, FAKT.
- Převod adresáře aplikací do adresáře pluginů 9. 7. 2026: výňatek z vyhledávání, SIGNAL.
- Že aplikace uvnitř běží přes MCP: Apps SDK, SIGNAL.
- Hooky: rozšíření Codexu, události, `hooks.json` a `config.toml`, **Settings › Hooks** v desktopové aplikaci, v cloudovém Work se příkazové hooky nepodporují: https://learn.chatgpt.com/docs/hooks, stav k 3. 11. 2026, FAKT.
- Skill je formát, plugin je jednotka k instalaci a šíření: https://learn.chatgpt.com/docs/customization/overview, stav k 3. 11. 2026, FAKT.
- Zkušenosti uživatelů (záměna projektu a GPT, starý význam slova plugin, rozpory v tarifech): https://www.theneuron.ai/explainer-articles/our-guide-to-ai-skills-projects-custom-gpts-agents-plugins-connectors-loops-and-codex-workflows/, https://blessingeffect.substack.com/p/how-i-use-projects-and-custom-gpts, https://www.chaindesk.ai/zh-cn/blog/custom-gpt-vs-projects, stav k 3. 11. 2026, SIGNAL. Vlákna na Redditu vyhledávání nenašlo.
- Konec vlastních GPT 11. 12. 2026: `12-VLASTNI-GPT-PREVOD.md`.
