# Nastavení: co kde je a co nastavit

Víte, co najdete v jednotlivých částech nastavení, co ve škole a ve firmě nastavit hned a co může zamknout správce workspace.

## Kde v aplikaci

- Web: ikona profilu › **Settings**. Desktop: **Settings** (česky **Nastavení**). Mobil: profil › nastavení, části se mohou jmenovat a řadit jinak.
- Správce workspace: **Workspace settings** (Admin Console), hlavně **Permissions & roles**, **Apps** a **Plugins**.

| Část (česky) | Co tam je | Doporučujeme | Co může zamknout správce | Kapitola |
|---|---|---|---|---|
| **General** | jazyk, vzhled | jazyk podle sebe; jazyk odpovědí řeší vlastní pokyny | obvykle nic | `07-VLASTNI-POKYNY.md` |
| **Notifications** | upozornění, třeba na hotovou úlohu | zapnout u naplánovaných úloh | obvykle nic | `14-NAPLANOVANE-ULOHY.md` |
| **Personalization** (**Personalizace**) | vlastní pokyny, osobnost, **Memory** s **Reference saved memories** a **Reference chat history** | krátké pokyny, paměť jednou za čas projít | paměť podle role | `06-PAMET.md`, `07-VLASTNI-POKYNY.md` |
| **Apps** / **Plugins** | připojené aplikace (od 17. 12. 2025 se konektorům říká apps) | připojit jen to, co používáte | které aplikace smíte připojit; ve Business jsou ve výchozím stavu zapnuté | `13-KONEKTORY-GOOGLE-MICROSOFT.md` |
| **Schedules** | naplánované úlohy | ve Business nejvýš 10 aktivních | dostupnost funkce | `14-NAPLANOVANE-ULOHY.md` |
| **Data controls** | **Improve the model for everyone**, **Shared links › Manage**, archiv a mazání chatů, export | jednou za měsíc projít sdílené odkazy | export a smazání účtu ve Business sami neuděláte | `03-BEZPECNE-S-DATY.md` |
| **Security and login** (**Zabezpečení**) | **Multi-factor authentication (MFA)** (**Vícefázové ověřování**), passkey, **Log out of all devices** | zapnout vícefázové ověřování a mít dvě metody | ve workspace ho vynutit nejde; u SSO ho řeší správce v poskytovateli přihlášení | tato kapitola |
| **Account** | tarif, workspace, smazání účtu | zkontrolovat správný workspace | smazání účtu ve firemním workspace; Codex ve Business mají jen workspace, které přidaly Codex seat před 24. 6. 2026 | `01-NEZ-ZACNETE.md` |
| **Connections** (**Připojení**), jen desktop | **Control this Mac or PC** (**Ovládat tento počítač**), **Control other devices**, **Allow connections** (**Povolit připojení**), udržet počítač vzhůru (**Zabránit uspání tohoto počítače**), SSH | zapnout, až budete počítač ovládat z mobilu | vzdálené ovládání | `17-CODEX.md` |

Práva pro Work a Codex (co smí v počítači dělat bez ptaní) se volí pod polem pro zadání, ne v Settings. Ověřte na účtu.

## Postup

První nastavení za 10 minut:

1) Workspace a jazyk. Klikněte na ikonu profilu a zkontrolujte, že jste ve workspace školy nebo firmy, ne v osobním. Přepnutí nic nepřesouvá ani nekopíruje. V **General** nastavte jazyk.
2) Vícefázové ověřování. **Settings › Security and login** › **Multi-factor authentication (MFA)** › vyberte metodu a projděte nastavení. Platí pro všechny služby OpenAI. Metody: aplikace v telefonu (například Google Authenticator), potvrzení v telefonu, SMS nebo WhatsApp, passkey; nabídka se liší podle zařízení, země, tarifu a způsobu založení účtu. Nastavte si aspoň dvě metody. E-mail jako záložní metoda není a obnova přes podporu trvá několik dní a jde jen jednou.
3) Personalizace. Vložte tři až šest vět vlastních pokynů (`07-VLASTNI-POKYNY.md`, krok 1 a 2).
4) Paměť. V **Personalization › Memory** se podívejte, co si ChatGPT pamatuje, a smažte, co tam být nemá (`06-PAMET.md`, krok 2 a 3).
5) Data controls. V **Shared links › Manage** smažte odkazy, které už nepotřebujete. Ve Business se data workspace k tréninku modelů nepoužívají. V osobním účtu Free, Plus a Pro je **Improve the model for everyone** ve výchozím stavu zapnuté; vypnutí historii chatů nesmaže.
6) Co nechat být:
   a) **Connections**, dokud nepotřebujete mobil (příklad níže),
   b) smazání účtu, export a archiv,
   c) konektory, ty připojte podle `13-KONEKTORY-GOOGLE-MICROSOFT.md`.
7) Ztracený telefon nebo přihlášení na cizím počítači: **Security › Log out of all devices**. Odhlášení může trvat až 30 minut.

## Příklad

Připojení mobilu k počítači:

1) Na počítači: **Nastavení › Připojení › Ovládat tento počítač** › **Set up** nebo **Add**.
2) Zapněte **Povolit připojení** a potvrďte přístup.
3) V mobilu naskenujte QR kód, přihlaste se stejným účtem a workspace a připojení schvalte.
4) V mobilu otevřete **Codex** (starší verze **Remote**) a vyberte počítač. Počítač musí zůstat zapnutý a online, pomůže **Zabránit uspání tohoto počítače**.

Připojujte jen vlastní zařízení. Odhlášení z ChatGPT vzdálené ovládání vypne, spárování zůstanou.

## Na co lidé narážejí

- Ztracený telefon s ověřovací aplikací. Bez druhé metody pomůže jen podpora OpenAI: ověření trvá několik dní a jednorázové přihlášení e-mailem dá jen jednou (FAKT). Lidé hlásí, že se mezitím k účtu nedostanou, i u přihlášení přes Google (SIGNAL). Pomáhá druhá metoda nastavená dřív, než telefon ztratíte.
- Nechtěný passkey. Passkey vytvořený omylem na jiném zařízení si účet po odhlášení všude vyžádal (SIGNAL).
- Paměť nejde zapnout. Při přepnutí **Reference saved memories** zmizí **Reference chat history**. Vypnutí uložených vzpomínek vypne i historii chatů, naopak ne (FAKT).
- Starý kontext v nových chatech. Lidem pomohl dočasný chat, nebo vypnutí obou přepínačů paměti (SIGNAL).
- Po přechodu z Plus na Business chybí chaty. Přepnutí workspace nic nepřesouvá (FAKT). Přesun se spouští zvlášť: ve workspace Business **Settings › Data controls › Merge data from your personal workspace** › **Merge** (FAKT). Sloučení nejde vrátit a ne všechno se přenese; důležité chaty si předem uložte (FAKT). Že přesun trvá až 24 hodin a někdy chat chybí, hlásí lidé (SIGNAL).
- Párování mobilu na Windows nebo Macu selže, i se zapnutým ověřováním (oddíl Když to chybí).

## Když to chybí

- Volba chybí nebo nejde změnit: zamkl ji správce workspace, nebo ji váš tarif nemá (`18-KDYZ-TO-NEFUNGUJE.md`).
- Nevidíte vícefázové ověřování:
  a) jste v desktopové aplikaci: zkuste chatgpt.com v prohlížeči, **Settings › Security and login**,
  b) přihlašujete se přes firemní SSO (správce ho nastavil pro doménu školy nebo firmy): ověřování řeší správce u poskytovatele přihlášení, ne v ChatGPT,
  c) přihlašujete se tlačítkem Google, Apple nebo Microsoft: nabídka metod závisí i na způsobu založení účtu; když volba chybí, zapněte druhý krok aspoň v účtu Google, Apple nebo Microsoft.
- **Povolit připojení** hlásí „Nepodařilo se aktualizovat dostupnost vzdáleného ovládání“: známá chyba aplikace, oficiální oprava ani odpověď vývojářů zatím není (SIGNAL). Uživatelé zkoušeli bez trvalého výsledku: synchronizaci hodin, vypnutí VPN a proxy, jinou síť, aktualizaci, odhlášení a restart aplikace, zapnutí vícefázového ověřování. Zkuste to po jednom, a když nic nepomůže, počkejte na aktualizaci aplikace.
- Chybí **Connections**: zavádí se postupně a ve workspace ho může muset povolit správce.
- Ve Business chybí export dat nebo smazání účtu: řeší vlastník workspace.

## Zdroj a stav

Články help.openai.com otevřené 3. 11. 2026 ve vestavěném prohlížeči (8), learn.chatgpt.com (2), GitHub (2).

- Vzdálené ovládání: **Settings › Connections › Control this Mac or PC**, **Set up** / **Add**, QR kód, stejný účet a workspace, počítač vzhůru, Mac nebo Windows, dostupnost podle zavádění a workspace: https://learn.chatgpt.com/docs/remote, stav k 3. 11. 2026, FAKT.
- **Control other devices**, přepínač připojení, odhlášení vypne **Remote Control**, SSH v Connections, povolení správcem: https://learn.chatgpt.com/docs/remote-connections, stav k 3. 11. 2026, FAKT. Dokumentace píše **Allow other devices to connect**, česká aplikace **Povolit připojení**.
- Vícefázové ověřování: **Settings › Security and login › Multi-factor authentication (MFA)**, metody, platnost pro všechny služby OpenAI, obnova přes podporu jen jednou, e-mail není metoda, **Log out of all devices** do 30 minut, ve workspace nejde vynutit: https://help.openai.com/en/articles/7967234, stav k 3. 11. 2026, FAKT. Přesnou cestu v desktopové aplikaci ověřte na účtu.
- U SSO se vícefázové ověřování nastavuje v poskytovateli přihlášení: https://help.openai.com/en/articles/9534785, stav k 3. 11. 2026, FAKT.
- **Data controls**, **Improve the model for everyone** zapnuté u osobních Free, Plus a Pro, dočasný chat až 30 dní, export a smazání účtu jen mimo Business: https://help.openai.com/en/articles/7730893, stav k 3. 11. 2026, FAKT.
- Business: data se netrénují, **Settings › Data controls › Shared links › Manage › Delete shared link**, chaty vidí jen autor, Codex seat jen pro workspace, které ho přidaly před 24. 6. 2026: https://help.openai.com/en/articles/8798634, stav k 3. 11. 2026, FAKT.
- Přepnutí workspace přes ikonu profilu nic nepřesouvá: https://help.openai.com/en/articles/8265430, stav k 3. 11. 2026, FAKT.
- Sloučení osobního workspace: **Settings › Data Controls › Merge**, nevratné, ne všechno se přenese: https://help.openai.com/en/articles/8801890, stav k 3. 11. 2026, FAKT. Až 24 hodin: SIGNAL (diskuze).
- Business: aplikace ve výchozím stavu zapnuté, správce je mění v **Admin Console › Plugins**: https://help.openai.com/en/articles/11509118, stav k 3. 11. 2026, FAKT. Přejmenování konektorů na apps od 17. 12. 2025: SIGNAL.
- Paměť: **Settings › Personalization › Memory**, volby **Memory**, **Reference saved memories**, **Reference chat history**, **Memory summary**, **Manage**, **Saved memories** podle účtu: https://help.openai.com/en/articles/8590148, stav k 3. 11. 2026, FAKT. Vazba přepínačů (vypnutí uložených vzpomínek vypne i historii): SIGNAL.
- Práva Codexu pod polem pro zadání: https://developers.openai.com/codex/concepts/sandboxing, stav k 3. 11. 2026, SIGNAL. Volby Work v desktopu: neověřeno.
- Části **General**, **Notifications**, **Account**, **Schedules** a umístění jazyka a vzhledu: SIGNAL ze stránek třetích stran, ověřte na účtu.
- Chyba vzdáleného ovládání: https://github.com/openai/codex/issues/57217 (26. 10. 2026, Windows 11, zavřeno bez opravy) a https://github.com/openai/codex/issues/46466 (18. 9. až 12. 10. 2026, Windows, nic nepomohlo), stejná chyba na Macu #56104; stav k 3. 11. 2026, SIGNAL.
- Diskuze, vše 2026 a SIGNAL: ztráta ověřovací aplikace https://community.openai.com/t/locked-out-after-losing-mfa-access/1398331; paměť nejde zapnout https://community.openai.com/t/bug-cant-enable-memory-reference-chat-history-disappears/1230990; chaty po přechodu na Business https://community.openai.com/t/chat-history-lost-after-upgrading-from-chatgpt-plus-to-business/1383802; starý kontext v nových chatech Reddit r/ChatGPT (archivní kopie).
- AI radar vaultu: k volbám nastavení ChatGPT nic, stav k 3. 11. 2026.
