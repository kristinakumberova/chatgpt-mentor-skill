# Paměť: co si pamatuje a jak ji řídit

Paměť máte zapnutou a víte, co si ChatGPT pamatuje, jak vzpomínku opravit nebo smazat a kdy pracovat bez paměti.

## Kde v aplikaci

- **Settings › Personalization › Memory**: dva přepínače, **Reference saved memories** (uložené vzpomínky) a **Reference chat history** (minulé chaty), dále **Memory summary** a správa uložených vzpomínek. Název prvního přepínače ověřte na účtu.
- Pod odpovědí: **Sources** ukáže, ze které vzpomínky nebo z kterého minulého chatu odpověď čerpala. Nejsou to soubory projektu ani soubory v **Space** (dřív Library), ty najdete v projektu a ve Space. Volba **Don't mention this again** zabrání, aby se věc znovu objevovala.
- Nový projekt: volba **project-only memory** při založení (`09-PROJEKTY.md`).
- Dočasný chat: nový chat › **Temporary** (`03-BEZPECNE-S-DATY.md`).

## Postup

1) Počítejte s tím, že paměť je zapnutá. ChatGPT bere v úvahu:
   a) minulé chaty (přepínač **Reference chat history**),
   b) uložené vzpomínky (přepínač **Reference saved memories**),
   c) vlastní pokyny (`07-VLASTNI-POKYNY.md`),
   d) soubory ve **Space** (dřív Library),
   e) připojené aplikace.
2) Podívejte se, co si pamatuje: **Settings › Personalization › Memory** › **Memory summary**. Nebo se zeptejte v chatu (prompt v oddílu Příklad).
3) Když je vzpomínka špatně nebo zastaralá:
   a) v **Memory** ji opravte nebo smažte,
   b) pod odpovědí, která ji použila, otevřete **Sources**. U vzpomínky by měla být volba **Don't mention this again**, ověřte na účtu.
4) Když nechcete, aby si něco zapamatoval, otevřete dočasný chat **Temporary**. Dočasný chat vzpomínky nevytváří. Volba **Unpersonalized** navíc nepoužije ani stávající paměť.
5) Pro téma, které se nemá míchat s ostatními (třída, klient, jeden projekt), založte projekt s **project-only memory**. Chaty v něm čerpají jen z projektu. Volí se při založení projektu.
6) Když paměť nechcete vůbec, vypněte oba přepínače v **Memory** (**Reference saved memories** i **Reference chat history**). Počítejte s tím, že:
   a) vypnutí paměti chaty nesmaže,
   b) smazání chatu nesmaže vzpomínku, která z něj vznikla. Vzpomínku smažte v **Memory** zvlášť,
   c) smazanou vzpomínku může OpenAI držet v záznamech ještě až 30 dní.
7) Do paměti nepatří údaje, které do ChatGPT nesmíte vkládat vůbec (`03-BEZPECNE-S-DATY.md`). Paměť neslouží jako úložiště pravidel. Závazný postup patří do projektu nebo do skillu (`11-SKILLS.md`).
8) Ve firemním workspace může nastavení paměti omezit vlastník workspace. Když volba chybí nebo nejde změnit, je to jeho nastavení.
9) Desktopová aplikace má navíc **místní paměť Codexu**, oddělenou od paměti ChatGPT. Ve výchozím stavu je vypnutá; zapíná se v **Settings › Personalization › Enable Codex memories**, maže přes **Delete Codex memories**. Ukládá se na počítači do složky `.codex\memories` (soubory `MEMORY.md`, `memory_summary.md`) a Codex ji plní sám z hotových chatů. Ručně ji neupravujte.
   a) Chat na webu, v mobilu i na desktopu: paměť účtu (kroky 1 až 8).
   b) Work v cloudu: paměť účtu a workspace.
   c) Codex a Work na desktopu se zapnutou místní pamětí: místní paměť; co si pamatuje tam, Chat neví, a naopak. Na jiném počítači ani u kolegy není.
   Pro práci s údaji o žácích nebo klientech nechte místní paměť vypnutou: ukládá se do souboru na disku mimo workspace. Co si má AI pamatovat, napište výslovně do `AGENTS.md` nebo do pokynů.

## Příklad

Co si o mně pamatuje:

```
Vypiš, co si o mně pamatuješ a z čeho to víš (uložená vzpomínka, minulý chat, vlastní pokyny, soubor, připojená aplikace). Nic neměň a nic nemaž.
```

Uložení užitečné vzpomínky (škola):

```
Zapamatuj si: učím češtinu ve 4. a 5. třídě, pracovní listy chci na jednu stranu A4 a klíč vždy zvlášť. Žádné údaje o konkrétních žácích si nepamatuj.
```

Uložení užitečné vzpomínky (kancelář):

```
Zapamatuj si: zápisy z porad chci jako tabulku rozhodnutí, úkol, kdo, do kdy. Chybějící termín označ „neuvedeno“.
```

Kontrola, že se vzpomínka nepoužívá (po smazání v Memory):

```
Jaký formát mám rád u zápisů z porad? Když to nevíš z paměti, řekni to.
```

## Když to chybí

- Chybí **Memory** nebo jde jen zčásti nastavit: omezil ji vlastník workspace. Zeptejte se ho, nebo pracujte v projektu s **project-only memory**.
- Chybí **Memory summary** nebo **Sources**: zavádí se postupně. Použijte prompt „Vypiš, co si o mně pamatuješ“.
- Chybí **project-only memory**: použijte dočasný chat a podklady nahrajte do něj.

## Zdroj a stav

- Místní paměť Codexu oddělená od paměti ChatGPT, ve výchozím stavu vypnutá, Enable Codex memories, ukládání do `$CODEX_HOME/memories`, Work používá paměť účtu a workspace: https://learn.chatgpt.com/docs/customization/memories, stav k 3. 11. 2026, FAKT.
- Work na desktopu se zapnutou pamětí Codexu odpověděl na „Co si o mně pamatuješ?“ obsahem místního `MEMORY.md`, po vypnutí paměti Codexu už o těchto věcech nevěděl: zkouška 3. 11. 2026, FAKT pro tento počítač. Dokumentace píše, že Work místní paměť nepoužívá; platí to nejspíš jen pro cloudový Work.
- Smazání **Delete Codex memories**, soubory `MEMORY.md` a `memory_summary.md`: https://www.memorylake.ai/en/blogs/turn-on-codex-local-memories, https://recallium.ai/codex, stav k 3. 11. 2026, SIGNAL (u Kristiny soubory ověřeny).

- Paměť, zdroje paměti, volby Reference chat history, Memory summary, Sources, Don't mention this again, vypnutí a mazání, 30 dní v záznamech, správa vlastníkem workspace: https://help.openai.com/en/articles/8590148, stav k 2. 11. 2026, FAKT. Stránka se naposledy měnila 31. 10. 2026, další změny jsou pravděpodobné.
- Paměť jen pro projekt při založení: https://help.openai.com/en/articles/8555545, stav k 2. 11. 2026, FAKT.
- Prompty „Zapamatuj si“ a „Vypiš, co si pamatuješ“ jsou doporučení příručky, na účtu Business nevyzkoušené, SIGNAL.
- Že je volba Don't mention this again přímo u Sources pod odpovědí: SIGNAL, nápověda uvádí obě volby, jejich přesné umístění ověřte na účtu.
- Název přepínače Reference saved memories a přejmenování Library na Space: SIGNAL, ověřte na účtu.
