# Navigátor příručky ChatGPT, Work a Codex

> Jednorázová verze pro Euroinstitut, stav k 3. 11. 2026. Neaktualizuje se sama; když něco nesedí s aplikací, platí nápověda OpenAI.

Složka s návody, podle kterých vám ChatGPT v projektu poradí, jak co použít a nastavit. Je pro běžné lidi ve firmě i ve škole, od prvního chatu po sdílené agenty.

## Kde v aplikaci

Příručka žije v jednom projektu ChatGPT: postranní panel › **Projects** › **New project**. Business dovoluje 40 souborů na projekt, příručka jich má 22.

## Postup

1) Založte projekt **New project** a pojmenujte ho „Příručka ChatGPT“.
2) Do projektu přidejte soubory `00-NAVIGATOR.md` až `20-POJMY.md` a `ZMENY.md`. Soubory `README.md` a `AGENTS.md` nenahrávejte, první je pro správce složky, druhý jen pro místní projekt (krok 6).
3) Otevřete nastavení projektu (Instructions) a vložte blok z oddílu „Instrukce projektu“.
4) V projektu otevřete nový chat a napište, co potřebujete, například „Chci, aby si ChatGPT nepamatoval jednu věc o mně“.
5) Když vyjde nová verze složky, staré soubory v projektu nahraďte novými. Co se změnilo, je v `ZMENY.md`.
6) Místní projekt místo cloudového (desktopová aplikace, jen Work): přidejte celou složku příručky přes **Add folder** (česky Přidat složku). Ve složce musí ležet soubor `AGENTS.md` s blokem instrukcí níž, upraveným pro složku (navíc: začít navigátorem, nehledat na webu, nic ve složce neměnit); v balíčku je připravený. Pole pokynů ani nahrání souborů pak nepotřebujete. Cloudový projekt ale funguje i v Chatu a v mobilu, místní jen ve Work na tomto počítači (`09-PROJEKTY.md`, kroky 8 a 9). Ověřeno v Codexu 3. 11. 2026, v aplikaci ChatGPT SIGNAL.

## Instrukce projektu

Zkopírujte celý blok do pole Instructions v projektu.

```
Jsi průvodce příručkou ChatGPT, Work a Codex pro lidi ve firmě nebo ve škole. Odpovídej česky a vykej.
Odpovídej jen podle souborů v tomto projektu. U každé rady uveď soubor a krok, ze kterého vychází, například „11-SKILLS.md, krok 3“.
Když odpověď v souborech není, řekni to rovnou a nic nedomýšlej, hlavně ne názvy tlačítek a nastavení. Doporuč ověřit v nápovědě OpenAI (help.openai.com) nebo u správce workspace.
Každý soubor má datum „stav k“. Když je údaj starší než 30 dní nebo je označený SIGNAL či ROZPOR, upozorni, že může být zastaralý, a doporuč ho ověřit v nápovědě OpenAI.
Popisky tlačítek jsou v souborech anglicky podle nápovědy. V české aplikaci se mohou jmenovat jinak. Když je uživatel nenajde, nabídni náhradní cestu z oddílu „Když to chybí“.
Nejdřív zjisti, jaký má uživatel tarif a co už používá. Začátečníkovi nedávej pokročilý postup.
Veď po jednom kroku: napiš jeden krok, počkej, co uživatel vidí, a teprve pak dej další.
Nic nenastavuj, nezapínej, neodesílej ani nesdílej za uživatele. Popiš, co má udělat on.
U otázek na osobní údaje, data žáků, klientů nebo na právo odkaž na 03-BEZPECNE-S-DATY.md a na pravidla organizace. Právní závěr nedávej.
Prompty ze souborů dávej do bloku ke zkopírování. Hranaté závorky nech vyplnit uživatele.
```

## Potřebuji → soubor

| Potřebuji | Soubor |
|---|---|
| zjistit, co mám v účtu a co mi zapnul správce | `01-NEZ-ZACNETE.md` |
| vybrat mezi Chat, Work a Codex | `02-CHAT-WORK-CODEX.md` |
| vědět, kde s daty pracovat, dočasný a zamčený chat | `03-BEZPECNE-S-DATY.md` |
| napsat zadání a zkontrolovat výsledek | `04-ZADANI-A-KONTROLA.md` |
| nahrát soubor, Space (dřív Library), limity souborů | `05-SOUBORY.md` |
| řídit paměť, smazat vzpomínku, paměť jen pro projekt | `06-PAMET.md` |
| nastavit, jak se mnou ChatGPT mluví | `07-VLASTNI-POKYNY.md` |
| aktuální fakta se zdrojem, hloubkový výzkum | `08-HLEDANI-A-VYZKUM.md` |
| mít téma na jednom místě, sdílet projekt s kolegy | `09-PROJEKTY.md` |
| vytvořit dokument, tabulku, prezentaci nebo obrázek | `10-DOKUMENTY-TABULKY-PREZENTACE.md` |
| uložit fungující postup jako skill a nasdílet ho | `11-SKILLS.md` |
| zachránit svoje vlastní GPT před koncem | `12-VLASTNI-GPT-PREVOD.md` |
| připojit Google Drive nebo SharePoint a OneDrive | `13-KONEKTORY-GOOGLE-MICROSOFT.md` |
| nechat úkol běžet pravidelně | `14-NAPLANOVANE-ULOHY.md` |
| sdíleného agenta pro tým | `15-WORKSPACE-AGENTS.md` |
| stránku nebo přehled pro kolegy (Pages ve Space, dřív Library, a Sites) | `16-SITES-A-PAGES.md` |
| pracovat nad složkou souborů v počítači | `17-CODEX.md` |
| něco nejde, tlačítko chybí, nemám oprávnění | `18-KDYZ-TO-NEFUNGUJE.md` |
| najít něco v Nastavení, první nastavení, dvoufázové ověření, připojit mobil | `19-NASTAVENI.md` |
| rozdíl projekt, skill, plugin, GPT, MCP, hooky | `20-POJMY.md` |
| co se v příručce změnilo | `ZMENY.md` |

## Příklad

Otázky, na které má projekt odpovědět ze souborů:

```
Jak zjistím, co si o mně ChatGPT pamatuje, a jak jednu věc smažu?
```

```
Mám vlastní GPT na přípravu zápisů z porad. Co s ním mám udělat do prosince?
```

Správná odpověď začíná souborem a krokem, například „06-PAMET.md, krok 2“ nebo „12-VLASTNI-GPT-PREVOD.md, krok 3“, a dá vám jen jeden krok. Když odpověď soubor ani krok neuvádí, instrukce projektu nejsou vložené. Zkontrolujte Instructions (krok 3 nahoře).

## Když to chybí

- Nemáte **Projects**: nahrajte soubory přímo do chatu (nejvýš ty, které potřebujete) a blok instrukcí vložte jako první zprávu.
- Projekt se nedá vytvořit ve firemním workspace: zeptejte se správce, jestli jsou projekty zapnuté (`01-NEZ-ZACNETE.md`).

## Zdroj a stav

- Limit 40 souborů na projekt v Business: https://help.openai.com/en/articles/8555545, stav k 2. 11. 2026, FAKT.
- Příručku má udržovat pravidelná sobotní kontrola nápovědy OpenAI. Co a kdy se změnilo, je v `ZMENY.md`. Když je poslední řádek starší než měsíc, berte údaje jako možná zastaralé.
