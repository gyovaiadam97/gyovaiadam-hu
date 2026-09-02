# gyovaiadam.hu — TERV

Állapot: **JÓVÁHAGYVA 2026-09-02, építés folyamatban.**

## 1. Cél

Side hustle indítása: „bármilyen szoftvert megépítek" szolgáltatás hirdetése egy saját domaines
landing oldalon (gyovaiadam.hu). Ugyanez az oldal a személyes CV / „minden, amit rólam tudni kell" hely.

Elsődleges konverzió: **érdeklődő megkeresés** (email / űrlap). Másodlagos: bizalomépítés
(referenciák, folyamat, ki vagyok).

Célközönség (feltételezés, pontosítandó): magyar KKV-tulajdonosok, szolgáltatók, tartalomgyártók,
akiknek belső eszköz, automatizálás, webapp vagy egy drága SaaS kiváltása kell, és nem akarnak
ügynökségi árat fizetni.

## 2. Tények, amikre építünk

- **Domain:** a gyovaiadam.hu **nincs regisztrálva** (whois.nic.hu: „Nincs találat", 2026-09-02).
  → Regisztrálni kell (javaslat: Rackhost, ahol a többi domain is van; kb. 3–5e Ft/év).
- **Bevált hosting-minta:** trustfunnel.hu GitHub Pages-en, saját domain + Let's Encrypt, ingyen, működik.
  Ellenpélda: novastudio.hu-nál a GitHub cert-kiadás beragadt. Itt viszont ÚJ domain → nincs forgalom,
  nincs kiesés-kockázat, ráérünk kivárni; ha beragad, B-terv a VPS.
- **VPS:** Hostinger VPS él (sonia.hu + GlitchTip fut rajta) — B-terv hostingnak, és a kapcsolati űrlap
  backendjének (ha lesz).
- **GitHub:** gyovaiadam97, gh CLI bejelentkezve.

## 3. Ajánlott megoldás

### Stack
- **Statikus oldal, egyetlen HTML + CSS + minimális JS**, keretrendszer nélkül. Indok: tartalom-oldal,
  nincs állapot, nincs backend-logika; a SvelteKit itt felesleges réteg. (A CLAUDE.md webapp-szabályai
  interaktív appra vonatkoznak; ez nem az.)
- Betűtípus: Google Fonts (2 család max), ikonok inline SVG. Képek WebP, méretre optimalizálva.
- Nyelv: **magyar** (elsődleges). Angol verzió: 2. ütem, ha kell (/en).
- Repo: `gyovaiadam97/gyovaiadam-hu` (public — GitHub Pages ingyen csak public repóról; titok nincs benne).
- Hosting: **GitHub Pages** (main ág, `/docs`), CNAME = gyovaiadam.hu, www → apex átirányítás.
- DNS (Rackhost, dns24 zóna): apex 4× A → 185.199.108–111.153, www CNAME → gyovaiadam97.github.io.
- Analitika: 2. ütem (opcionálisan Plausible/Umami saját VPS-en — cookie-mentes, nem kell süti-banner).

### Kapcsolatfelvétel
- MVP: kiemelt **email-cím** (kattintható + másolható), plusz opcionálisan telefon/Telegram/LinkedIn.
- 2. ütem: űrlap → kis FastAPI-végpont a VPS-en → Brevo email Ádámnak (spam-védelem: honeypot + rate limit).
  Statikus oldalról más nem megy backend nélkül; külső form-szolgáltatás (Formspark stb.) is opció.

### Oldalszerkezet (egyoldalas, szekciók)
1. **Hero** — „Bármilyen szoftvert megépítek a vállalkozásodnak." Alcím: mit, kinek, miért gyors/olcsó
   (AI-alapú fejlesztés, fix ár, hetek nem hónapok). CTA: „Írj, és 24 órán belül válaszolok."
2. **Mit építek** — 6 kártya: belső eszköz/vezérlőpult · webapp · automatizálás/AI-integráció ·
   drága SaaS kiváltása saját appal · macOS app / Premiere plugin · landing/weboldal.
3. **Referenciák** — 6–8 valós projekt, mind: probléma → megoldás → eredmény (számmal, ha van):
   - AdyPod — Premiere plugin (jumpcut + multicam), AutoPod-előfizetés kiváltása, 3 vágógépen éles
   - Ady / AdyCaptions — feliratozó webapp, Submagic + Alrite kiváltása, 4 munkatárs használja
   - Sonia (sonia.hu) — 21 napos önismereti interjú webapp, éles, Postgres + hibakövetés
   - Scribe — macOS meeting-jegyző (helyi átirat + AI-összefoglaló + Notion)
   - Investo — befektetési portfólió-elemző webapp (FastAPI + SvelteKit)
   - Nova Offload — archiváló app (Offshoot kiváltása), natív GUI
   - Számla-átnevező — AI-s számla-feldolgozó, 17 számla 73 mp alatt
   - trustfunnel.hu — Framer-oldal kiváltása statikus oldallal (évi ~60e Ft megtakarítás)
   - (Memory Book preview — csak Steve engedélyével)
   Vezérfonal: **4 fizetős előfizetést váltottam ki saját szoftverrel** — ez a legerősebb üzenet.
4. **Hogyan dolgozom** — 5 lépés: igényfelmérés (30 perc hívás) → írásos specifikáció + fix ár →
   építés heti demókkal → teszt közösen → átadás + üzemeltetés/karbantartás opció.
5. **Rólam / CV** — fotó + rövid sztori: Nova Produkciós Iroda társalapító és CFO (2023–), pénzügyi
   háttér → érti az üzleti oldalt is; Kezdő Befektető (11 000+ követő, 1 000+ hírlevél-olvasó,
   200+ kurzusvásárló); technológiák: Python/FastAPI, TypeScript/SvelteKit, Postgres, Claude Agent SDK,
   VPS-üzemeltetés, macOS/Premiere-bővítmények. Tanulmányok + korábbi munkák: **Ádámtól kell**.
6. **Árazás / mire számíts** — sáv-jellegű (pl. „kis automatizálás X-től, teljes webapp Y-tól") vagy
   csak „fix ár a spec után". **Ádám dönt.**
7. **GYIK** — 5–6 kérdés (mennyi idő, ki üzemelteti, kié a kód, mi van ha elromlik, AI-val készül-e).
8. **Kapcsolat** — email, (telefon), LinkedIn, GitHub; lábléc: impresszum-minimum (név, székhely, adószám
   — ha van vállalkozói forma).

### Design
- Saját, egyszerű arculat: **nem** a KB (zsálya) és nem a Nova arculat — ez személyes fejlesztői brand.
- Javaslat: világos alap, egy erős akcentszín, sok fehér tér, nagy tipó; sötét mód automatikus
  (prefers-color-scheme). Mobilon először tervezve.
- Szükséges Ádámtól: 1 jó portréfotó (+ opcionálisan 2–3 screenshot a referenciákhoz — a Nova-s
  appokról készíthetek).

### Szövegírás
- Humanizer-elvek, nincs gondolatjel (—), nincs AI-frázis. Copy-vázlat a copywriting-operator
  doktrína alapján (offer + bizonyíték + kockázatcsökkentés).

## 4. Ütemezés

| # | Lépés | Ki | Állapot |
|---|-------|----|---------|
| 0 | Terv jóváhagyása + nyitott kérdések megválaszolása | Ádám | ✅ 09-02 |
| 1 | Domain regisztrálása (Rackhost) | Ádám (Claude másodpilóta) | ⬜ |
| 2 | Szöveg-vázlat (minden szekció) → Ádám átnézi | Claude → Ádám | ✅ 09-02 (beépítve az oldalba, Ádám átnézi élőben) |
| 3 | Design + HTML/CSS megépítése, lokális preview | Claude | ✅ 09-02 |
| 4 | Fotó + hiányzó CV-adatok beépítése | Ádám ad, Claude épít | ⬜ |
| 5 | Repo + GitHub Pages + DNS + HTTPS | Claude (DNS: Ádám lép be, Claude vezérel) | 🟡 repo+Pages kész (gyovaiadam97/gyovaiadam-hu, CNAME beállítva); DNS + HTTPS a domain-regisztráció után |
| 6 | Ellenőrzés: mobil/desktop, Lighthouse, linkek, cert | Claude | 🟡 mobil/desktop headless-screenshot OK (390/1440 px, nincs vízszintes túlcsordulás); cert+Lighthouse élesítés után |
| 7 | 2. ütem: űrlap-backend, analitika, angol verzió | később | ⬜ |

Becslés: 1–3. lépés egy ülésben; élesítés a domain-regisztráció + DNS-átfutás után (órák–1 nap).

## 5. Döntések (Ádám válaszai, 2026-09-02)

1. **Számlázás:** egyéni vállalkozóként. (Impresszum-adatok: név + „egyéni vállalkozó"; székhely/adószám
   később, ha Ádám megadja.)
2. **Árazás:** árak kimehetnek. Konkrét számokat Ádám nem adott → Claude javasolt sávokat tett az oldalra
   (lásd 7. pont), **Ádámnak jóvá kell hagynia vagy átírnia**.
3. **CV:** NEM klasszikus önéletrajz. A „kóding vonalat" a referenciák mutatják be; tanulmányok, korábbi
   munkák nem kellenek.
4. **Referenciák:** MINDEN saját app/webapp/szoftver mehet: AdyPod, Ady, Offload, Scribe, Sonia, Investo,
   Számla-átnevező, trustfunnel.hu, podcast-ajánlat weboldal (podcast.novastudio.hu) stb.
   **Memory Book NEM mehet** (nem Ádámé).
5. **Kapcsolat:** csak gyovaiadam97@gmail.com egyelőre.
6. **Fotó/videó:** placeholderrel indulunk; később fotók + videó Ádámról (a hero-ba tervezve).
7. **Hosting:** GitHub Pages.
8. **Nyelv:** csak magyar.
9. **Design:** a `DESIGN.md` (Downloads-ból bemásolva a projektbe) — „Henry" stílus. **A forrás az élő www.ai.work oldal** (a refero.design csak ebből vonta ki a tokeneket); az elrendezést onnan másoltuk szekciónként (2026-09-02, 2. kör). Stílus: fekete vászon,
   300-as súlyú világos címek, pill gombok, hajszálvékony warm-gray keretek, chromatikus szín csak a
   stat-sávokban. NB International Pro helyett Inter (300/400/500) + JetBrains Mono (a doksi saját
   helyettesítési ajánlása szerint, Google Fonts).

## 6. Árazás-javaslat (JÓVÁHAGYANDÓ)

Tájékoztató „-tól" sávok az oldalon, a pontos ár a spec után fix:
- Automatizálás, kis eszköz (1–2 hét): **250 000 Ft-tól**
- Belső eszköz, weboldal, landing (2–4 hét): **600 000 Ft-tól**
- Teljes webapp, előfizetés kiváltása (4–8 hét): **1 500 000 Ft-tól**
- Üzemeltetés, karbantartás: **25 000 Ft/hó-tól**
ÁFA-státusz nincs kiírva (Ádám adja meg: alanyi adómentes-e).

## 7. Napló

- 2026-09-02: projekt indul, terv megírva, domain-állapot ellenőrizve (nincs regisztrálva).
- 2026-09-02: Ádám jóváhagyta, válaszok beépítve, DESIGN.md átvéve; építés indul.
- 2026-09-02: oldal kész (`docs/index.html` + `docs/style.css`), repo publikus, Pages bekapcsolva main:/docs.
- 2026-09-02: domain-regisztráció elhalasztva (Ádám később veszi meg), ezért a CNAME ideiglenesen LEVÉVE; előnézet: https://gyovaiadam97.github.io/gyovaiadam-hu/ (200, ellenőrizve). Domain után: `docs/CNAME` vissza + Pages cname beállítás.
  Headless-Chrome tanulság: az ablak min. 500 px széles, mobil-nézethez iframe-be kell tenni (390 px).

## 8. Köv. lépések

1. **Ádám:** gyovaiadam.hu regisztrálása (Rackhost), később. Utána: `printf 'gyovaiadam.hu\n' > docs/CNAME` + push + `gh api -X PUT repos/gyovaiadam97/gyovaiadam-hu/pages -f cname=gyovaiadam.hu`.
2. **DNS** (Rackhost admin, Ádám belép, Claude vezérel): apex A → 185.199.108.153, .109.153, .110.153, .111.153;
   `www` CNAME → gyovaiadam97.github.io. TTL 300.
3. GitHub Pages: DNS-check zöld → cert kérés → `https_enforced=true` (gh api PUT .../pages -F https_enforced=true).
4. Ádám átnézi élőben a szövegeket és az ÁRAKAT (6. pont) → javítások.
5. Fotó/videó a hero-ba és a Rólam-szekcióba, amikor megvan.
6. 2. ütem: űrlap-backend (VPS + Brevo), analitika, angol.
- 2026-09-02 (2. kör): Ádám visszajelzése: nem hasonlított eléggé a refero-sablonra. Kiderült, hogy a sablon az élő **www.ai.work** oldal; azt szekciónként végigfotóztam és a számított stílusértékeket kimértem (body #141414, nem fekete; chipek bone 4%, 4px; címke-pill bone 10% + mono 10px; kártyák 8px, 24px padding; hero 8px beljebb, 8px radius; záró CTA 96px). Az oldal teljesen újraépítve az eredeti szerkezetére: keretezett hero fotóval + lebegő fehér kártyák, vízszintes munkakártya-sor számlálóval, 3 stat-kártya, keretezett idővonal-kártya (folyamat), eredmény-idézet, váltakozó feature-sorok mockokkal, üzemeltetés-inbox, lebegő eszköz-chipek, bento-árak, Rólam, GYIK, 96px CTA, lábléc óriás wordmarkkal, lebegő „Írj nekem" gomb.
  Hero-fotó: Artlisttel generált aranyórás hegyi táj (130 kredit), `docs/img/hero.webp` + `hero-m.webp` + `og.jpg`. Tanulság: a DESIGN.md tokenlista önmagában nem elég, mindig az eredeti oldal URL-je/képernyőképe kell.
- 2026-09-02 (3. kör, „az animációk hiányoznak"): CSS+vanilla JS animációk az eredeti mintájára: hero belépő (kép zoom+fade, sorok lépcsőzetesen, fehér kártyák felúsznak, pörgő státusz, villogó kurzor), görgetésre megjelenés (`data-reveal`, görgetés-pozíció alapú ellenőrzés + 250 ms-os tartalék-poll; NEM IntersectionObserver, mert az átugrott elemeket sosem mutatta meg), felpörgő számok, sorban kigyulladó idővonal + ↺ újra-gomb, mock-animációk (terminál gépelés, előfizetés-pill váltás, chat-üzenetek, shimmer), inbox-üzenetek beúszása, lebegő eszköz-chipek, óriás wordmark felúszása, `prefers-reduced-motion` tisztelve.
  Teszt-tanulság: rejtett Chrome-fülben és headless virtual-time alatt a scroll-esemény és a rAF nem fut → a görgetés-alapú animációt csak setTimeout-os szkripttel (scroll-behavior:auto) lehet headlessben igazolni; a `.in` osztálynév ütközött a `.big .in` grid-szelektorral (átnevezve `big-in`).
- 2026-09-02 (4. kör, „nem tetszik, alkosd újra"): új refero-sablon = **www.getharvest.com** (Harvest). A Chrome-extension épp nem élt, ezért curl + headless Chrome: a refero HTML-ből kinyerve a DESIGN.md (`DESIGN-harvest.md`) és az eredeti URL; a Harvest oldal teljes képernyőképe + CSS-fájljai letöltve, színek pixelből mérve (alap #fbf5f0, barack kártya #f3ebe4, korall #fba37f, narancs #fa5d00, tinta #1d1e1c, meleg árnyék `0 4px 10px rgba(123,85,31,.21)`), betűk: Besley (Google Fonts, az eredeti is ezt tölti) + Inter a Muoto helyett.
  Szerkezet 1:1 a Harvest nyomán: lebegő fehér pill-nav; hero két oszlop (serif 72px forgó szóval + narancs kézi aláhúzás, email-„input" + fekete pill, pipák; jobbra korall keretes app-mock ütemtervvel és kéz-kurzorral); bizalmi sáv (technológiák szürke wordmarkokként); „Mit építek" kártyasor kézi rajzos ikonokkal + nyilak; „Munkáim" tab-pill sor + két oszlop + csíkos barack keretben fehér mock-kártya lebegő fekete gombbal (8 projekt-fül); „Folyamat" bento 3+2 illusztrált kártya; „Árak" stat-sor + barack ár-kártyák (Harvest testimonial-kártya mintájára) + nyilak + CTA; Rólam; GYIK; korall CTA-kártya fehér belsővel + mock; lábléc link-oszlopok + „Kezdd itt" kártya.
  Az előző (Henry/ai.work) verzió: `archive/index-henry.html` + `archive/style-henry.css`.
- 2026-09-02 (5. kör): Ádám szerint „nagyon jó” a Harvest-verzió; a hero ütemterv-mockja lecserélve szoftverkészítés-grafikára: IDE-ablak (fülek, Futtatás-gomb), fent a kérés buborékban, balra soronként gépelődő Python-kód (14 mp-es hurok), jobbra élő előnézet, amiben az app elemei a kód ütemére jelennek meg, végül zöld „Tesztek: 12/12” jelvény; kéz-kurzor a gombon. Csak CSS-keyframe, reduced-motion tisztelve.
- 2026-09-02 (6. kör, „komolyabb, látványosabb, modernebb, futurisztikusabb"): a kód-ablak helyett Artlist-render (Nano Banana 2, 3 változat, 390 kredit): lebegő üveg UI-panelek narancs fényáramokkal krém háttéren; a 2. (izzó, dinamikus) változat került be `docs/img/hero-3d.webp` (+ mobil és og.jpg). CSS: radiális narancs glow lüktetéssel, lassú lebegés, három üveg-jelvény (Specifikáció elfogadva / 12/12 teszt / Heti demó). A korall keret a hero-ból kikerült, a CTA-kártyában maradt. Opció későbbre: image-to-video ugyanebből a képből, ha mozgó hero kell.
- 2026-09-02 (7. kör, „pixeles retro design programozó-ikonnal és számítógéppel"): a 3D-render helyett pixel art a hero-ban. Artlist (3 változat, 390 kredit) → az 1. (közeli, szemüveges programozó CRT előtt, narancs bögre, floppy) 240 px szélesre kicsinyítve + 32 színű palettára kvantálva, így valódi pixelrács (`docs/img/hero-pixel.png`, 25 KB, `image-rendering: pixelated`). Retro ablak: 4 px tintakeret, korall „árnyék", fekete címsor Press Start 2P fonttal (GYOVAIADAM.EXE), scanline-réteg, BUILD-csík lépcsős animációval + százalék-számláló, villogó blokk-kurzor, három pixel-jelvény (+1 APP KÉSZ / 12/12 TESZT OK / LVL 9 · SZOFTVER). A 3D-render (`hero-3d.webp`) a repóban marad tartaléknak.
- 2026-09-02 (8. kör, „legyen nagyobb, esztétikus"): a pixel-kép a tartalom befoglaló dobozára vágva (4:3), 256 px-es rácsra kvantálva; a hero-rács 0.85fr/1.35fr, a cím 66 px, az ablak 24 px-szel túlnyúlik jobbra; az ablak háttere a kép pontos krémszíne, hogy ne látszódjon szegély.
- 2026-09-02 (9. kör, „ezt megtartanám, kérek egy újabb verziót ezzel a designnal, a végén döntök"): új refero-sablon = **www.monad.com** (Monad, Webflow). Chrome-extension nem élt → curl + headless; DESIGN-v2.md kinyerve; monad.com CSS-ből a valódi fontok (Untitled Serif + ABC Diatype Mono, fizetősek → Newsreader + IBM Plex Mono), színek (#f6f3f1 pergamen, #242424, #2b59d1 kék, #cfdaf5 periwinkle, pasztell washok), 40 px kártyák, 100 px pillek, 1 px #cecac8 keretek. A Monad középső szekciói headlessben nem renderelődtek (Webflow-animáció), azokat a HTML-szövegből és a tokenekből rekonstruáltam.
  **v2 külön oldal: `docs/v2/`** (index.html + style.css, noindex), a v1 (Harvest + pixel-hero) érintetlen a gyökérben. Szerkezet: fekete bejelentő sáv; nav (pöttyös kör-logó, mono uppercase linkek, fekete + kék pill); tipográfiai hero (serif 80 px) + a Monad jellegzetes csatorna-diagramja a folyamatra fordítva (bal: ötlet/Excel/kézi munka/drága előfizetés/fejben tartott folyamat → középső rombusz-hub Spec/Építés/Teszt/Átadás címkékkel, zöld glow, pörgő pöttyös logó → jobb: webapp/belső eszköz/automatizálás/macOS/weboldal; animált szaggatott vonalak, mobilon pill-lista); eszköz-sáv; „Hogyan dolgozom" 3 keretes kártya mini-illusztrációval; periwinkle „Munkáim" kártya pasztell wash-sal és függőlegesen görgő projekt-pillekkel; 9 projekt-kártya színes wash-sal; „Miért velem" 2×2; „Három lépésben"; árak 4 kártya; Rólam; GYIK ↓-nyilakkal; arany→narancs gradiens CTA-kártya; lábléc órával. Tanulság: a hero gombsorát `.cta`-nak hívtam, ütközött a CTA-kártyával → `.hero-cta`.
- 2026-09-02 (10. kör): a Monad-v2 Ádám kérésére törölve (git-előzményben megvan). Új v2 = **www.altitude.so** (Altitude, „midnight financial editorial"): #181818 vászon, #111/#1f/#26/#32 felület-lépcső, #eeeeee szöveg, #a4a19b másodlagos, egyetlen kék #2b7fff linkekre; Libre Baskerville 400 címek (72/48 px), Inter test, Fira Code a terminálban, mind Google Font, ahogy az eredetin is; 4 px gombok, 8 px kártyák, 16 px képkeret, hajszálkeretek, alig-árnyékok. Az Altitude egy React-SPA, headlessben csak a hero renderelt, a többi szekciót a refero részletes komponens-leírásaiból + a HTML szövegéből építettem.
  Szerkezet: 64 px nav (hegy-glif + GYOVAIADAM); tipográfiai hero fehér inverz gombbal és **1 px-es hegygerinc-vonallal** (generált SVG-path, betöltéskor kirajzolódik); „Egy ember, aki az egész projektet viszi" 40/60 split: jobbra terminál-ablak (traffic-light, sidebar, Fira Code, soronként megjelenő spec + tesztek) egy Artlisttel generált kék-szürke festői hegyi fotó fölött (`docs/v2/img/mtn.webp`, 130 kredit); „Mit építek" = az egyetlen világos blokk, 5 oszlopos off-white csempe-rács ikonokkal; „Munkáim" = terminál-stílusú adattábla 9 sorral (projekt/típus/mit váltott ki/eredmény/állapot-badge); „Kiszámítható folyamat" 3 kártya mini-táblával, statokkal, deploy-log-gal; árak 4 kártya; Rólam fotókerettel; számozott GYIK (01 .); záró CTA; #111 lábléc.
- 2026-09-02 (11. kör): v2 hero: a hegygerinc-vonal helyett 1 px-es vonalas „építési útvonal": vízszintes vonal 4 csomóponttal (Specifikáció, Építés, Teszt, Átadás; balra Ötlet felirat), a végén vonalas app-ablak (Kész szoftver); betöltéskor kirajzolódik, majd egy fénypont fut végig rajta (SMIL animateMotion). Ugyanaz a #a4a19b, 1.4 px vonalnyelv, mint az Altitude-é.
- 2026-09-02 (12. kör, „egybefüggő és látványosabb"): a v2 hero-ábra szélétől szélig futó, egybefüggő vonal: balról három bemeneti ág (Ötlet, Excel-tábla, Kézi munka) fut össze a Specifikációnál; az Építésnél három párhuzamos build-ág commit-pontokkal (Heti demók), újra egyesül a Teszt rombusznál; Átadás után áthalad a vonalas app-ablakon (villogó kurzor) és kifut jobbra. Négy fénypont fut rajta eltolással, a csomópontok gyűrűként felvillannak, amikor a pont odaér (SMIL). Betöltéskor lépcsőzetesen rajzolódik ki. Arányosan skálázódik (viewBox meet, aspect-ratio).

## 9. Állapot 2026-09-02 este (holnap folytatjuk)
- **v1** (Harvest-stílus + pixeles retro hero): https://gyovaiadam97.github.io/gyovaiadam-hu/
- **v2** (Altitude-stílus, sötét szerkesztőségi, egybefüggő animált építési útvonal a hero-ban): https://gyovaiadam97.github.io/gyovaiadam-hu/v2/
- **Ádám dönt a kettő között.** A nyertes marad a gyökérben, a másik az `archive/` mappába kerül (a Henry-verzió már ott van).
- Nyitott: árak jóváhagyása (250e/600e/1,5M/25e Ft-tól, 30 nap díjmentes javítás), AdyPod-„Eredmény" mondat, hero-kártyák példaszövegei (v1), portré/videó, domain-regisztráció → CNAME vissza + DNS.
- Sonia-mellékszál: a 2. etap kiválasztó tesztjénél a teszt-visszaállító szkript futott közben (másik Claude-munkamenet); talált hiba: dupla javaslat-generálás párhuzamos betöltésnél → zár kell (a Sonia-munkamenetnek jelezve Ádám által).
