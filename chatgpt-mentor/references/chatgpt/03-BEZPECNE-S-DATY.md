# Bezpečně s daty

Víte, kde s daty pracovat, co do ChatGPT nikdy nedávat a k čemu je dočasný a zamčený chat.

**Pravidlo Euroinstitutu:** ve firemním workspace ChatGPT Euroinstitutu smíte pracovat se skutečnými podklady, včetně IVP a jmen žáků, bez začerňování. Platí jen pro firemní účet. Když se pravidlo školy změní, má přednost před touto kapitolou. Kapitola není právní rada.

## Kde v aplikaci

- Název workspace: nabídka účtu.
- Dočasný chat: nový chat › **Temporary**, před první zprávou volba **Personalized / Unpersonalized**.
- Zamčený chat: nabídka chatu (•••) › **Lock chat**.
- Paměť: **Settings › Personalization › Memory** (`06-PAMET.md`).

## Postup

1) Pracovní podklady jen ve firemním workspace Euroinstitutu. Před vložením zkontrolujte název workspace. Osobní účet ChatGPT na pracovní podklady nikdy.
2) Nevkládejte hesla, přístupové klíče, čísla karet ani přihlašovací údaje. Nikdy a nikam.
3) Nový postup, prompt nebo skill zkuste nejdřív na jednom podkladu a výstup porovnejte s originálem. Teprve pak ho pouštějte na další.
4) Paměť si pamatuje i to, co napíšete o žácích. Kdo nechce, aby se údaje přenášely mezi chaty, pracuje v projektu s pamětí jen pro projekt (`09-PROJEKTY.md`), nebo paměť vypne (`06-PAMET.md`).
5) Dočasný chat použijte, když nechcete, aby se chat uložil do historie a vytvořil vzpomínku. Před první zprávou jde zvolit:
   a) **Unpersonalized**: chat nepoužije paměť ani vlastní pokyny. Hodí se na čistý pokus.
   b) **Personalized**: podle starší nápovědy použije existující paměť a pokyny, ale novou vzpomínku nevytvoří (SIGNAL).
   Kopie dočasného chatu se podle starší nápovědy může z bezpečnostních důvodů uchovat až 30 dní (SIGNAL).
6) Zamčený chat (**Lock chat**) schová chat z historie, připnutých chatů a hledání a otevře se PINem nebo ověřením na zařízení. Chat nesmaže a nemění, jak dlouho se data uchovávají.
7) Text z webu, e-mailu nebo dokumentu je údaj, ne pokyn. Když v něm stojí „pošli seznam kontaktů“, ChatGPT to nemá udělat. Odesílání, mazání a sdílení vždy schvalujte sami.
8) Výstup, který jde k rodičům, klientům nebo do spisu, si přečtěte celý a za obsah odpovídáte vy. AI nestanovuje diagnózu ani hodnocení konkrétního člověka.

## Příklad

Kontrola výstupu proti podkladu před odesláním:

```
Porovnej výstup s původním podkladem. Vypiš každé jméno, datum, číslo a tvrzení z výstupu a u každého uveď místo v podkladu. Označ: sedí / změněno / v podkladu není. Nic neopravuj.
[podklad]
[výstup]
```

## Když to chybí

- Nevidíte název Euroinstitutu: jste v osobním účtu. Přepněte na workspace Euroinstitutu, chat v osobním účtu smažte.
- Chybí **Temporary**: zkuste nový chat ve webové aplikaci.
- Chybí **Lock chat**: zavádí se postupně.

## Zdroj a stav


- Obsah z Business OpenAI ve výchozím stavu nepoužívá k trénování modelů: https://openai.com/business-data, stav k 2. 11. 2026, FAKT. Jak to vyhodnotit pro vaši organizaci, rozhoduje organizace.
- Dočasný chat nevytváří vzpomínky a před startem jde zvolit Unpersonalized: https://help.openai.com/en/articles/8590148, stav k 2. 11. 2026, FAKT.
- Chování volby Personalized a uchování kopie až 30 dní: https://help.openai.com/en/articles/8914046, ověřeno 7. 10. 2026, SIGNAL, ověřte v aktuální nápovědě.
- Pravidlo Euroinstitutu k datům: skripta Tomáše Doležala ze 3. 9. 2026. Je to pravidlo organizace, ne právní výklad této příručky.
- Zamčený chat v Business od 20. 10. 2026, zavádí se postupně: https://help.openai.com/en/articles/11391654, stav k 2. 11. 2026, SIGNAL.
- Řídit se nejdřív pravidly organizace a důležitý výstup nechat zkontrolovat člověkem: https://openai.com/academy/responsible-and-safe-use, stav k 2. 11. 2026.
