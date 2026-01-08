# Salinas Construct SRL - Website Oficial

Site web modern și minimalist pentru Salinas Construct SRL, companie specializată în construcții, renovări și instalații.

## 🎨 Identitate Brand

Site-ul folosește identitatea oficială a brand-ului Salinas Construct:
- **Logo Oficial** - Logo circular cu lucrători în construcție (assets/identity.png)
- **Paleta de Culori Brand** (assets/palette.jpg):
  - 🖤 **Negru** (#1A1A1A) - Profesionalism și soliditate
  - 🟡 **Galben Auriu** (#FFD700) - Excelență și calitate premium
  - ⚫ **Gri Charcoal** (#333333) - Modernitate și eleganță
  - ⚪ **Alb** (#FFFFFF) - Claritate și spațiu

## 🎯 Caracteristici

- **✅ Brand Identity Integration** - Logo și culori oficiale ale companiei
- **Design Modern** - Design curat cu accentele galbene din brand
- **Responsive Design** - Optimizat pentru desktop, tabletă și mobile
- **Multilingv** - Suport complet pentru Română și Engleză
- **Servicii Interactive** - Carduri clickable cu modale detaliate (5 servicii complete)
- **Animații Fluide** - Tranziții și efecte moderne cu culorile brand-ului
- **Portfolio Interactiv** - Galerie cu filtre pentru proiecte (cu suport pentru imagini înainte/după)
- **Formular Contact** - Formular functional pentru solicitări de ofertă

## 📂 Structura Proiectului

```
ludo-mvp/
├── assets/
│   ├── identity.png    # Logo oficial Salinas Construct
│   └── palette.jpg     # Paleta de culori brand
├── index.html          # Pagina principală cu toate secțiunile
├── styles.css          # Stiluri cu culorile brand
├── script.js           # Funcționalitate JavaScript și suport multilingv
├── README.md          # Documentația proiectului
└── TODO.md            # Lista taskuri viitoare
```

## 🎨 Secțiuni Website

1. **Hero Section** - Secțiune principală cu titlu impact și call-to-action
2. **Servicii** - 5 servicii principale:
   - Renovări și Modernizări
   - Finisaje Interioare
   - Instalații Electrice
   - Instalații Sanitare
   - Instalații Acoperișuri
3. **Portofoliu** - Galerie proiecte cu sistem de filtrare (6 proiecte placeholder)
4. **Despre Noi** - Informații despre companie, statistici și echipă (4 membri)
5. **Certificări** - Certificări și parteneri (ISO 9001, ANRE, ISCIR)
6. **Blog** - Secțiune pentru articole și știri (3 articole placeholder)
7. **Contact** - Formular de contact și informații de contact
8. **Footer** - Links rapide, social media și informații legale

## 🚀 Cum să Rulezi Website-ul

### Metoda 1: Deschide Direct în Browser
Dublu-click pe fișierul `index.html` pentru a deschide site-ul direct în browser.

### Metoda 2: Server Local (Recomandat)
Pentru funcționalitate completă, rulează un server local:

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (dacă ai instalat)
npx http-server -p 8000
```

Apoi deschide `http://localhost:8000` în browser.

## 📸 Adăugare Imagini

Site-ul folosește momentan placeholder-uri pentru imagini. Pentru a adăuga imaginile tale:

### Pentru Portofoliu (Înainte/După):
1. Salvează imaginile în format: `project-1-before.jpg`, `project-1-after.jpg`, etc.
2. În `index.html`, găsește secțiunea `.portfolio-item` și înlocuiește:
```html
<div class="portfolio-image placeholder">
    <!-- Placeholder -->
</div>
```
Cu:
```html
<img src="path/to/project-1-before.jpg" alt="Proiect 1" class="portfolio-image">
```

### Pentru Echipă:
Înlocuiește `<div class="team-photo placeholder-small">` cu:
```html
<img src="path/to/team-member.jpg" alt="Nume" class="team-photo">
```

### Pentru Blog:
Înlocuiește `<div class="blog-image placeholder">` cu:
```html
<img src="path/to/blog-image.jpg" alt="Titlu articol" class="blog-image">
```

## 🌐 Schimbarea Limbii

Website-ul suportă Română și Engleză. Utilizatorii pot schimba limba folosind butoanele RO/EN din navbar. Limba preferată este salvată în `localStorage`.

## ✨ Funcționalități JavaScript

- **Navbar Sticky** - Navigare fixă cu efect scroll
- **Mobile Menu** - Meniu responsive pentru dispozitive mobile
- **Smooth Scroll** - Derulare fluidă între secțiuni
- **Portfolio Filter** - Filtrare proiecte după categorie
- **Stats Counter** - Animație contoare pentru statistici
- **Intersection Observer** - Animații la scroll
- **Form Validation** - Validare formular contact
- **Language Switcher** - Schimbare dinamică limbă RO/EN

## 🎨 Personalizare Culori

Variabilele de culoare se găsesc în `styles.css`:

```css
:root {
    --primary-color: #1a1a1a;      /* Culoare primară */
    --accent-color: #2563eb;        /* Culoare accent (albastru) */
    --accent-hover: #1d4ed8;        /* Hover accent */
    --text-primary: #1a1a1a;        /* Text principal */
    --text-secondary: #6b7280;      /* Text secundar */
}
```

## 📱 Responsive Breakpoints

- **Desktop**: > 1024px
- **Tablet**: 768px - 1024px
- **Mobile**: < 768px
- **Small Mobile**: < 480px

## 🔧 Personalizare Conținut

### Modificare Informații Contact:
Editează secțiunea `#contact` din `index.html`:
- Adresă
- Telefon
- Email
- Program

### Modificare Servicii:
Editează secțiunea `.services-grid` pentru a adăuga/modifica servicii.

### Modificare Echipă:
Editează secțiunea `.team-grid` pentru a adăuga membri echipei.

## 📊 SEO și Performance

- Meta tags optimizate pentru SEO
- Font loading optimizat (Google Fonts cu preconnect)
- Images lazy loading ready
- Semantic HTML5
- Accessibility friendly

## 🔄 Integrare Formular Contact

Formularul de contact are un handler placeholder. Pentru integrare reală:

1. **Backend API**: Conectează la API-ul tău în `script.js`:
```javascript
const response = await fetch('/api/contact', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(formData)
});
```

2. **Email Service**: Folosește servicii ca EmailJS, Formspree, sau SendGrid

3. **PHP Backend**: Creează un fișier `contact.php` pentru procesare server-side

## 📝 TODO - Viitoare Îmbunătățiri

- [ ] Adăugare imagini reale pentru toate secțiunile
- [ ] Integrare formular contact cu backend
- [ ] Adăugare Google Maps pentru locație
- [ ] Optimizare imagini (WebP, lazy loading)
- [ ] Adăugare Google Analytics
- [ ] Implementare funcționalitate înainte/după pentru imagini portofoliu
- [ ] Adăugare testimoniale clienți
- [ ] Secțiune FAQ
- [ ] Chatbot pentru întrebări rapide

## 🛠️ Tehnologii Folosite

- HTML5
- CSS3 (Custom Properties, Flexbox, Grid)
- JavaScript (ES6+)
- Google Fonts (Inter)
- SVG Icons

## 📄 Licență și Drepturi

© 2026 Salinas Construct SRL. Toate drepturile rezervate.

## 📞 Suport

Pentru întrebări sau suport tehnic:
- Email: office@salinasconstruct.ro
- Telefon: +40 721 234 567 