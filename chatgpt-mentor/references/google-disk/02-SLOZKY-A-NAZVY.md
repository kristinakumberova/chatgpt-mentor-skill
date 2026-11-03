# Složky a názvy, které najde člověk i AI

Kapitola dává jednoduchý vzor složek a názvů. AI hledá soubory podle názvu a složky, takže s „dokument (3) finální2.docx“ sáhne vedle stejně snadno jako kolega.

## Kde

- Disk Google › **Nový** › **Nová složka**.
- Přejmenování: pravé tlačítko na souboru › **Přejmenovat**.
- Google oficiální vzor složek nedává. Vzor níž je doporučení, tým si ho může upravit (PŘEDPOKLAD).

## Postup

1) Dohodněte s týmem jeden vzor a zapište ho do dokumentu „Jak pojmenováváme“ v kořeni sdíleného disku. Bez dohody vzor nevydrží ani měsíc.

2) Založte stejnou sadu složek v každé oblasti (zakázka, předmět, projekt):
   a) **01_Podklady** - vstupy, které se nemění (zadání, učebnice, smlouva v PDF).
   b) **02_Rozpracovane** - koncepty, sem smí AI zapisovat.
   c) **03_Schvalene** - jen schválené verze, AI sem nezapisuje.
   d) **Sablony** - prázdné vzory (04-VERZE-HISTORIE-A-SABLONY.md, krok 6).
   e) **Archiv** - staré věci, které nechcete mazat.

3) Pojmenujte soubor podle vzoru `RRRR-MM-DD_tema_typ_v01`, například `2026-11-02_porada-obchod_zapis_v01`.
   a) Datum na začátku: soubory se seřadí samy.
   b) Bez diakritiky a mezer: názvy se nerozbijí při stažení a v odkazu.
   c) Verze `v01`, `v02` jen u nahraných souborů (PDF, Word). Nativní Google dokument má historii verzí, číslo v názvu nepotřebuje.

4) Slovo „finální“ do názvu nepište. Schválení nedokazuje. Schválený soubor přesuňte do **03_Schvalene** a do historie verzí zapište, kdo a kdy schválil.

5) Když zadáváte práci AI, dejte jí odkaz na konkrétní soubor nebo složku, ne jen téma. Odkaz zkopírujete: pravé tlačítko › **Sdílet** › **Kopírovat odkaz**. Sdílení se tím nemění.

## Příklad

Škola: `Dejepis_7A/01_Podklady/2026-09-01_ucebnice-kap3_vypis.pdf`, výstup `02_Rozpracovane/2026-11-02_pracovni-list-kap3_v01`.
Kancelář: `Zakazka-Novostavba/01_Podklady/2026-10-15_poptavka_klient.pdf`, výstup `02_Rozpracovane/2026-11-02_nabidka_navrh`.

Nechte AI navrhnout úklid, ale přejmenujte sami:

```
Pomocí Google Drive otevři složku [odkaz na složku] a vypiš všechny soubory.
Navrhni nové názvy podle vzoru RRRR-MM-DD_tema_typ_v01 (bez diakritiky a mezer).
Datum ber z data vytvoření souboru, když není v názvu.
Vrať tabulku: současný název | navržený název | do které složky patří (01_Podklady, 02_Rozpracovane, 03_Schvalene, Archiv).
Nic nepřejmenovávej ani nepřesouvej. U souborů, kde si nejsi jistý, napiš "nevím".
```

Tabulku projděte a změny udělejte ručně. Hromadné přejmenování AI na sdíleném disku je zápis do cizích souborů.

## Když to chybí

| Co vidíte | Co udělat |
|---|---|
| Nejde vytvořit složku na sdíleném disku | Máte roli Komentující nebo Čtenář, požádejte o vyšší roli. |
| Nejde přejmenovat soubor | Nemáte právo upravovat, požádejte vlastníka. |
| AI najde starou verzi místo nové | Staré verze přesuňte do Archivu a v promptu dejte odkaz, ne název. |
| Kolegové vzor nedodržují | Dejte odkaz na „Jak pojmenováváme“ do popisu sdíleného disku a vraťte se k němu na poradě. |

## Zdroj a stav

- Google vzor struktury složek nedává (PREDPOKLAD na základě Learning Center): https://support.google.com/a/users/answer/9282958
- Vytvoření a kopírování souborů: https://support.google.com/docs/answer/49114
- Stav k 2. 11. 2026. Vzor složek a názvů je doporučení této příručky, ne pravidlo Google.
