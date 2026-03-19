# Kripto Kladionica — SEO Paket: Dokumentacija & Upute

---

## Što je isporučeno

| Datoteka | Opis |
|---|---|
| `index.html` | Originalna stranica s potpuno optimiziranim `<head>` |
| `sitemap.xml` | XML sitemap za Google Search Console |
| `robots.txt` | Direktive za crawlere, blokiran `/admin` |

---

## 1. Što je dodano u `<head>`

### Title & Meta Description
```
Title:       Kripto Kladionica — Sportsko Klađenje s USDT | Bez KYC & Anonimno
Description: Kladi se na sport s USDT kriptovalutom — bez KYC provjere, potpuno anonimno...
```
- Title je unutar preporučenih 50–60 znakova (vidljivo u Google rezultatima)
- Description je unutar 150–160 znakova
- Sadrži primarne ključne riječi: **kripto kladionica**, **USDT**, **bez KYC**, **anonimno**

### Canonical URL
```html
<link rel="canonical" href="https://kriptokladionica.com/">
```
**⚠️ Obavezno zamijeni** `kriptokladionica.com` s tvojom stvarnom domenom.

### Open Graph (Facebook, WhatsApp, LinkedIn dijeljenje)
Kada netko podijeli link na društvenim mrežama, prikazat će se:
- Naslov, opis i slika
- **Trebaš kreirati:** `og-image.png` (1200×630 px, tamna pozadina, logo + tagline)
- Postavi je na: `https://TVOJA_DOMENA.com/og-image.png`

### Twitter/X Card
- `summary_large_image` format — prikazuje veliku sliku uz objavu
- Koristi iste slike kao OG

### Strukturirani podaci (JSON-LD)

Dodana su **4 schema.org bloka**:

| Tip | Svrha |
|---|---|
| `Organization` | Google prikazuje panel sa desne strane za brandove |
| `WebSite` | Aktivira Sitelinks Searchbox u Google rezultatima |
| `FAQPage` | FAQ se prikazuje **direktno u Google rezultatima** (rich snippet) |

FAQ pitanja koja su dodana:
1. Trebam li KYC verifikaciju?
2. Koje kriptovalute prihvaćate?
3. Koliko je brza isplata?
4. Je li stranica sigurna?

**Ova pitanja možeš mijenjati** — važno je da odgovaraju stvarnom sadržaju stranice.

### Performance meta tagovi
- `theme-color: #00e5a0` — boja naslova preglednika na mobitelu
- `dns-prefetch` za Google Fonts i Firebase — brže učitavanje
- `color-scheme: dark` — sprečava flash bijele pozadine

---

## 2. Postavljanje na server

### Datoteke koje trebaju biti u root direktoriju:
```
/
├── index.html
├── robots.txt
├── sitemap.xml
├── og-image.png          ← trebaš kreirati (1200×630px)
└── logo.png              ← koristi se u JSON-LD Organization schema
```

### Nakon postavljanja — obavezni koraci:

#### Google Search Console
1. Idi na: https://search.google.com/search-console
2. Dodaj svoju domenu
3. Verificiraj vlasništvo (HTML tag ili DNS)
4. Pošalji sitemap: `https://TVOJA_DOMENA.com/sitemap.xml`
5. Traži indeksiranje glavne stranice

#### Google Rich Results Test
Provjeri strukturirane podatke:
https://search.google.com/test/rich-results

Unesi URL i provjeri da li su FAQ i Organization schema ispravno prepoznati.

#### PageSpeed Insights
Provjeri brzinu:
https://pagespeed.web.dev/

---

## 3. Ključne riječi — primarni fokus

| Ključna riječ | Namjera pretrage |
|---|---|
| kripto kladionica | Korisnik traži kladionicu s kriptom |
| USDT klađenje | Korisnik zna koju kripto želi |
| kladionica bez KYC | Korisnik svjesno traži anonimnost |
| sportska kladionica bez verifikacije | Isti namjera, drugačiji izraz |
| anonimno klađenje | Privatnost kao prioritet |
| crypto betting hrvatska | Engleski izraz, HR publika |

**Savjet:** Ove ključne riječi trebaš koristiti i u **tekstualnom sadržaju** stranice (H1, H2, paragrafima) — ne samo u meta tagovima.

---

## 4. Ograničenja & napomene

### Domena
Sve što je dodano koristi placeholder domenu `kriptokladionica.com`.
**Zamijeni je s tvojom stvarnom domenom** u:
- `<link rel="canonical">`
- Svim `og:url` i `og:image` tagovima
- JSON-LD blokovima (`"url"`, `"logo"`)
- `sitemap.xml`
- `robots.txt` (Sitemap direktiva)

### Gambling & Google Ads
Google ograničava oglašavanje kockarskih stranica — organski SEO je ovdje ključan.
Prirodni backlinks (linkovi s foruma, kripto zajednica) su najvrjedniji.

### Single-Page App (SPA)
Stranica je SPA (sve na jednom `index.html`). Google uglavnom dobro indeksira SPA-ove,
ali preporuča se koristiti **Server-Side Rendering (SSR)** ili **prerendering** ako
organički promet postane primarni kanal.

---

## 5. Brza kontrolna lista

- [ ] Zamijeni `kriptokladionica.com` s pravom domenom
- [ ] Kreira `og-image.png` (1200×630 px)
- [ ] Kreira `logo.png` za JSON-LD
- [ ] Postavi sve datoteke u root direktorij
- [ ] Dodaj stranicu u Google Search Console
- [ ] Pošalji sitemap u Search Console
- [ ] Testiraj rich snippets na: search.google.com/test/rich-results
- [ ] Provjeri PageSpeed score

---

*Generirano za: Kripto Kladionica | USDT | NO-KYC | HR tržište*
