# Vlastní GPT končí 11. 12. 2026

Zazálohujete svoje vlastní GPT a převedete je na plugin se skillem, dřív než přestanou fungovat.

## Kde v aplikaci

- Vaše GPT: postranní panel › **GPTs** › vaše GPT › úprava (**Edit**).
- Převod: nabídka převodu GPT na plugin. Přesné místo tlačítka ověřte na účtu.
- Výsledek: **Plugins** a **Plugins › Skills** (`11-SKILLS.md`).

## Postup

1) Zjistěte termín. Vlastní GPT standardně skončí 11. 12. 2026 ve všech tarifech. Datum pro váš účet si ověřte v upozornění ve workspace. Nové GPT už nejspíš nejdou založit, ověřte v nabídce. Tato příručka neučí stavět nové GPT. Nové postupy dělejte jako skill.
2) Sepište si všechna svoje GPT, která používáte vy nebo kolegové. U každého napište, k čemu je a kdo ho používá.
3) Každé GPT zazálohujte, než ho převedete:
   a) zkopírujte celý text pokynů (Instructions) do dokumentu,
   b) stáhněte nebo najděte originály souborů ze znalostí (Knowledge),
   c) zapište, jaké akce a připojené aplikace GPT používá a jaký model,
   d) zapište tři typické zadání, se kterými GPT používáte. Poslouží na test.
4) Převeďte GPT na plugin nabídkou převodu. Při převodu:
   a) z pokynů vznikne skill,
   b) akce se nepřenesou a připojené aplikace nastavíte znovu,
   c) model se nepřenese,
   d) plugin začíná jako soukromý, vidíte ho jen vy,
   e) původní GPT je po převodu jen ke čtení.
5) Vyzkoušejte nový skill na třech zadáních z kroku 3d a výsledky porovnejte s tím, co dávalo GPT.
6) Když GPT používali kolegové, nasdílejte jim plugin nebo skill (`11-SKILLS.md`, krok 7) a pošlete jim, jak ho najdou.
7) Náhradní cesta bez nabídky převodu: otevřete nový chat, vložte zálohu pokynů a soubory a požádejte o skill (prompt v oddílu Příklad). ChatGPT použije **skill-creator**.

## Příklad

Převod zálohy na skill:

```
Z přiložených pokynů a souborů mého vlastního GPT „[název]“ vytvoř skill.
Zachovej, co GPT dělalo: [jednou větou]. Pokyny převeď beze změny smyslu. Když v nich je odkaz na akci nebo připojenou aplikaci, vypiš ji zvlášť. Tu nastavím sám.
Nejdřív mi ukaž návrh pokynů skillu a popis, kdy ho použít.
```

Porovnání (škola):

```
Totéž zadání dávám starému GPT i novému skillu: „[připrav diktát pro 3. třídu na vyjmenovaná slova po B]“. Porovnej oba výsledky: co nový skill vynechal, co přidal a jestli drží stejný formát.
```

Seznam GPT pro tým (kancelář):

```
Připrav tabulku pro převod vlastních GPT v našem týmu: název GPT, k čemu je, kdo ho používá, záloha pokynů (ano/ne), soubory (ano/ne), akce a aplikace, převedeno (ano/ne), otestováno (ano/ne). Řádky nech prázdné, vyplním je sám.
```

## Když to chybí

- Nevidíte nabídku převodu: ve firemním workspace ji může řídit správce. Použijte náhradní cestu z kroku 7 a zeptejte se správce.
- GPT patří kolegovi, který odešel: převést ho nejspíš může jen vlastník GPT nebo správce workspace (SIGNAL). Zálohu pokynů udělejte z toho, co vidíte, a předejte ji správci.
- Akce GPT (napojení na jinou službu) po převodu nefunguje: akce se nepřenáší. Připojte aplikaci znovu v pluginu, nebo se obraťte na správce.
- Je po 11. 12. 2026: GPT už standardně nefungují. Ze zálohy vytvořte skill podle kroku 7.

## Zdroj a stav

- Konec vlastních GPT 11. 12. 2026 ve všech tarifech, převod na plugin, co se přenáší a co ne, soukromý plugin, GPT po převodu jen ke čtení: https://help.openai.com/en/articles/20001519-custom-gpt-retirement-and-migration-faq, stav k 2. 11. 2026, FAKT.
- Konec zakládání nových GPT: FAQ uvádí 25. 9. 2026, jiný zdroj 26. 10. 2026 pro Enterprise. ROZPOR, ověřte v nabídce svého účtu.
- Přesné místo a název tlačítka převodu a cesta GPTs › Edit: SIGNAL, ověřte na účtu.
- Zálohovat pokyny a soubory a převést je přes skill-creator: praktik AI Univerzita, https://www.youtube.com/watch?v=lsWgmVX3TVY, SIGNAL.
