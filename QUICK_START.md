# ZugangsWeg.at - Quick Start Guide

**Alles ist fertig! Hier ist was du JETZT tun musst:**

---

## 🚀 In 5 Minuten live gehen

### Schritt 1: Git Repository erstellen (2 Min)

Öffne Terminal/CMD und führe aus:

```bash
cd C:\Users\Thomas\Desktop\ZugangsWeg.at-Page

git init
git add .
git commit -m "🚀 Initial commit - ZugangsWeg.at Landing Page

✅ index.html - Komplett (Hero, Vision, Status, Contact)
✅ impressum.html + datenschutz.html - DSGVO-konform
✅ css/style.css - WCAG 2.1 AA, Mobile-First
✅ Dokumentation - README, CLAUDE, DEPLOYMENT
✅ Kernbotschaft prominent: Weil wir es verdient haben

Generated with Claude Code
Co-Authored-By: Claude <noreply@anthropic.com>"
```

### Schritt 2: Zu GitHub pushen (1 Min)

**Falls Repository NICHT existiert:**

1. Gehe zu https://github.com/LEEI1337
2. Klicke "New Repository"
3. Name: `ZugangsWeg.at-Page`
4. Public (für GitHub Pages)
5. KEIN README hinzufügen
6. Create

**Dann:**

```bash
git remote add origin https://github.com/LEEI1337/ZugangsWeg.at-Page.git
git branch -M main
git push -u origin main
```

**Falls Repository EXISTIERT:**

```bash
git remote add origin https://github.com/LEEI1337/ZugangsWeg.at-Page.git
git push -u origin main
```

### Schritt 3: GitHub Pages aktivieren (1 Min)

1. Gehe zu https://github.com/LEEI1337/ZugangsWeg.at-Page
2. Klicke **Settings** (oben rechts)
3. Linkes Menü: **Pages**
4. Source: Branch `main`, Folder `/` (root)
5. **Save**

### Schritt 4: Warten & Testen (1 Min)

**Warte 1-2 Minuten**, dann öffne:

```
https://leei1337.github.io/ZugangsWeg.at-Page/
```

**Prüfe:**
- ✅ Seite lädt (nicht 404)
- ✅ Styling funktioniert (nicht nur ungestyltes HTML)
- ✅ Links zu Impressum/Datenschutz gehen
- ✅ "Weil wir es verdient haben" ist sichtbar

**Wenn alles ✅ → FERTIG! 🎉**

---

## 📂 Was du hast

```
ZugangsWeg.at-Page/
├── index.html              # Hauptseite
├── impressum.html          # Impressum
├── datenschutz.html        # Datenschutz
├── css/style.css           # Komplettes Styling
├── README.md               # Entwickler-Doku
├── CLAUDE.md               # AI Tonalitäts-Guide
├── DEPLOYMENT.md           # Detaillierte Deploy-Anleitung
├── PROJECT_SUMMARY.md      # Projekt-Zusammenfassung
└── QUICK_START.md          # Diese Datei
```

---

## ✅ Kernbotschaften (alle drin!)

1. **"Weil wir es verdient haben"** - 3x prominent platziert
2. **ALPHA-Status** - Ehrlich: "0 Menschen geholfen (noch!)"
3. **Hoffnung** - Keine falschen Versprechungen
4. **Gemeinschaft** - "WIR bauen" (nicht "ICH")

---

## 🔧 Troubleshooting

### Problem: 404 Not Found

**Lösung:** Warte 2-5 Minuten, dann reload. GitHub Pages braucht Zeit.

### Problem: Kein Styling (nur HTML)

**Lösung 1:** Hard Reload (Ctrl+F5)
**Lösung 2:** Prüfe `index.html` Zeile 8:
```html
<link rel="stylesheet" href="css/style.css">
```
(NICHT `/css/style.css` - kein Slash am Anfang!)

### Problem: Links funktionieren nicht

**Lösung:** Relative Pfade prüfen (`impressum.html` NICHT `/impressum.html`)

---

## 📱 Nächste Schritte

### Heute:

1. ✅ Deployment testen
2. ✅ Familie/Freunde zeigen: "Schau mal, was denkst du?"
3. ✅ Typos suchen (frische Augen helfen)

### Diese Woche:

1. HTML validieren: https://validator.w3.org/
2. CSS validieren: https://jigsaw.w3.org/css-validator/
3. Accessibility Check: https://wave.webaim.org/
4. Kleine Fixes committen + pushen

### Diesen Monat:

1. Feedback umsetzen
2. Optional: Bilder/Icons hinzufügen
3. Optional: Eigene Domain verbinden (`zugangsweg.at`)

---

## 📞 Support

**Fragen? Probleme?**

1. Lies `DEPLOYMENT.md` (detaillierte Anleitung)
2. Lies `README.md` (technische Doku)
3. GitHub Issues: https://github.com/LEEI1337/ZugangsWeg.at-Page/issues

---

## 🎉 Das war's!

**In 5 Minuten hast du:**
- ✅ Eine professionelle Landing Page
- ✅ WCAG 2.1 AA konform
- ✅ Mobile-First Responsive
- ✅ Datenschutz-freundlich (kein Tracking!)
- ✅ Auf GitHub Pages (kostenlos!)

**Jetzt kannst du die Welt zeigen:**

> "Nicht die Politik. Nicht der Staat. Nicht die Großkonzerne.
> Sondern WIR.
> **Weil wir es verdient haben.**"

---

🚀 **Los geht's. JETZT.**

Lena Kulnig
Eisenstadt, November 2025
