# Soubory a jejich limity

Nahrajete správný podklad a ověříte, že ho ChatGPT opravdu otevřel a přečetl.

## Kde v aplikaci

- Příloha k chatu: tlačítko **+** u pole pro zadání › nahrát soubor.
- Uložené soubory: postranní panel › **Space** (dřív **Library**). V něm nahrání souboru (dřív **Upload**), přidání uloženého souboru do chatu (dřív **Add from library**) a přehled místa (dřív **Storage**). Přesné nové popisky ověřte na účtu.
- Soubory projektu: projekt › **Sources** nebo soubory projektu (`09-PROJEKTY.md`).

## Postup

1) Nahrajte jen soubory, které úkol potřebuje. Pět souvisejících stránek je lepší než celá složka.
2) Před prací ověřte, že soubor přečetl. Řekněte si o název, dva konkrétní údaje z obsahu a místo, kde stojí (prompt v oddílu Příklad). Údaje si sami najděte v souboru.
3) U víc verzí jednoho dokumentu napište, která platí. Chybějící část v odpovědi neznamená, že údaj v dokumentu není.
4) U PDF řekněte, které strany vás zajímají. Skeny, tabulky a obrázky se mohou načíst hůř než běžný text. Nečitelná místa ať ChatGPT označí.
5) Když potřebujete graf nebo obrázek z PDF, přiložte PDF přímo do chatu. Obrázky z PDF uloženého v projektu se nemusí načíst.
6) Soubor, který budete používat opakovaně, uložte do **Space**. V dalším chatu ho připojíte ze Space a nemusíte ho nahrávat znovu.
7) Smazáním chatu se soubor ze Space nesmaže. Mažte ho ve Space zvlášť.

## Příklad

Ověření, že soubor přečetl:

```
Než začneš, ověř podklady. U každého souboru uveď název, co jsi přečetl (celý, část, jen název) a dva konkrétní údaje i s místem, kde je najdu (strana, nadpis). Když něco nejde přečíst, napiš to a zastav se.
```

Škola:

```
V přiloženém smyšleném textu o výletu najdi místo srazu a čas návratu. U každého údaje napiš větu, ve které stojí.
```

Kancelář:

```
V přiloženém ceníku na straně [3] vypiš tabulku: položka, cena, jednotka, poznámka pod čarou. Hodnoty neopravuj, jen přepiš. Nečitelná místa označ „nečitelné“.
```

## Když to chybí

- Soubor se nenahraje: zkontrolujte velikost a typ. Rozdělte velký soubor, nebo vložte potřebný text přímo do zprávy.
- ChatGPT odpovídá, jako by soubor neviděl: nahrajte ho znovu přímo do chatu a zopakujte krok 2.
- Chybí **Space**: na mobilu se dostupnost mění, zkuste webovou aplikaci.
- Soubor ze sdíleného disku Google ve Space: může nefungovat. Zdroje si odporují (ROZPOR), ověřte na cvičném souboru. Když nejde, soubor stáhněte a nahrajte, nebo použijte konektor (`13-KONEKTORY-GOOGLE-MICROSOFT.md`).

## Zdroj a stav

- Obrázky z PDF uloženého v projektu se nemusí načíst: https://help.openai.com/en/articles/8555545, stav k 2. 11. 2026, FAKT.
- Space (dřív Library), mazání chatu nemaže uložený soubor: https://help.openai.com/en/articles/20001052, ověřeno 7. 10. 2026, stav k 2. 11. 2026, FAKT. Nové popisky tlačítek po přejmenování: SIGNAL.
- Sdílené disky Google ve Space: nápověda ze 7. 10. je v první verzi nepodporovala, novější stav neznáme. ROZPOR.
- Limity souborů podle nápovědy z 7. 10. 2026: do 512 MB na soubor, textové dokumenty do 2 milionů tokenů, tabulky zhruba 50 MB, obrázky 20 MB. Limit neznamená, že model posoudí celý obsah najednou. SIGNAL, limity se mění, ověřte v nápovědě.
