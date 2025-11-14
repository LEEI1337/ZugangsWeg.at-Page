# ZugangsWeg.at - Landing Page

**Status:** ALPHA
**Version:** 0.1.0
**Letzte Aktualisierung:** November 2025

---

## 🎯 Was ist das?

Dies ist die **Landing Page** für **ZugangsWeg.at** - ein Projekt, das Menschen, KMUs und vergessene Stimmen zusammenbringt, um gemeinsam Lösungen für gesellschaftliche Probleme zu entwickeln.

**Nicht die Politik. Nicht der Staat. Nicht die Großkonzerne.**
Sondern **WIR**: Die Menschen, die KMUs, die Kinder, die Alten, die Vergessenen, die Aktivisten.

**Weil wir es verdient haben.**

---

## 📂 Repository-Struktur

```
ZugangsWeg.at-Page/
├── index.html              # Hauptseite (Hero, Vision, Status, Kontakt)
├── impressum.html          # Impressum (§5 TMG / §25 MedienG)
├── datenschutz.html        # Datenschutzerklärung (DSGVO-konform)
├── css/
│   └── style.css           # Komplettes Styling (WCAG 2.1 AA)
├── js/                     # (Leer - derzeit kein JavaScript nötig)
├── images/                 # (Leer - Platzhalter für zukünftige Assets)
├── README.md               # Diese Datei
└── CLAUDE.md               # AI-Tonfall-Guidelines für dieses Projekt
```

---

## 🚀 Technologie-Stack

**Absichtlich einfach gehalten:**

- **HTML5** - Semantisch, barrierefrei
- **CSS3** - Keine Frameworks, pure CSS
- **Kein JavaScript** - Funktioniert ohne JS (Progressive Enhancement)
- **GitHub Pages** - Kostenlos, schnell, zuverlässig
- **Kein Tracking** - Keine Cookies, kein Analytics, kein Marketing

**Warum so simpel?**

- ✅ Schnell zu laden (auch auf langsamen Verbindungen)
- ✅ Funktioniert überall (alte Browser, Screen Reader, Textbrowser)
- ✅ Leicht zu pflegen (jeder kann HTML/CSS lernen)
- ✅ Transparent (jeder kann den Code lesen)
- ✅ Datenschutz-freundlich (nichts zu verstecken)

---

## 🎨 Design-Prinzipien

### 1. Accessibility First (WCAG 2.1 AA)

- ✅ Semantisches HTML (heading hierarchy, landmarks)
- ✅ Keyboard-Navigation (skip-links, focus states)
- ✅ Screen Reader Support (ARIA labels wo nötig)
- ✅ Farbkontrast (mindestens 4.5:1 für Text)
- ✅ Responsive Design (320px → 1920px)
- ✅ Kein Auto-Play, keine Animationen ohne `prefers-reduced-motion`

### 2. Deutsche Typografie-Standards

- **Max. 30em Zeilenlänge** (~50-60 Zeichen) für optimale Lesbarkeit
- **Line-Height 1.6** für Fließtext
- **Georgia/Times New Roman** (Serif) für Fließtext
- **System Sans-Serif** für Überschriften
- **Linksbündig** (NICHT Blocksatz, um Lücken zu vermeiden)

### 3. Mobile-First

- Basis-Design für 320px (iPhone SE)
- Breakpoints: 768px (Tablet), 1024px (Desktop)
- Touch-Targets mindestens 44x44px
- Kein horizontales Scrollen

---

## 🎨 Farb-Schema (EUKRATIE Theme)

```css
/* Primary - Blau (Vertrauen, Stabilität) */
--color-primary: #2980b9
--color-primary-dark: #1e6a99
--color-primary-light: #3498db

/* Secondary - Grün (Hoffnung, Wachstum) */
--color-secondary: #27ae60
--color-secondary-dark: #1e8449
--color-secondary-light: #2ecc71

/* Alert - Orange (ALPHA Phase) */
--color-alpha: #e67e22

/* Neutral */
--color-dark: #1a252f
--color-text: #2c3e50
--color-background: #ffffff
--color-background-alt: #ecf0f1
```

---

## 📝 Content-Strategie

### Kernbotschaften (auf JEDER Seite):

1. **"Weil wir es verdient haben"** - Prominente Platzierung
2. **ALPHA-Status** - Ehrlich kommunizieren: 0 Menschen geholfen (noch)
3. **Hoffnung** - Nicht Versprechungen, sondern Möglichkeiten zeigen
4. **Gemeinschaft** - "WIR bauen das" (nicht "ICH baue das")
5. **Transparenz** - Was existiert, was fehlt (ehrlich)

### Tonfall:

- ✅ Hoffnungsvoll, aber nicht naiv
- ✅ Ehrlich, aber nicht zynisch
- ✅ Inklusiv, aber nicht herablassend
- ✅ Technisch präzise, aber verständlich

---

## 🛠️ Lokales Setup

### Voraussetzungen:

- Git
- Einen modernen Browser
- (Optional) Einen lokalen Webserver (z.B. `http-server`)

### Schritte:

1. **Repository klonen:**
   ```bash
   git clone https://github.com/LEEI1337/ZugangsWeg.at-Page.git
   cd ZugangsWeg.at-Page
   ```

2. **Lokal testen:**

   **Option A - Einfach (Datei öffnen):**
   ```bash
   # Öffne index.html direkt im Browser
   # (Funktioniert, aber relative Links könnten Probleme machen)
   ```

   **Option B - Mit lokalem Server (empfohlen):**
   ```bash
   # Node.js http-server installieren (einmalig)
   npm install -g http-server

   # Server starten
   http-server -p 8000

   # Browser öffnen: http://localhost:8000
   ```

   **Option C - Python (wenn vorhanden):**
   ```bash
   # Python 3
   python -m http.server 8000

   # Browser öffnen: http://localhost:8000
   ```

3. **Änderungen machen:**
   - HTML/CSS bearbeiten
   - Browser neu laden (F5)
   - Wiederholen

---

## 🚀 Deployment (GitHub Pages)

### Erstmalig aktivieren:

1. Gehe zu **GitHub Repository → Settings → Pages**
2. **Source:** Deploy from a branch
3. **Branch:** `main` (oder `master`)
4. **Folder:** `/` (root)
5. **Save**

GitHub baut die Seite automatisch und stellt sie bereit unter:
`https://LEEI1337.github.io/ZugangsWeg.at-Page/`

### Bei jedem Push:

```bash
git add .
git commit -m "Beschreibung der Änderungen"
git push origin main
```

GitHub Pages aktualisiert automatisch (dauert 1-2 Minuten).

---

## ✅ Pre-Deployment Checklist

Bevor du pushst, prüfe:

- [ ] **HTML-Validierung:** https://validator.w3.org/
- [ ] **CSS-Validierung:** https://jigsaw.w3.org/css-validator/
- [ ] **Accessibility Check:** https://wave.webaim.org/
- [ ] **Mobile-Test:** Browser DevTools (320px, 768px, 1024px)
- [ ] **Keyboard-Navigation:** Alle Links/Buttons mit Tab erreichbar?
- [ ] **Screen Reader Test:** (z.B. NVDA auf Windows, VoiceOver auf Mac)
- [ ] **Farbkontrast:** https://webaim.org/resources/contrastchecker/
- [ ] **Rechtschreibung:** Deutsch-Korrektur durchlaufen lassen
- [ ] **Links funktionieren:** Alle internen/externen Links testen

---

## 🧪 Testing

### Browser-Kompatibilität:

Getestet mit:
- ✅ Chrome/Edge (Chromium) - neueste Version
- ✅ Firefox - neueste Version
- ✅ Safari (macOS/iOS) - neueste Version
- ✅ Legacy-Browser (IE11 wird NICHT unterstützt)

### Device-Tests:

- ✅ iPhone SE (320px)
- ✅ iPhone 12/13/14 (390px)
- ✅ iPad (768px)
- ✅ Desktop (1024px+)

### Accessibility-Tests:

- ✅ NVDA Screen Reader (Windows)
- ✅ VoiceOver (macOS/iOS)
- ✅ Keyboard-Navigation
- ✅ High Contrast Mode
- ✅ Reduced Motion

---

## 🤝 Beitragen

**Aktuell (ALPHA-Phase):**

Diese Landing Page ist bewusst **sehr simpel** gehalten. Wenn du helfen möchtest:

1. **Fehler melden:** GitHub Issues verwenden
2. **Verbesserungen vorschlagen:** Pull Request mit klarer Beschreibung
3. **Accessibility-Probleme:** Haben höchste Priorität!

**Wichtig:**
- ✅ Halte die Seite **einfach** (kein jQuery, kein React, kein Tailwind)
- ✅ **WCAG 2.1 AA** ist Minimum (nicht verhandelbar)
- ✅ **Mobile-First** denken
- ✅ **Keine Tracking-Tools** hinzufügen (niemals!)

### Code-Style:

**HTML:**
- 4 Spaces Einrückung
- Semantische Tags (`<header>`, `<main>`, `<section>`, `<footer>`)
- ARIA nur wo nötig (nicht überall!)

**CSS:**
- BEM-ähnliche Namenskonvention (`.hero-manifesto`, `.contact-role`)
- Mobile-First Media Queries
- CSS Custom Properties (`:root` Variablen)

---

## 📄 Lizenz

**Noch zu klären.**

Vorläufig: Alle Rechte vorbehalten (Lena Kulnig, 2025).

Open-Source-Lizenz folgt (wahrscheinlich MIT oder CC BY-SA 4.0).

---

## 📧 Kontakt

**Projektleitung:**
Lena Kulnig
E-Mail: lena@zugangsweg.at

**GitHub Issues:**
https://github.com/LEEI1337/ZugangsWeg.at-Page/issues

---

## 🔗 Weiterführende Links

- **Hauptprojekt (privat):** https://github.com/LEEI1337/ZugangsWeg.at
- **Buch "Digitale Dysbalance: Von Kleben zu Bauen"** (Band 4) - Erscheint 2026
- **WCAG 2.1 Guidelines:** https://www.w3.org/WAI/WCAG21/quickref/
- **GitHub Pages Docs:** https://docs.github.com/en/pages

---

## 📊 Projekt-Status

**Was EXISTIERT (November 2025):**
- ✅ Dieses Landing Page Repository
- ✅ Konzept (vollständig dokumentiert in Buch 4)
- ✅ Technischer Prototyp (Webseitenscanner)
- ✅ Testseite (basic)

**Was FEHLT (noch ~95%):**
- ❌ Nutzerkonten / Authentifizierung
- ❌ Projekt-Einreichungs-System
- ❌ Bounty-System (Impact-Belohnungen)
- ❌ Community-Features
- ❌ Mobile App
- ❌ API
- ❌ Beta-Tester
- ❌ Budget (€0)
- ❌ **Menschen geholfen (0 - noch!)**

**Wann BETA?**
Wenn der erste Mensch durch ZugangsWeg.at **echte Hilfe** bekommt.

**Wann STABLE?**
Wenn 100+ Projekte laufen und tausende Menschen mitmachen.

---

## 💚 Warum das alles?

**Weil Georg im Trainingsmodus seiner Smartwatch feststeckt.**
**Weil Sarah nicht mehr kleben, sondern bauen will.**
**Weil Maria Angst vor Inkasso-Briefen hat.**

**Weil wir alle ein System verdient haben, das für uns da ist.**
**Nicht gegen uns.**

**Weil wir es verdient haben.**

---

**Los geht's. JETZT.**

Lena Kulnig
Eisenstadt, November 2025
