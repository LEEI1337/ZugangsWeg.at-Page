# GitHub Pages - Schnell-Anleitung

**Die Website ist fertig! Jetzt live stellen in 5 Minuten.**

---

## Schritt 1: GitHub Repository erstellen (2 Min)

1. Gehe zu https://github.com/LEEI1337
2. Klicke **"New Repository"** (grüner Button oben rechts)
3. Einstellungen:
   - **Repository name:** `ZugangsWeg.at-Page`
   - **Public** (wichtig für GitHub Pages!)
   - **KEIN** README hinzufügen (haben wir schon)
   - **KEINE** .gitignore
   - **KEINE** Lizenz
4. Klicke **"Create repository"**

---

## Schritt 2: Code zu GitHub pushen (1 Min)

**Öffne CMD/Terminal** und führe aus:

```bash
cd C:\Users\Thomas\Desktop\ZugangsWeg.at-Page

git remote add origin https://github.com/LEEI1337/ZugangsWeg.at-Page.git
git branch -M main
git push -u origin main
```

**Falls GitHub nach Login fragt:**
- Username: `LEEI1337`
- Password: Dein **Personal Access Token** (nicht dein normales Passwort!)

**Kein Token?** Erstelle einen hier:
https://github.com/settings/tokens
- Klicke "Generate new token (classic)"
- Name: "ZugangsWeg.at"
- Expire: 90 days
- Scopes: ✅ `repo` (alle Häkchen)
- Generate → Token kopieren (nur 1x sichtbar!)

---

## Schritt 3: GitHub Pages aktivieren (1 Min)

1. Gehe zu https://github.com/LEEI1337/ZugangsWeg.at-Page
2. Klicke **Settings** (oben rechts)
3. Im linken Menü: **Pages**
4. Unter "Build and deployment":
   - **Source:** Deploy from a branch
   - **Branch:** `main` (aus Dropdown)
   - **Folder:** `/ (root)` (aus Dropdown)
   - Klicke **Save**

---

## Schritt 4: Warten & Testen (1-2 Min)

**GitHub baut deine Seite jetzt automatisch!**

1. Warte 1-2 Minuten
2. Reload die Settings-Seite
3. Oben siehst du: **"Your site is live at https://leei1337.github.io/ZugangsWeg.at-Page/"**
4. Klicke drauf → **FERTIG!** 🎉

---

## Deine Live-URL:

```
https://leei1337.github.io/ZugangsWeg.at-Page/
```

---

## Wichtige Checks nach dem Launch:

### 1. Funktioniert alles?
- ✅ CSS wird geladen? (Seite ist gestylt, nicht nur Text)
- ✅ Cover-Bild wird angezeigt?
- ✅ Links zu Impressum/Datenschutz funktionieren?
- ✅ Österreich-Flagge + Herz neben Logo?
- ✅ Navigation funktioniert? (klick auf "Vision", "Status", etc.)

### 2. Mobile testen:
- Öffne die Seite am Handy
- Oder: Browser → F12 → Device Toolbar (Ctrl+Shift+M)
- Teste: iPhone SE, iPad, Desktop

### 3. Newsletter-Formular:
- Klicke "Jetzt Buch downloaden"
- Öffnet sich dein E-Mail-Client?
- Falls nicht: Das ist normal (mailto: funktioniert nur wenn E-Mail-Client konfiguriert ist)
- Alternative: User können direkt an lena@zugangsweg.at schreiben

---

## Zukünftige Updates machen:

Wenn du die Seite änderst:

```bash
cd C:\Users\Thomas\Desktop\ZugangsWeg.at-Page

# Änderungen speichern
git add .
git commit -m "Beschreibung der Änderungen"
git push

# Warte 1-2 Min → Live!
```

---

## Eigene Domain verbinden (später)

**Wenn du `zugangsweg.at` kaufst:**

1. Bei deinem Domain-Anbieter (z.B. World4You, Namecheap):
   ```
   Type: CNAME
   Name: www
   Value: leei1337.github.io
   ```

2. GitHub Settings → Pages → Custom Domain:
   - Gib ein: `www.zugangsweg.at`
   - ✅ Enforce HTTPS
   - Save

3. Warte 24h → fertig!

---

## Troubleshooting

### Problem: 404 Not Found
**Lösung:** Warte 2-5 Minuten nach dem Push, dann reload.

### Problem: Kein CSS (nur ungestylter Text)
**Lösung 1:** Hard Reload (Ctrl+F5)
**Lösung 2:** Prüfe `index.html` Zeile 8:
```html
<link rel="stylesheet" href="css/style.css">
```
(NICHT `/css/style.css` - kein Slash am Anfang!)

### Problem: Cover-Bild wird nicht angezeigt
**Lösung:** Prüfe ob `images/cover.png` existiert:
```bash
ls images/
```

### Problem: mailto: funktioniert nicht
**Das ist NORMAL!** Nicht jeder hat einen E-Mail-Client konfiguriert.
**Lösung:** User schreiben direkt an lena@zugangsweg.at

---

## Stats & Analytics (OHNE Tracking!)

**GitHub bietet Traffic-Stats (privacy-friendly):**

1. GitHub Repo → Insights → Traffic
2. Siehst du:
   - Unique Visitors (letzte 14 Tage)
   - Page Views
   - Referring Sites

**KEIN Google Analytics nötig!** ✅

---

## Was du JETZT hast:

✅ **Moderne Landing Page** (2025-Design)
✅ **HackerOne Erklärung** ("Bugs = Gesellschaftliche Probleme")
✅ **Buch-Download prominent** (alle 4 Bücher erklärt)
✅ **Newsletter-Formular** (E-Mail-Eingabe)
✅ **Österreich-Herz** (🇦🇹 ❤️ Made with ❤️ in Austria)
✅ **Responsive** (funktioniert auf allen Geräten)
✅ **Barrierefrei** (WCAG 2.1 AA)
✅ **Kein Tracking** (Signal-Prinzipien)
✅ **Impressum & Datenschutz** (DSGVO-konform)

---

## Nächste Schritte (nach Launch):

### Heute:
1. ✅ Live stellen (diese Anleitung)
2. ✅ Testen (alle Links, Mobile, etc.)
3. ✅ Freunden/Familie zeigen

### Diese Woche:
1. HTML validieren: https://validator.w3.org/
2. CSS validieren: https://jigsaw.w3.org/css-validator/
3. Accessibility Check: https://wave.webaim.org/
4. Kleine Fixes committen + pushen

### Diesen Monat:
1. Feedback sammeln
2. Typos korrigieren
3. Optional: Bilder/Icons hinzufügen
4. Optional: Eigene Domain verbinden

---

## Support

**Fragen? Probleme?**

1. Lies `DEPLOYMENT.md` (detaillierte Anleitung)
2. Lies `README.md` (technische Doku)
3. GitHub Issues: https://github.com/LEEI1337/ZugangsWeg.at-Page/issues

---

## 🎉 Das war's!

**In 5 Minuten hast du:**
- ✅ Eine professionelle Landing Page
- ✅ Auf GitHub Pages (kostenlos!)
- ✅ Mit eigener URL
- ✅ Bereit für tausende Besucher

**Viel Erfolg mit ZugangsWeg.at!** 🚀🇦🇹❤️

---

**Weil wir es verdient haben.**

Lena Kulnig
Eisenstadt, November 2025
