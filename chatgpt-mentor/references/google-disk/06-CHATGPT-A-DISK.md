# ChatGPT a Google Disk

Kapitola vás provede připojením Disku k ChatGPT, prvním čtením a prvním zápisem. ChatGPT pak vidí všechno, k čemu má váš Google účet přístup.

## Kde

- Aplikace ChatGPT na počítači › **Plugins** v postranním panelu (v některých verzích pod **Customize**) › **Google Drive**. Web má Plugins taky. Mobilní ovládání zde ověřené není.
- V chatu: napište **@** a vyberte **Google Drive**. Dokumenty, Tabulky a Prezentace Google jdou přes tentýž plugin.
- Soubory z Disku ve **Space** (dřív Library): postranní panel Space › filtr **Google Drive**.
- Firemní nastavení: správce v **Admin** › **Workspace connections**, u Enterprise **Safety & Security Controls** v nastavení aplikace.

## Postup

1) Zjistěte, co máte.
   a) **ChatGPT Business:** akce Disku jsou podle nápovědy zapnuté, správce je může vypnout (SIGNAL).
   b) **ChatGPT Enterprise nebo Edu:** akce Disku jsou vypnuté, dokud je nezapne správce.
   c) **Osobní tarif ChatGPT:** připojíte si Disk sami. Účty gmail.com ChatGPT Business podle nápovědy nepodporuje, osobní Google účet tedy připojíte jen k osobnímu tarifu (SIGNAL). Firemní soubory přes soukromý účet nepřipojujte.
   Správce může povolit čtení a zápis zvlášť.

2) Připojte Disk: **Plugins** › **Google Drive** › tlačítko pro přidání nebo připojení › vyberte **firemní** Google účet › přečtěte, jaká oprávnění ChatGPT chce › **Povolit**. Přihlášení může přijít až v chatu. Je-li plugin už v **Installed**, pokračujte krokem 3.

3) Vyzkoušejte čtení na cvičném souboru. Vytvořte Google dokument „Cvičný soubor AI“, napište do něj tři věty a kódové slovo `G-ALFA`. Pak nový chat › **@** › **Google Drive** › první prompt z části Příklad. Odpověď porovnejte s dokumentem.

4) Pracujte s podklady. Do promptu dávejte odkaz na konkrétní soubor nebo složku a chtějte název a odkaz souboru, který ChatGPT skutečně otevřel.

5) Zápis zkoušejte zvlášť a nejdřív bez rizika.
   a) **Nový soubor:** nechte ChatGPT vytvořit nový Google dokument ve složce **02_Rozpracovane** (druhý prompt v části Příklad). Složku založte podle 02-SLOZKY-A-NAZVY.md, krok 2. Odkaz otevřete a zkontrolujte složku i obsah.
   b) **Úprava existujícího souboru:** podle nápovědy ChatGPT upravuje nativní Google soubory, jeden návod tvrdí, že jen kopíruje text (ROZPOR). **Ověřte na cvičném souboru:** kopie souboru z kroku 3, jedna změněná věta, porovnání v historii verzí (04-VERZE-HISTORIE-A-SABLONY.md, krok 2).
   c) ChatGPT se může před akcí zeptat. Přečtěte, co přesně chce udělat, a teprve pak potvrďte.

6) Sdílené disky: **ověřte na cvičném souboru.** Starší zprávy uvádějí, že Space (dřív Library) sdílené disky nepokrývá. Správce Enterprise je povoluje jen celé podle ID disku, ne po složkách (ROZPOR, u Business nedohledáno). Dejte cvičný soubor na sdílený disk a zopakujte krok 3.

7) Space (dřív Library): soubor z Disku si drží oprávnění z Googlu, ale obsah zkopírovaný na stránku Space vidí každý s přístupem ke stránce.

8) Odpojení: **Plugins** › **Google Drive** › odpojit. Vypnutí v ChatGPT nezruší oprávnění v Googlu, odeberte ho i tam (10-BEZPECNOST-A-KDYZ-NECO-NEJDE.md, krok 6).

## Příklad

Škola: z cvičné kopie tematického plánu vypsat otevřené otázky. Kancelář: z cvičné kopie podkladů k poradě vypsat nerozhodnuté body.

Čtení:

```
Pomocí Google Drive otevři tento cvičný dokument: [odkaz].
Uveď jeho přesný název, kódové slovo a dvě konkrétní věty z textu.
Když obsah nepřečteš, řekni to. Nic neměň.
```

Zápis do nového souboru:

```
Z dokumentu [odkaz] vypiš otevřené otázky a ulož je jako nový Google dokument
s názvem 2026-11-02_otevrene-otazky_navrh do složky [odkaz na složku 02_Rozpracovane].
Původní dokument neměň. Vrať odkaz na skutečně uložený soubor.
```

## Když to chybí

| Co vidíte | Co udělat |
|---|---|
| Google Drive není v Plugins | Zkontrolujte, že jste v pracovním účtu ChatGPT. Dostupnost ověřte u správce. |
| Odkaz se neotevře | Připojený Google účet nemá k souboru právo. Zkontrolujte, který účet je připojený. |
| Čtení funguje, zápis ne | Správce zápis nepovolil, nebo nemáte v Googlu právo upravovat. Výsledek vložte do dokumentu ručně. |
| Soubor ze sdíleného disku nenajde | Viz krok 6. Mezitím soubor stáhněte a přiložte do chatu. |
| ChatGPT tvrdí, že soubor upravil, ale změna není | Otevřete historii verzí. Co tam není, se nestalo. |

## Zdroj a stav

- Plugins a Google Drive: https://learn.chatgpt.com/docs/plugins (FAKT)
- Tarify a správa přístupu k Disku: https://help.openai.com/en/articles/10948259 a https://help.openai.com/en/articles/20001608-managing-google-drive-access-in-chatgpt (SIGNAL, stránky vracely chybu 403, převzato z výpisu vyhledávače)
- Firemní připojení: https://learn.chatgpt.com/docs/enterprise/shared-connections a https://learn.chatgpt.com/docs/enterprise/apps-and-connectors (FAKT / SIGNAL)
- Space (dřív Library): https://learn.chatgpt.com/docs/space (FAKT)
- Stav k 2. 11. 2026. Zápis do existujících souborů a sdílené disky v Business: ROZPOR, ověřte na cvičném souboru.
