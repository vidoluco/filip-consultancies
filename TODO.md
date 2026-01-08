# TODO - Salinas Construct Website

## 🎯 Taskuri Prioritare

### 📸 Imagini Reale
- [ ] **Portofoliu - Imagini Înainte/După**
  - Înlocuiește SVG-urile mock cu fotografii reale ale proiectelor
  - Pentru fiecare proiect, adaugă câte 2 imagini: înainte și după
  - Optimizează imaginile pentru web (WebP format recomandat)
  - Locație: [index.html:173-211](index.html#L173-L211) și următoarele `.portfolio-item`

- [ ] **Servicii - Imagini pentru Modale**
  - Adaugă 3 imagini pentru fiecare serviciu în modale
  - Imagini cu lucrări în progres și finalizate
  - Locație: [script.js:570-601](script.js#L570-L601) - înlocuiește placeholder-urile

- [ ] **Echipă - Fotografii Membrii**
  - Adaugă fotografii profesionale pentru fiecare membru al echipei
  - Format: portret, fundal neutru
  - Locație: [index.html](index.html) - secțiunea `.team-member`

- [ ] **Blog - Imagini Articole**
  - Adaugă imagini reprezentative pentru fiecare articol
  - Dimensiune recomandată: 800x600px
  - Locație: [index.html](index.html) - secțiunea `.blog-card`

- [ ] **Despre Noi - Fotografie Echipă/Birou**
  - Adaugă o fotografie de grup sau a biroului
  - Locație: [index.html](index.html) - `.about-image`

### 🎨 Design și Funcționalități

- [ ] **Before/After Slider Interactiv**
  - Implementează slider funcțional pentru imagini înainte/după în portofoliu
  - Folosește librărie precum twentytwenty sau creează funcționalitate custom
  - Referință: butoanele "Înainte / După" din portofoliu

- [ ] **Logo Personalizat**
  - Creează un logo personalizat pentru Salinas Construct
  - Înlocuiește SVG-ul geometric cu logo-ul real
  - Locație: [index.html:18-22](index.html#L18-L22)

- [ ] **Favicon**
  - Creează și adaugă favicon pentru site
  - Generează în multiple dimensiuni (16x16, 32x32, 180x180 pentru Apple)
  - Adaugă în `<head>` tag-uri pentru favicon

### 📝 Conținut

- [ ] **Informații Companie**
  - Actualizează adresa, telefon, email cu datele reale
  - Locație: [index.html](index.html) - secțiunea `#contact`
  - CUI și J verifică dacă sunt corecte în footer

- [ ] **Membrii Echipă**
  - Actualizează numele și rolurile membrilor echipei
  - Adaugă mai multe detalii dacă e necesar
  - Locație: [index.html](index.html) - `.team-member`

- [ ] **Articole Blog**
  - Scrie articole reale sau înlocuiește placeholder-urile
  - Creează pagini separate pentru fiecare articol
  - Link-urile "Citește mai mult" să ducă la articole complete

### 🔧 Funcționalități Backend

- [ ] **Formular Contact - Integrare Email**
  - Conectează formularul la un serviciu de email
  - Opțiuni: EmailJS, Formspree, SendGrid, sau PHP backend
  - Locație: [script.js:213-231](script.js#L213-L231)

- [ ] **Validare Formular Avansată**
  - Adaugă validare pentru număr de telefon românesc
  - Verifică format email
  - Mesaje de eroare în română/engleză

- [ ] **Newsletter Subscription**
  - Adaugă formular pentru newsletter în footer
  - Integrare cu Mailchimp sau alt serviciu

### 🌐 SEO și Performance

- [ ] **Meta Tags Optimizate**
  - Adaugă Open Graph tags pentru social media
  - Twitter Card tags
  - Schema.org markup pentru business

- [ ] **Optimizare Imagini**
  - Convertește toate imaginile în format WebP
  - Implementează lazy loading
  - Adaugă srcset pentru responsive images

- [ ] **Google Analytics**
  - Adaugă Google Analytics sau alt tool de analytics
  - Tracking pentru evenimente (click contact, download PDF, etc.)

- [ ] **Google Maps**
  - Adaugă hartă Google Maps în secțiunea contact
  - Marchează locația biroului

- [ ] **Sitemap și Robots.txt**
  - Generează sitemap.xml
  - Creează robots.txt

### 📱 Mobile și UX

- [ ] **Testare Cross-Browser**
  - Testează pe Chrome, Firefox, Safari, Edge
  - Verifică funcționalitățile pe fiecare browser

- [ ] **Testare Mobile**
  - Testează pe diferite dispozitive mobile
  - Verifică menu mobile, modale, formulare

- [ ] **Loading States**
  - Adaugă indicatori de loading pentru formular
  - Skeleton screens pentru imagini

- [ ] **Error States**
  - Mesaje de eroare friendly pentru formular
  - Pagină 404 customizată

### 🚀 Features Suplimentare (Opțional)

- [ ] **Testimoniale Clienți**
  - Adaugă secțiune cu recenzii de la clienți
  - Include rating cu stele

- [ ] **FAQ Section**
  - Secțiune cu întrebări frecvente
  - Accordion pentru a afișa/ascunde răspunsurile

- [ ] **Calculator Preț Estimativ**
  - Tool interactiv pentru estimare preț renovare
  - Bazat pe metrii pătrați și tipul lucrărilor

- [ ] **Galerie Foto Avansată**
  - Lightbox pentru imagini din portofoliu
  - Zoom și navigare între imagini

- [ ] **Video Tour**
  - Adaugă video prezentare în hero section
  - Sau video testimoniale de la clienți

- [ ] **Live Chat**
  - Integrează WhatsApp chat button
  - Sau alt serviciu de live chat

- [ ] **Multi-step Quote Form**
  - Formular în pași pentru solicitare ofertă
  - Cu selectare servicii, upload poze, detalii proiect

### 📄 Documentație și Legal

- [ ] **Pagină Termeni și Condiții**
  - Creează pagină separată pentru T&C

- [ ] **Pagină Politică Confidențialitate**
  - GDPR compliant
  - Explicație utilizare cookies

- [ ] **Cookie Consent Banner**
  - Implementează banner pentru acceptare cookies

### 🔐 Securitate

- [ ] **HTTPS**
  - Asigură-te că site-ul rulează pe HTTPS

- [ ] **Form Validation Backend**
  - Nu te baza doar pe validare client-side
  - Implementează validare pe server

- [ ] **Rate Limiting**
  - Protecție împotriva spam pe formular
  - reCAPTCHA sau hCaptcha

## 📊 Prioritizare

### Urgent (Săptămâna 1)
1. Imagini reale pentru portofoliu
2. Informații companie reale
3. Integrare formular contact
4. Logo personalizat

### Important (Săptămâna 2-3)
1. Imagini pentru servicii și echipă
2. Before/After slider
3. Google Maps
4. SEO optimization

### Nice to Have (Luna 1-2)
1. Toate features-urile suplimentare
2. Video content
3. Calculator preț
4. Testimoniale

---

## 📝 Note

- Toate placeholder-urile sunt marcate în cod cu comentarii
- Imaginile mock sunt SVG-uri care pot fi înlocuite ușor
- Structura și stilurile sunt gata - doar conținutul lipsește

## 🎨 Design Assets Necesare

### Dimensiuni Recomandate pentru Imagini:
- **Portfolio**: 800x600px (aspectratio 4:3)
- **Blog**: 800x600px
- **Team Photos**: 400x400px (pătrat)
- **Service Modal**: 600x400px
- **About Us**: 800x600px
- **Logo**: SVG (scalabil) sau PNG 200x200px minimum

### Format Imagini:
- **Principal**: WebP (pentru performance)
- **Fallback**: JPG (pentru compatibilitate)
- **Logo/Icons**: SVG (pentru claritate)

---

**Ultima actualizare**: 8 Ianuarie 2026
