# Skill ChatGPT mentor: nahrání a vyzkoušení

Skill vás provede tím, jak svou opakovanou práci převést do ChatGPT: projekt, skill, plugin, nebo naplánovaná úloha. Odpovídá podle přiložené příručky a chybějící ověří na webu OpenAI. Stav k 3. 11. 2026.

## Nahrání

1) V ChatGPT na webu otevřete postranní panel › **Plugins** › záložka **Skills**.

2) Klikněte na **Create** › **Upload from your computer**.

3) Vyberte soubor `chatgpt-mentor.zip` z této složky.
   a) ZIP nejde vybrat: zkuste vybrat celou složku `chatgpt-mentor`.
   b) Nabídka **Upload** chybí: nahrávání skillů vypnul správce workspace. Zeptejte se ho, nebo použijte náhradní cestu níž.

4) Počkejte na kontrolu. Skill se objeví v **Created by me**. Když je označený **Needs Review**, přečtěte si, co ChatGPT hlásí, a potvrďte.

## Vyzkoušení

1) Otevřete nový chat a napište:

```text
@chatgpt-mentor Každý týden píšu žákům zpětnou vazbu podle kritérií a pořád vkládám stejný prompt. Jak to mám v ChatGPT nastavit?
```

2) Správná odpověď doporučí jeden nástroj (tady skill), uvede soubor a krok z příručky, například „11-SKILLS.md, krok 3“, a položí jednu otázku.

3) Zkuste i otázku, kterou příručka nemá. Skill má říct, že ji ověří na webu, a uvést odkaz.

## Sdílení s kolegy

1) **Plugins › Skills** › u skillu **•••** › **Share**.

2) Nejdřív jedné kolegyni, ať ho vyzkouší. Pak skupině nebo celému workspace.

## Když to nejde

| Co vidíte | Co udělat |
|---|---|
| Chybí **Skills** | skilly nemá zapnuté správce; použijte náhradní cestu |
| Skill odpovídá bez souboru a kroku | nepoužil se; zavolejte ho výslovně přes `@chatgpt-mentor` |
| Skill je **Blocked** | obraťte se na správce, skill nepoužívejte |

**Náhradní cesta:** založte projekt „ChatGPT mentor“, do **Sources** nahrajte soubory ze složky `chatgpt-mentor/references/chatgpt/` a text souboru `SKILL.md` (bez první části mezi čárami `---`) vložte do pokynů projektu.

## Aktualizace

Příručka ve skillu je stav k 3. 11. 2026 a sama se neaktualizuje. Novou verzi nahrajete stejným postupem a starou smažete.
