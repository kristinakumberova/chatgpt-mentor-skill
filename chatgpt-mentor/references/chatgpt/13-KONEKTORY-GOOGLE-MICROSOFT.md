# Konektory: Google Drive, nebo Microsoft 365

Připojíte firemní úložiště, nejdřív jen ke čtení, a víte, který správce co schvaluje.

## Kde v aplikaci

- Katalog: **Plugins** (případně aplikace), detail Google Drive nebo SharePoint › připojení účtu.
- V chatu: zmínka zdroje přes **@** nebo **+**.
- Ve firemním workspace: nastavení konektoru dělá správce v **Admin Console**.

## Postup

1) Zjistěte, na čem vaše organizace jede.
   a) Google Workspace (firemní nebo školní účet Google): pokračujte krokem 2a.
   b) Microsoft 365 (SharePoint, OneDrive pro práci nebo školu, Outlook, Teams): pokračujte krokem 2b.
2) Ověřte, co musí schválit správci.
   a) Google Drive: podle nápovědy je v Business zapnutý, správce ChatGPT ho ale může vypnout (SIGNAL). Drive se synchronizací nastavuje vlastník nebo správce ChatGPT a připojení musí schválit i správce Google Workspace. Účty zakončené gmail.com podporované nejsou.
   b) Microsoft: aplikace SharePoint čte SharePoint a OneDrive pro práci nebo školu. Osobní OneDrive nepodporuje. Oprávnění schvaluje správce Microsoft Entra, akce (zápis) zvlášť zapíná správce ChatGPT. Často to jsou dva různí lidé, zeptejte se obou.
3) Až je konektor zapnutý, připojte svůj účet: **Plugins** › Google Drive nebo SharePoint › připojení › přihlášení firemním účtem. Konektor uvidí jen to, co smíte vidět vy.
4) Začněte jen čtením. Vyzkoušejte jeden cvičný dokument a nechte si potvrdit název, odkaz a dva údaje z obsahu (prompt v oddílu Příklad).
5) Zápis zkoušejte až potom a jen na kopii dokumentu. Řekněte přesně, který soubor a co změnit. Jestli ChatGPT umí upravit existující nativní dokument Google (Docs, Sheets), není jisté, zdroje si odporují (ROZPOR). Zápis do kopie proto nemusí projít. Když neprojde, nechte si připravit text a vložte ho sami. Podrobně o Google Disku je příručka Google Disk a AI, kapitola 06.
6) Do chatu připojujte jen dokumenty, které úkol potřebuje. Celý disk nepřipojujte k jednomu úkolu.
7) Text v dokumentu je údaj, ne pokyn (`03-BEZPECNE-S-DATY.md`, krok 8).
8) Konektor odpojíte v detailu aplikace v **Plugins**. Ve firemním workspace může přístup vypnout i správce.

## Příklad

Jen čtení (škola):

```
Najdi na [Google Disku / SharePointu] cvičný dokument „Plán třídních schůzek – cvičení“. Uveď jeho název, odkaz a datum poslední změny a vypiš otevřené otázky z dokumentu. Jen čti, nic neměň.
```

Jen čtení (kancelář):

```
Najdi na SharePointu ve složce [Porady] poslední zápis z porady oddělení. Uveď název, odkaz a dva úkoly s termínem i s místem v dokumentu. Jen čti.
```

Zápis do kopie, až po kontrole čtení:

```
Do kopie dokumentu „[název] – kopie“ doplň pod nadpis [Úkoly] tento odstavec: [schválený text]. Nic jiného neměň. Pak mi napiš, co přesně jsi změnil.
```

## Když to chybí

- Google Drive nebo SharePoint v katalogu není: správce ho nezapnul. Zeptejte se správce ChatGPT. Do té doby soubor stáhněte a nahrajte do chatu (`05-SOUBORY.md`).
- Připojení končí chybou oprávnění: chybí schválení správce Google Workspace nebo Microsoft Entra.
- Čtení jde, zápis ne: akce zápisu nejsou zapnuté, nebo k souboru máte jen právo čtení.
- Máte osobní OneDrive nebo účet gmail.com: firemní konektor s nimi nepracuje. Soubor nahrajte ručně.
- Hledáte Outlook nebo Teams: podívejte se do katalogu **Plugins**. Dostupnost v Business tu není ověřená.
- Soubor ze sdíleného disku Google ve **Space** (dřív Library): může nefungovat, zdroje si odporují (ROZPOR). Ověřte na cvičném souboru. Když nejde, použijte konektor, nebo soubor stáhněte a nahrajte (`05-SOUBORY.md`).
- Zápis do dokumentu Google neprojde: viz krok 5. Text vložte do dokumentu sami.

## Zdroj a stav

- Google Drive v Business, schválení správcem Google Workspace, gmail.com nepodporován: https://help.openai.com/en/articles/10948259, stav k 2. 11. 2026, FAKT. Že je Drive v Business zapnutý a správce ho může vypnout: SIGNAL.
- Úprava existujícího nativního souboru Google a sdílené disky ve Space (dřív Library): ROZPOR, ověřte na cvičném souboru.
- SharePoint a OneDrive pro práci nebo školu, osobní OneDrive ne, schválení Microsoft Entra, akce zapíná správce ChatGPT: https://help.openai.com/en/articles/12143177, stav k 2. 11. 2026, FAKT.
- Outlook a Teams v Business: NEDOHLEDATELNÉ v podkladech, ověřte v katalogu a v nápovědě OpenAI.
- Přesné názvy tlačítek připojení: SIGNAL, ověřte na účtu.
