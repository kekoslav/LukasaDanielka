# Lukáš & Danielka – svadobná web stránka

Tento projekt je jednoduchá **statická web stránka** vytvorená pomocou **HTML, CSS a JavaScriptu**.  
Slúži na zverejnenie svadobných informácií pre hostí (program, miesto, RSVP, kontakty).

Projekt je navrhnutý tak, aby mu rozumel **začiatočník v programovaní** a aby fungoval bez servera alebo databázy.

---

## Štruktúra projektu

Projekt obsahuje tieto súbory:

- **index.html**  
  Obsahuje štruktúru stránky:
  - navigáciu (menu),
  - jednotlivé sekcie stránky,
  - texty a odkazy,
  - vložený RSVP formulár (Google Form).

- **style.css**  
  Obsahuje vzhľad stránky:
  - farby,
  - písma,
  - rozloženie prvkov,
  - responzívne správanie (mobil / tablet / desktop).

- **script.js**  
  Obsahuje logiku stránky:
  - odpočítavanie do dátumu svadby,
  - plynulé scrollovanie po kliknutí na menu,
  - ovládanie mobilného (hamburger) menu.

Všetky súbory musia byť uložené v **jednom priečinku**.

---

## Na čom stránka funguje

- Beží v moderných webových prehliadačoch:
  - Google Chrome
  - Mozilla Firefox
  - Microsoft Edge
  - Safari
- Nepotrebuje:
  - server,
  - databázu,
  - backendový kód.
- Používa externé služby:
  - Google Fonts (písma),
  - externý obrázok ako pozadie,
  - Google Form ako RSVP formulár (vložený cez iframe).

---

## Ako stránku spustiť

### Možnosť 1 – dvojklik (najjednoduchšie)

1. Otvor priečinok s projektom.
2. Dvojklikni na súbor **index.html**.
3. Stránka sa otvorí v prehliadači.

### Možnosť 2 – VS Code + Live Server (odporúčané)

1. Nainštaluj **Visual Studio Code**.
2. Nainštaluj rozšírenie **Live Server**.
3. Otvor priečinok s projektom vo VS Code.
4. Pravým klikom na `index.html` vyber **Open with Live Server**.

Výhoda: po uložení zmien sa stránka automaticky obnoví.

---

## Ako stránku upravovať

### Úprava obsahu (index.html)

V súbore `index.html` môžeš upravovať:
- mená,
- dátum svadby,
- program dňa,
- informácie o mieste,
- kontakty,
- texty v sekciách,
- RSVP formulár (iframe odkaz).

Typické úpravy:
- doplnenie mien a telefónnych čísel,
- doplnenie čísla účtu,
- zmena odkazu na Google Form,
- úprava textov pre hostí.

---

### Úprava dizajnu (style.css)

V súbore `style.css`:
- na začiatku sú definované farby a písma (CSS premenné),
- trieda `.hero` definuje úvodnú sekciu s pozadím,
- `@media` sekcie riešia mobilné zobrazenie.

Príklady zmien:
- zmena hlavnej farby stránky,
- zmena písma,
- zmena hero obrázka,
- úprava rozloženia pre mobilné zariadenia.

---

### Úprava správania stránky (script.js)

V súbore `script.js` sa nachádza:

#### Odpočítavanie do svadby

const weddingDate = new Date("2026-08-14T15:00:00+02:00").getTime();
Tu môžeš zmeniť dátum a čas svadby.

---

## Scrollovanie

Kliknutie na položky v menu plynulo presunie stránku na príslušnú sekciu.

---

## Mobilné menu

Kliknutím na hamburger ikonku sa menu zobrazí alebo skryje.  
JavaScript prepína CSS triedy.

---

## Najčastejšie úpravy – prehľad

| Čo chceš zmeniť | Súbor |
|-----------------|-------|
| Texty, mená, časy | index.html |
| Dátum odpočítavania | script.js |
| Farby a písma | style.css |
| Pozadie (hero obrázok) | style.css |
| RSVP formulár | index.html |
| Mobilné menu | style.css + script.js |

---

## Zverejnenie stránky (hosting)

Stránku je možné zverejniť zadarmo:

### GitHub Pages

1. Nahraj projekt do GitHub repozitára.
2. Otvor **Settings → Pages**.
3. Vyber branch (napr. `main`) a root folder.
4. GitHub vygeneruje verejnú URL stránky.

### Netlify alebo Vercel

- Nahraj priečinok alebo prepoj GitHub repozitár.
- Nasadenie prebehne automaticky bez ďalšej konfigurácie.

---

## Odporúčania pre začiatočníka

- Rob malé zmeny a často stránku testuj.
- Po každej zmene súbor ulož.
- Ak niečo nefunguje:
  - skontroluj názvy súborov,
  - skontroluj, či sú v rovnakom priečinku,
  - otvor **Developer Tools (F12)** a pozri konzolu.
- Neboj sa experimentovať – projekt je vhodný na učenie.

---

## Zhrnutie

Tento projekt:
- je jednoduchý a prehľadný,
- je vhodný pre začiatočníkov,
- nevyžaduje server ani databázu,
- dá sa ľahko upravovať a zverejniť.

Slúži ako praktický prvý projekt na pochopenie základov webového vývoja.
