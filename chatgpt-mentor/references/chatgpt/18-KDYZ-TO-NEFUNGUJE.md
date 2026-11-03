# Když to nefunguje

Podle toho, co vidíte, poznáte, jestli chybí tarif, nastavení správce, nebo oprávnění, a víte, koho se zeptat.

## Kde v aplikaci

- Vaše nastavení: **Settings**.
- Nastavení workspace: **Admin Console**, jen vlastník a správce.
- Připojené aplikace: **Plugins**.

## Postup

1) Zapište si přesně, co vidíte: chybějící tlačítko, chybovou hlášku, nebo špatný výsledek. Přidejte, v jaké aplikaci jste (web, desktop, mobil) a v jakém workspace.
2) Najděte svůj případ v tabulce.

| Co vidíte | Pravděpodobná příčina | Co udělat |
|---|---|---|
| tlačítko nebo funkce v nabídce chybí | tarif ji nemá, správce ji nezapnul, nebo se zavádí postupně | zkuste webovou aplikaci, pak se zeptejte správce |
| kolega funkci má, vy ne | jiný workspace, jiná role, nebo postupné zavádění | porovnejte workspace v nabídce účtu, zeptejte se správce |
| chyba oprávnění u Google Drive | chybí schválení správce Google Workspace, nebo máte účet gmail.com | správce Google Workspace (`13-KONEKTORY-GOOGLE-MICROSOFT.md`) |
| chyba oprávnění u SharePointu nebo OneDrivu | chybí schválení správce Microsoft Entra, nebo jde o osobní OneDrive | správce Microsoft Entra (`13-KONEKTORY-GOOGLE-MICROSOFT.md`) |
| čtení jde, zápis ne | akce zápisu nejsou zapnuté, nebo máte k souboru jen čtení | správce ChatGPT, vlastník souboru |
| ChatGPT odpovídá, jako by soubor neviděl | soubor se nenačetl celý, sken, obrázek v PDF v projektu | nahrát přímo do chatu, ověřit dvěma údaji (`05-SOUBORY.md`) |
| ChatGPT pořád připomíná starou věc | uložená vzpomínka nebo minulý chat | smazat vzpomínku v Memory (`06-PAMET.md`) |
| volba paměti nejde změnit | nastavení vlastníka workspace | vlastník workspace (`06-PAMET.md`) |
| nový skill není v nabídce | skill nevznikl, nebo je Needs Review či Blocked | Plugins › Skills › Created by me, správce (`11-SKILLS.md`) |
| nejde vytvořit vlastní GPT | zakládání nových GPT skončilo | udělejte skill (`11-SKILLS.md`, `12-VLASTNI-GPT-PREVOD.md`) |
| nejde přidat další naplánovaná úloha | Business má strop 10 aktivních úloh | jednu pozastavit nebo smazat (`14-NAPLANOVANE-ULOHY.md`) |
| agent nebo úloha hlásí chybu přístupu | konektor se odpojil, změnilo se oprávnění | připojit znovu (`13-KONEKTORY-GOOGLE-MICROSOFT.md`) |
| Site nečte data z Drive nebo SharePointu | správce nezapnul Allow use in Sites | správce ChatGPT (`16-SITES-A-PAGES.md`) |
| došel limit | Work a Codex čerpají ze stejného limitu | počkat, rozdělit úkol, zeptat se správce |
| výsledek je špatně, ale vypadá dobře | zadání bez podkladů nebo bez kontroly | zadání z pěti částí a kontrola (`04-ZADANI-A-KONTROLA.md`) |

3) Když případ v tabulce není, zeptejte se v tomto projektu a přidejte, co jste zapsali v kroku 1.
4) Když nepomůže ani to, napište správci workspace (prompt v oddílu Příklad). Správce má Admin Console a vidí, co je zapnuté.
5) Když jde o chybu aplikace (padá, nenačte se), zkuste se odhlásit a přihlásit, aktualizovat aplikaci, nebo jinou aplikaci (web místo desktopu). Pak nápověda OpenAI.

## Příklad

Popis problému do chatu:

```
Něco mi nefunguje. Aplikace: [web / desktop / mobil]. Workspace: [název]. Chtěla jsem: [co]. Vidím: [přesná hláška nebo co chybí].
Podle příručky mi řekni nejpravděpodobnější příčinu a jeden krok, který mám zkusit. Nic nenastavuj.
```

Zpráva správci, kterou pošlete sami:

```
Dobrý den, v ChatGPT [Business] mi nefunguje [funkce]. Aplikace: [web / desktop / mobil]. Hláška: [text]. Kolega [má / nemá] totéž. Můžete prosím ověřit, jestli je [funkce / konektor] pro mě zapnutá? Děkuji.
```

## Když to chybí

- Nevíte, kdo je správce: v Business vlastník nebo správce workspace, ve škole obvykle IT nebo vedení (`01-NEZ-ZACNETE.md`).
- Správce neví: odkažte ho na nápovědu OpenAI ke konkrétní funkci. Odkazy jsou v oddílu Zdroj a stav příslušné kapitoly.

## Zdroj a stav

- Souhrn příčin podle kapitol 05, 06, 11 až 16 této příručky, stav k 2. 11. 2026.
- Admin Console v Business: https://help.openai.com/en/articles/11391654, stav k 2. 11. 2026, FAKT.
- Nápověda OpenAI: https://help.openai.com.
