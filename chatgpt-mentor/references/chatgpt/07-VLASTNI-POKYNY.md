# Vlastní pokyny

Jednou nastavíte, jak s vámi má ChatGPT mluvit a jak má odpovídat, a nemusíte to psát do každého chatu.

## Kde v aplikaci

- **Settings › Personalization**: vlastní pokyny (custom instructions) a volba osobnosti.
- Pokyny pro jedno téma: nastavení projektu › **Instructions** (`09-PROJEKTY.md`).
- Místní Work a Codex: osobní pokyny se ukládají do globálního souboru `AGENTS.md` (ve Windows obvykle `C:\Users\<jméno>\.codex\AGENTS.md`). Pokyny z **Personalization** se tam nepřenesou samy.

## Postup

1) Sepište tři až šest stabilních přání, která platí skoro pro každý chat: jazyk, tón, délka, formát, co dělat při nejistotě.
2) Vložte je do **Settings › Personalization** a uložte.
3) Pravidlo jen pro jedno téma (třída, klient, typ dokumentu) dejte do instrukcí projektu, ne do vlastních pokynů.
4) Jednorázovou výjimku napište do zadání. Pokyny kvůli jednomu úkolu neměňte.
5) Ověřte účinek: stejné krátké zadání dejte v běžném chatu a v dočasném chatu **Unpersonalized**, který pokyny nepoužije. Porovnejte tón, délku a jestli pokyny dodržel.
6) Pokyny jsou součást paměti (`06-PAMET.md`). Když chcete zkusit chat úplně bez nich, použijte **Temporary › Unpersonalized**.
7) Osobnost mění styl, jakým ChatGPT mluví. Nepřidá mu znalosti ani schopnosti.

## Příklad

Pokyny pro učitele:

```
Piš česky a vykej. Odpovídej stručně, nejdřív výsledek, pak vysvětlení.
Když chybí cíl hodiny, věk žáků nebo časová dotace, zeptej se dřív, než začneš.
Neodvozuj diagnózy ani hodnocení konkrétního dítěte. Návrh označ jako podklad k mému posouzení.
Nelichot mi. Když v zadání vidíš rozpor nebo chybu, řekni to.
```

Pokyny pro kancelář:

```
Piš česky, věcně, bez úvodních frází. E-maily do pěti vět, když neřeknu jinak.
Čísla a termíny přebírej jen z podkladů. Chybějící údaj označ „doplnit“ a nevymýšlej ho.
Když si nejsi jistý, napiš to a navrhni, jak to ověřit.
Nelichot mi. Rozpor nebo chybu v zadání řekni na začátku odpovědi.
```

Kontrola účinku:

```
Napiš krátkou odpověď kolegovi, že porada se přesouvá z úterý na čtvrtek. Čas neuvádím.
```

Správně: odpověď je česky, krátká a místo času je „doplnit“ nebo otázka.

## Když to chybí

- Chybí **Personalization** nebo nejde uložit: ve firemním workspace může nastavení omezit správce. Pokyny vložte jako první zprávu chatu, nebo je dejte do instrukcí projektu.
- Pokyny se nedrží: zkraťte je. Dlouhý seznam pravidel se dodržuje hůř než pět vět.
- Pokyny si odporují s instrukcemi projektu: rozhodněte, které platí, a druhé upravte.
- Místní Work pokyny nedrží: globální `AGENTS.md` je prázdný. Zkouška: v novém místním chatu napište „Jaké vlastní pokyny ode mě máš? Vypiš je doslova a napiš, odkud je máš.“ Když žádné nemá, vložte pokyny do globálního `AGENTS.md` nebo do osobních pokynů v nastavení Codexu.

## Zdroj a stav

- Vlastní pokyny a osobnost: https://learn.chatgpt.com/docs/personalize, ověřeno 7. 10. 2026, stav k 2. 11. 2026, FAKT.
- V Codexu jsou osobní pokyny v globálním `AGENTS.md`: https://learn.chatgpt.com/docs/personalize, stav k 3. 11. 2026, FAKT. Pro místní Work SIGNAL (stejné jádro jako Codex, nezkoušeno). Cesta `.codex\AGENTS.md` ve Windows: zjištěno na počítači 3. 11. 2026, SIGNAL. Jestli Personalization platí v cloudovém Work: NEDOHLEDATELNÉ.
- Dočasný chat Unpersonalized bez paměti a pokynů: https://help.openai.com/en/articles/8590148, stav k 2. 11. 2026, FAKT.
- Pokyn „nelichot mi, řekni rozpor“: praktici (Berman a rozhovor s Altmanem, https://www.youtube.com/watch?v=3gXLmy7DK_4), SIGNAL.
