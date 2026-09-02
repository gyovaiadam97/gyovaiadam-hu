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
9. **Design:** a `DESIGN.md` (Downloads-ból bemásolva a projektbe) — „Henry" stílus: fekete vászon,
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
- 2026-09-02: oldal kész (`docs/index.html` + `docs/style.css`), repo publikus, Pages bekapcsolva main:/docs, cname=gyovaiadam.hu.
  Headless-Chrome tanulság: az ablak min. 500 px széles, mobil-nézethez iframe-be kell tenni (390 px).

## 8. Köv. lépések

1. **Ádám:** gyovaiadam.hu regisztrálása (Rackhost). Utána szólni.
2. **DNS** (Rackhost admin, Ádám belép, Claude vezérel): apex A → 185.199.108.153, .109.153, .110.153, .111.153;
   `www` CNAME → gyovaiadam97.github.io. TTL 300.
3. GitHub Pages: DNS-check zöld → cert kérés → `https_enforced=true` (gh api PUT .../pages -F https_enforced=true).
4. Ádám átnézi élőben a szövegeket és az ÁRAKAT (6. pont) → javítások.
5. Fotó/videó a hero-ba és a Rólam-szekcióba, amikor megvan.
6. 2. ütem: űrlap-backend (VPS + Brevo), analitika, angol.
