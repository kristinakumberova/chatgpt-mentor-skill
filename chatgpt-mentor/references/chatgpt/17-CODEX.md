# Codex pro netechniky

Codex použijete tam, kde Work nestačí: na práci nad celou složkou souborů ve vašem počítači.

## Kde v aplikaci

- Desktopová aplikace › výběr **Codex** (vedle **ChatGPT**).
- Místní projekt: přidání složky (**Add folder**).
- Pravidla pro složku: soubor `AGENTS.md` ve složce.
- Skill v Codexu: napíšete **$** a název, například `$skill-creator`.

## Postup

1) Použijte Codex, když:
   a) potřebujete projít nebo upravit hodně souborů najednou (seřadit, přejmenovat, sjednotit formát),
   b) z mnoha dokumentů vytáhnout údaje do jedné tabulky,
   c) chcete, aby pravidla pro práci ležela ve složce a platila pokaždé stejně.
   Na jeden dokument nebo jednu otázku stačí Chat nebo Work.
2) Udělejte si kopii složky, se kterou bude Codex pracovat. První pokusy dělejte jen na kopii.
3) V Codexu přidejte tuto kopii jako projekt (**Add folder**). Codex vidí jen složky, které mu přidáte.
4) Do složky můžete dát soubor `AGENTS.md` s pravidly práce: jazyk, co nikdy neměnit, jak pojmenovávat soubory. Codex ho přečte na začátku každé práce. Nechte si ho napsat (prompt v oddílu Příklad).
5) Zadejte úkol a řekněte, ať nejdřív ukáže plán a seznam souborů, které změní. Až plán schválíte, ať pokračuje.
6) Po práci si nechte vypsat, co se změnilo. Otevřete pár souborů a zkontrolujte je sami.
7) Codex a Work čerpají ze stejného limitu. Velká práce nad stovkami souborů ho může rychle vyčerpat.
8) Do složky pro Codex nedávejte soubory, které do ChatGPT nesmíte vkládat (`03-BEZPECNE-S-DATY.md`).

## Příklad

Pravidla do `AGENTS.md`:

```
Napiš mi soubor AGENTS.md pro tuto složku. Pravidla: piš česky, originály nikdy nepřepisuj, výsledky ukládej do podsložky „vystup“, názvy souborů ve tvaru RRRR-MM-DD-nazev, před každou změnou ukaž plán a počkej na schválení. Nic jiného ve složce neměň.
```

Údaje z mnoha souborů (kancelář):

```
Ve složce jsou smyšlené smlouvy ve formátu PDF. Z každé vypiš do tabulky XLSX: název souboru, smluvní strana, datum podpisu, datum konce, výpovědní lhůta. Když údaj v souboru není, napiš „neuvedeno“. Originály neměň. Nejdřív mi ukaž plán.
```

Úklid příprav (škola):

```
Ve složce jsou moje přípravy na hodiny z minulého roku. Navrhni, jak je seřadit do podsložek podle ročníku a měsíce, a ukaž seznam přesunů. Nic nepřesouvej, dokud neřeknu „ano“.
```

## Když to chybí

- Nemáte Codex: nainstalujte desktopovou aplikaci ChatGPT, nebo se zeptejte správce, jestli ho máte v tarifu. Menší práci zvládne Work s nahranými soubory.
- Codex nevidí soubory: složka není přidaná jako projekt. Přidejte ji znovu přes **Add folder**.
- Codex nepoužívá pravidla: soubor se musí jmenovat přesně `AGENTS.md` a ležet v hlavní přidané složce (`09-PROJEKTY.md`, krok 10).
- Codex nedrží vaše osobní pokyny: pokyny z Personalization se do Codexu nepřenesou, Codex má globální `AGENTS.md` (`07-VLASTNI-POKYNY.md`).
- Skill z ChatGPT v Codexu nenajdete: místní skill a skill v ChatGPT nemusí být totéž. Vyvolejte ho názvem s **$**, nebo ho vytvořte znovu přes `$skill-creator`.

## Zdroj a stav

- Codex a sdílený limit s Work: https://learn.chatgpt.com/docs/use-chatgpt, ověřeno 7. 10. 2026, stav k 2. 11. 2026, FAKT.
- Místní projekt a Add folder: https://learn.chatgpt.com/docs/projects, ověřeno 7. 10. 2026, FAKT.
- AGENTS.md: https://learn.chatgpt.com/docs/agent-configuration/agents-md, ověřeno 7. 10. 2026, FAKT.
- Skills v Codexu přes $: https://learn.chatgpt.com/docs/build-skills, ověřeno 7. 10. 2026, FAKT.
- Příklady jsou návrh příručky, na účtu nevyzkoušené, SIGNAL.
