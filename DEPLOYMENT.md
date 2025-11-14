# ZugangsWeg.at Landing Page - Deployment Guide

**Status:** READY FOR DEPLOYMENT
**Datum:** November 2025

---

## ✅ Was wurde erstellt?

### Dateien (komplett):

```
ZugangsWeg.at-Page/
├── index.html              # ✅ Hauptseite (546 Zeilen, komplett)
├── impressum.html          # ✅ Impressum (DSGVO-konform)
├── datenschutz.html        # ✅ Datenschutzerklärung (DSGVO-konform)
├── css/
│   └── style.css           # ✅ Komplettes Styling (1000+ Zeilen)
├── js/                     # (Leer - kein JS nötig)
├── images/                 # (Leer - bereit für Assets)
├── README.md               # ✅ Entwickler-Dokumentation
├── CLAUDE.md               # ✅ AI Tonalitäts-Guidelines
└── DEPLOYMENT.md           # ✅ Diese Datei
```

---

## 🎯 Kernbotschaften implementiert

### 1. "Weil wir es verdient haben" ✅
**Platzierung:**
- Hero Section (Manifesto Box, groß & fett)
- Contact Section (vor Kontaktformular)
- Datenschutz-Seite (am Ende, als philosophische Begründung)

### 2. ALPHA-Status ehrlich kommuniziert ✅
**Wo:**
- Hero Badge (orange, prominent)
- Status Section (große ALPHA Badge + ehrliche Auflistung)
- Footer (Version + Status)

**Botschaft:**
- ✅ "0 Menschen geholfen (noch!)"
- ✅ "~95% fehlt noch"
- ✅ "€0 Budget"
- ✅ "Winziges Team"

### 3. Hoffnung statt Versprechungen ✅
**Messaging:**
- ✅ "Wir versprechen nichts. Wir bieten Hoffnung."
- ✅ "Das ist was möglich IST, nicht was wir garantieren"
- ✅ BETA-Vision zeigt Potenzial, ohne zu übertreiben

### 4. Gemeinschaft statt Individualismus ✅
**Tonalität:**
- ✅ "UNSERE Plattform" (nicht "meine")
- ✅ "WIR bauen" (durchgehend)
- ✅ 6 verschiedene Rollen (jeder kann mitmachen)

---

## 🚀 GitHub Pages Deployment

### Schritt 1: Repository vorbereiten

**Stelle sicher, dass du im richtigen Verzeichnis bist:**

```bash
cd C:\Users\Thomas\Desktop\ZugangsWeg.at-Page
```

### Schritt 2: Git initialisieren (falls nicht schon geschehen)

```bash
# Git Repository initialisieren
git init

# Alle Dateien hinzufügen
git add .

# Ersten Commit erstellen
git commit -m "🚀 Initial commit - ZugangsWeg.at Landing Page

✅ index.html - Hero, Vision, Status, Contact Sections
✅ impressum.html - DSGVO-konform
✅ datenschutz.html - Signal-Prinzipien, Privacy by Design
✅ css/style.css - WCAG 2.1 AA, Mobile-First, Deutsche Typografie
✅ README.md - Entwickler-Dokumentation
✅ CLAUDE.md - AI Tonalitäts-Guidelines
✅ DEPLOYMENT.md - Deployment-Anleitung

Kernbotschaft: 'Weil wir es verdient haben' - prominent implementiert
Status: ALPHA (ehrlich kommuniziert)
Tonalität: Hoffnungsvoll, ehrlich, inklusiv

Generated with Claude Code (https://claude.com/claude-code)
Co-Authored-By: Claude <noreply@anthropic.com>"
```

### Schritt 3: Remote Repository verbinden

**Falls du das Repository neu erstellst auf GitHub:**

1. Gehe zu https://github.com/LEEI1337
2. Klicke auf "New Repository"
3. Name: `ZugangsWeg.at-Page`
4. Public (für GitHub Pages)
5. KEIN README hinzufügen (haben wir schon)
6. Create Repository

**Dann verbinden:**

```bash
git remote add origin https://github.com/LEEI1337/ZugangsWeg.at-Page.git
git branch -M main
git push -u origin main
```

**Falls das Repository bereits existiert:**

```bash
# Prüfe ob Remote schon verbunden ist
git remote -v

# Falls nicht, verbinde es
git remote add origin https://github.com/LEEI1337/ZugangsWeg.at-Page.git

# Push
git push -u origin main
```

### Schritt 4: GitHub Pages aktivieren

1. Gehe zu https://github.com/LEEI1337/ZugangsWeg.at-Page
2. Klicke auf **Settings** (oben rechts)
3. Im linken Menü: **Pages**
4. Unter "Source":
   - Branch: `main` auswählen
   - Folder: `/ (root)` auswählen
   - **Save** klicken
5. Warten (1-2 Minuten)
6. Seite neu laden - du siehst die URL:
   `https://leei1337.github.io/ZugangsWeg.at-Page/`

### Schritt 5: Testen

**Öffne im Browser:**
```
https://leei1337.github.io/ZugangsWeg.at-Page/
```

**Teste:**
- ✅ Seite lädt vollständig
- ✅ CSS wird geladen (nicht ungestylt)
- ✅ Links funktionieren (Impressum, Datenschutz, zurück)
- ✅ Kontaktformular zeigt E-Mail-Client (mailto:lena@zugangsweg.at)
- ✅ Responsive (öffne DevTools, teste 320px, 768px, 1024px)
- ✅ Accessibility (Keyboard-Navigation mit Tab-Taste)

---

## 🧪 Pre-Deployment Checklist

### HTML Validierung:

**Online:**
1. Gehe zu https://validator.w3.org/
2. Upload `index.html`, `impressum.html`, `datenschutz.html`
3. Behebe alle Fehler (Warnings sind okay)

**Lokal (falls nu-validator installiert):**
```bash
vnu index.html impressum.html datenschutz.html
```

### CSS Validierung:

**Online:**
1. Gehe zu https://jigsaw.w3.org/css-validator/
2. Upload `css/style.css`
3. Behebe alle Fehler

### Accessibility Check:

**Online:**
1. Gehe zu https://wave.webaim.org/
2. Gib URL ein: `https://leei1337.github.io/ZugangsWeg.at-Page/`
3. Prüfe Errors (sollten 0 sein)
4. Prüfe Contrast Errors (sollten 0 sein)

**Keyboard-Navigation:**
- [ ] Tab-Taste durchläuft alle interaktiven Elemente
- [ ] Skip-Link funktioniert (Tab → Enter springt zu Main)
- [ ] Focus-States sind sichtbar (blauer Outline)
- [ ] Enter aktiviert Links/Buttons

**Screen Reader (optional aber empfohlen):**
- Windows: NVDA (kostenlos)
- Mac: VoiceOver (eingebaut)

### Mobile Test:

**Browser DevTools:**
1. F12 → Device Toolbar (Ctrl+Shift+M)
2. Teste:
   - [ ] iPhone SE (375x667, 320px nach Zoom)
   - [ ] iPhone 12 Pro (390x844)
   - [ ] iPad (768x1024)
   - [ ] Desktop (1920x1080)

**Prüfe:**
- [ ] Kein horizontales Scrollen
- [ ] Text lesbar (nicht zu klein)
- [ ] Buttons groß genug (mindestens 44x44px Touch-Target)
- [ ] Bilder passen sich an

### Rechtschreibung:

**Deutsch-Korrektur:**
- [ ] index.html durchlesen
- [ ] impressum.html durchlesen
- [ ] datenschutz.html durchlesen
- [ ] README.md durchlesen

**Tools:**
- VS Code: Rechtschreibprüfung Extension (z.B. "German - Code Spell Checker")
- LanguageTool (https://languagetool.org/)

---

## 🔧 Troubleshooting

### Problem: Seite zeigt nur HTML, kein Styling

**Ursache:** CSS wird nicht geladen (Pfad falsch oder GitHub Pages noch nicht fertig)

**Lösung 1 - Pfad prüfen:**
```html
<!-- In index.html, sollte sein: -->
<link rel="stylesheet" href="css/style.css">
<!-- NICHT: -->
<link rel="stylesheet" href="/css/style.css"> <!-- Falscher absoluter Pfad -->
```

**Lösung 2 - GitHub Pages Wartezeit:**
- Warte 2-5 Minuten nach Aktivierung
- Seite neu laden (Ctrl+F5 für Hard Reload)

### Problem: 404 Not Found

**Ursache:** GitHub Pages noch nicht aktiviert oder Branch falsch

**Lösung:**
1. Settings → Pages
2. Prüfe: Branch = `main`, Folder = `/ (root)`
3. Warte 2 Minuten, reload

### Problem: Links zu Impressum/Datenschutz funktionieren nicht

**Ursache:** Relative Pfade könnten falsch sein

**Lösung:**
```html
<!-- Sollte sein: -->
<a href="impressum.html">Impressum</a>
<!-- NICHT: -->
<a href="/impressum.html">Impressum</a>
```

### Problem: mailto: funktioniert nicht

**Das ist NORMAL!**
- `mailto:lena@zugangsweg.at` öffnet E-Mail-Client
- Wenn kein E-Mail-Client konfiguriert → Browser zeigt Fehler
- User müssen E-Mail-Client installiert haben (Outlook, Thunderbird, etc.)

**Alternative (in Zukunft):**
- Kontaktformular mit Backend (PHP, Node.js)
- Aber ALPHA hat kein Backend → mailto: ist okay

---

## 📊 Performance Check (optional)

### Google Lighthouse:

1. Öffne DevTools (F12)
2. Tab "Lighthouse"
3. Select:
   - [x] Performance
   - [x] Accessibility
   - [x] Best Practices
   - [x] SEO
4. "Generate Report"

**Erwartete Werte:**
- **Performance:** 95-100 (statische Seite, kein JS)
- **Accessibility:** 95-100 (WCAG 2.1 AA konform)
- **Best Practices:** 90-100
- **SEO:** 90-100

### PageSpeed Insights:

https://pagespeed.web.dev/

**Gib URL ein:**
`https://leei1337.github.io/ZugangsWeg.at-Page/`

---

## 🔐 Security Check

### HTTPS:

GitHub Pages erzwingt automatisch HTTPS ✅

### CSP (Content Security Policy):

Derzeit keine CSP-Header (GitHub Pages Standard).

**In Zukunft (wenn Custom Domain):**
Füge `.htaccess` oder Cloudflare Page Rules hinzu für CSP.

### Keine Tracking-Tools:

✅ Kein Google Analytics
✅ Kein Facebook Pixel
✅ Keine Cookies (außer GitHub Pages technische)
✅ Kein JavaScript

**= Maximale Privacy ✅**

---

## 📝 Post-Deployment Aufgaben

### 1. Domain verbinden (optional, später)

**Wenn du `zugangsweg.at` hast:**

1. DNS-Einstellungen bei deinem Registrar:
   ```
   Type: CNAME
   Name: www
   Value: leei1337.github.io
   ```

2. GitHub Settings → Pages → Custom Domain:
   - `www.zugangsweg.at` eingeben
   - "Enforce HTTPS" aktivieren

**Anleitung:** https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

### 2. Google Search Console (optional)

**Wenn du in Google-Suche erscheinen willst:**

1. Gehe zu https://search.google.com/search-console/
2. Füge Property hinzu: `https://leei1337.github.io/ZugangsWeg.at-Page/`
3. Verify Ownership (HTML-Tag oder File Upload)
4. Sitemap einreichen (erstelle `sitemap.xml` - siehe unten)

### 3. Sitemap erstellen (optional)

**Erstelle `sitemap.xml`:**

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://leei1337.github.io/ZugangsWeg.at-Page/</loc>
    <lastmod>2025-11-14</lastmod>
    <priority>1.0</priority>
  </url>
  <url>
    <loc>https://leei1337.github.io/ZugangsWeg.at-Page/impressum.html</loc>
    <lastmod>2025-11-14</lastmod>
    <priority>0.5</priority>
  </url>
  <url>
    <loc>https://leei1337.github.io/ZugangsWeg.at-Page/datenschutz.html</loc>
    <lastmod>2025-11-14</lastmod>
    <priority>0.5</priority>
  </url>
</urlset>
```

**Dann:**
```bash
git add sitemap.xml
git commit -m "Add sitemap.xml for SEO"
git push
```

### 4. Social Media Meta Tags (optional)

**Füge in `<head>` von index.html hinzu:**

```html
<!-- Open Graph (Facebook, LinkedIn) -->
<meta property="og:title" content="ZugangsWeg.at - Wir bauen unser eigenes System">
<meta property="og:description" content="Nicht die Politik. Nicht der Staat. Nicht die Großkonzerne. Sondern WIR. Weil wir es verdient haben.">
<meta property="og:type" content="website">
<meta property="og:url" content="https://leei1337.github.io/ZugangsWeg.at-Page/">
<!-- <meta property="og:image" content="URL_TO_PREVIEW_IMAGE.jpg"> -->

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="ZugangsWeg.at - Wir bauen unser eigenes System">
<meta name="twitter:description" content="Nicht die Politik. Nicht der Staat. Nicht die Großkonzerne. Sondern WIR. Weil wir es verdient haben.">
<!-- <meta name="twitter:image" content="URL_TO_PREVIEW_IMAGE.jpg"> -->
```

---

## ✅ Final Quality Check

**Bevor du LIVE gehst, prüfe:**

1. **Botschaft klar?**
   - [ ] "Weil wir es verdient haben" sichtbar?
   - [ ] ALPHA-Status kommuniziert?
   - [ ] Hoffnung (nicht Versprechungen)?

2. **Ehrlichkeit?**
   - [ ] "0 Menschen geholfen (noch!)" steht da?
   - [ ] "€0 Budget" erwähnt?
   - [ ] "~95% fehlt noch" klar?

3. **Inklusivität?**
   - [ ] "WIR" statt "ICH"?
   - [ ] 6 Rollen (jeder kann mitmachen)?
   - [ ] Keine Fachbegriffe ohne Erklärung?

4. **Technisch solide?**
   - [ ] HTML validiert?
   - [ ] CSS validiert?
   - [ ] WCAG 2.1 AA erfüllt?
   - [ ] Mobile funktioniert (320px+)?
   - [ ] Kein Tracking?

**Wenn alle ✅ → DEPLOY!**

---

## 🎉 Nach dem Deployment

### Teile die URL:

```
https://leei1337.github.io/ZugangsWeg.at-Page/
```

**Wo teilen:**
- [ ] Buch 4 (als QR-Code oder Link)
- [ ] E-Mail-Signatur (lena@zugangsweg.at)
- [ ] Social Media (wenn du magst)
- [ ] PanLab Eisenstadt (Community zeigen)

### Monitor Analytics (OHNE Tracking):

**GitHub bietet Traffic-Stats (privacy-friendly):**
1. GitHub Repo → Insights → Traffic
2. Siehst du:
   - Unique Visitors (letzte 14 Tage)
   - Page Views
   - Referring Sites

**KEIN Google Analytics nötig!** ✅

---

## 📞 Support

**Bei Problemen:**

1. **GitHub Issues:** https://github.com/LEEI1337/ZugangsWeg.at-Page/issues
2. **E-Mail:** lena@zugangsweg.at
3. **GitHub Pages Docs:** https://docs.github.com/en/pages

---

## 🚀 Nächste Schritte (nach ALPHA)

**Wenn erste Menschen geholfen wurde → BETA:**

1. **Erweitere die Website:**
   - Projekt-Einreichungs-Formular (Backend nötig)
   - Blog/News-Section
   - Community-Seite (Contributors zeigen)

2. **Techstack erweitern:**
   - Backend: Node.js + PostgreSQL
   - Frontend: Bleibt HTML/CSS (später React?)
   - Authentication: Signal-Prinzipien (E2E, Privacy)

3. **Domain:**
   - Kaufe `zugangsweg.at`
   - Verbinde mit GitHub Pages (siehe oben)

**Aber JETZT: Erst mal ALPHA starten! ✅**

---

**Los geht's. JETZT.**

Lena Kulnig
Eisenstadt, November 2025
