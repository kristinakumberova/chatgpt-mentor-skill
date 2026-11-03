# Google dokument, nebo nahraný soubor

Kapitola vám pomůže poznat, jestli máte nativní Google soubor (Dokumenty, Tabulky, Prezentace), nebo nahraný soubor (PDF, Word, Excel). AI s nimi zachází různě: ChatGPT podle nápovědy upravuje jen nativní Google soubory, nahrané jen čte.

## Kde

- Disk Google, sloupec s ikonou a názvem souboru.
- Otevřený soubor: nabídka **Soubor**.
- Nastavení převodu: ozubené kolo vpravo nahoře › **Nastavení** (popisek volby ověřte na svém účtu).

## Postup

1) Poznejte typ souboru.
   a) **Nativní Google soubor:** název bez přípony, modrá ikona Dokumentů, zelená Tabulek, žlutá Prezentací.
   b) **Nahraný soubor:** název s příponou `.pdf`, `.docx`, `.xlsx`, `.pptx`. Při otevření nahraného Wordu se u názvu ukáže štítek `.DOCX`.

2) Rozhodněte, jestli převádět.
   a) **Převeďte**, když chcete, aby AI soubor upravovala, nebo když na něm pracuje víc lidí najednou.
   b) **Nepřevádějte** podepsané smlouvy, oficiální PDF, vysvědčení, faktury a výkresy. Zůstanou jako nahrané, AI je jen čte.

3) Převeďte Word, Excel nebo PowerPoint: otevřete soubor na Disku › **Soubor** › **Uložit jako Dokumenty Google** (u tabulky **Tabulky Google**, u prezentace **Prezentace Google**). Vznikne nová kopie, originál zůstane. Popisky ověřte na svém účtu.

4) Převeďte PDF jen tehdy, když potřebujete text upravovat: pravé tlačítko na PDF › **Otevřít v aplikaci** › **Dokumenty Google**. Rozložení stránky, tabulky a obrázky se často rozpadnou. Obsah zkontrolujte proti originálu.

5) Po převodu přejmenujte kopii tak, aby nebyly dva soubory se stejným názvem, a originál přesuňte do **01_Podklady** (02-SLOZKY-A-NAZVY.md, krok 2).

6) Soubory `.md` (markdown, prostý text s nadpisy, v jakém je i tahle příručka) Disk a Dokumenty od 5. 10. 2026 zobrazí a upraví přímo. Převádět je nemusíte.

## Příklad

Škola: učitel dostal plán akcí jako `plan-akci.docx`. Převede ho na Google dokument, aby do něj AI mohla doplnit termíny, a původní Word nechá v Podkladech.
Kancelář: ceník dodavatele v PDF se nepřevádí. AI z něj jen čte ceny do nové tabulky.

Prompt pro kontrolu převodu:

```
Pomocí Google Drive porovnej tyto dva soubory:
originál [odkaz na .docx nebo .pdf] a převedenou kopii [odkaz na Google dokument].
Vypiš, co v kopii chybí nebo se liší: tabulky, čísla, odrážky, poznámky pod čarou, obrázky.
Nic neměň. Když některý soubor nepřečteš, řekni který.
```

Rozdíly, které AI najde, ověřte v obou souborech sami. Když AI řekne „žádné rozdíly“, zkontrolujte aspoň tabulky a čísla.

## Když to chybí

| Co vidíte | Co udělat |
|---|---|
| V nabídce Soubor není „Uložit jako Dokumenty Google“ | Soubor nemáte právo upravovat. Vytvořte si kopii, nebo požádejte vlastníka. |
| Po převodu PDF je text rozházený | Pracujte s originálem PDF a výstup nechte AI zapsat do nového dokumentu. |
| AI soubor přečte, ale neupraví | Je to nahraný soubor. Převeďte ho (krok 3) nebo nechte AI vytvořit nový soubor. |
| Na Disku jsou dva soubory stejného jména | Jeden je originál, druhý kopie. Přejmenujte kopii (krok 5). |

## Zdroj a stav

- Zápis ChatGPT jen do nativních souborů: https://learn.chatgpt.com/docs/plugins (SIGNAL, z dokumentace pluginů; ověřte na cvičném souboru)
- Markdown v Disku a Dokumentech od 5. 10. 2026: https://workspaceupdates.googleblog.com/ (FAKT, štítek Google Drive)
- Vytvoření a kopírování souborů: https://support.google.com/docs/answer/49114
- Stav k 2. 11. 2026. Popisky převodu nebyly ověřeny na účtu.
