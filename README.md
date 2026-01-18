# Exacto Cuatro

Een gepersonaliseerde versie van het NRC "Precies Vier" spel.

## Bestanden

- `index.html` - Het hoofdspel (menu + spelscherm)
- `puzzels.json` - De puzzeldata
- `admin.html` - Beheerderspaneel om nieuwe puzzels te maken

## Installatie op GitHub Pages

### Stap 1: Repository aanmaken
1. Ga naar [github.com](https://github.com) en log in
2. Klik op het **+** icoon rechtsboven → **New repository**
3. Geef het een naam, bijv. `exacto-cuatro`
4. Zet het op **Public** (nodig voor gratis GitHub Pages)
5. Klik **Create repository**

### Stap 2: Bestanden uploaden
1. Klik op **uploading an existing file**
2. Sleep alle drie de bestanden (`index.html`, `puzzels.json`, `admin.html`) naar het upload veld
3. Klik **Commit changes**

### Stap 3: GitHub Pages activeren
1. Ga naar **Settings** (tandwiel icoon)
2. Scroll naar **Pages** in het linkermenu
3. Onder "Source" selecteer **Deploy from a branch**
4. Selecteer **main** branch en **/ (root)**
5. Klik **Save**

### Stap 4: Link delen
Na een paar minuten is je site live op:
```
https://[jouw-gebruikersnaam].github.io/exacto-cuatro/
```

Sophie kan deze link openen op haar iPhone!

## Puzzels toevoegen

### Via het beheerderspaneel
1. Ga naar `https://[jouw-gebruikersnaam].github.io/exacto-cuatro/admin.html`
2. Log in met het wachtwoord (standaard: `sophie2024`)
3. Vul de puzzel in
4. Klik **Genereer JSON**
5. Kopieer de code

### In GitHub plakken
1. Open `puzzels.json` in je repository
2. Klik op het potlood-icoon (Edit)
3. Voeg een komma toe na de laatste `}` 
4. Plak de nieuwe puzzel erboven
5. Klik **Commit changes**

### Voorbeeld puzzels.json met meerdere puzzels:
```json
[
    {
        "id": "puzzel-1",
        "name": "Eerste puzzel",
        "categories": [...]
    },
    {
        "id": "puzzel-2",
        "name": "Tweede puzzel",
        "categories": [...]
    }
]
```

## Wachtwoord wijzigen

Open `admin.html` en zoek deze regel:
```javascript
const ADMIN_PASSWORD = 'sophie2024';
```
Wijzig `sophie2024` naar je eigen wachtwoord.

## Voortgang resetten

Sophie's voortgang (vinkjes) wordt opgeslagen in haar browser. Om te resetten kan zij:
1. De browsercache/data voor de site wissen, of
2. In de browser console: `localStorage.removeItem('exactoCuatroProgress')`

---

Veel plezier met puzzelen! 🧩
