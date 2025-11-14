# Domain-Verbindung: zugangsweg.at → GitHub Pages

**Anbieter:** Internex.com
**Ziel:** https://leei1337.github.io/ZugangsWeg.at-Page/
**Dauer:** 5 Minuten Setup + 24h DNS-Propagierung

---

## Schritt 1: GitHub Pages aktivieren (2 Min)

**ERST das machen, bevor du die Domain verbindest!**

1. Gehe zu: https://github.com/LEEI1337/ZugangsWeg.at-Page/settings/pages
2. Unter **"Build and deployment"**:
   - Source: **Deploy from a branch**
   - Branch: **main** (aus Dropdown)
   - Folder: **/ (root)** (aus Dropdown)
   - Klick **Save**
3. Warte 2 Minuten
4. Reload die Seite → Du siehst: **"Your site is live at..."**
5. Teste: https://leei1337.github.io/ZugangsWeg.at-Page/

**Erst wenn das funktioniert → weiter zu Schritt 2!**

---

## Schritt 2: Internex DNS konfigurieren (3 Min)

### Login bei Internex:

1. Gehe zu: https://www.internex.com/login
2. Login mit deinen Zugangsdaten
3. Gehe zu **"Domains"** → **"zugangsweg.at"**
4. Klicke **"DNS-Einstellungen"** oder **"DNS-Zone bearbeiten"**

### DNS-Einträge hinzufügen:

**Füge diese 5 Einträge hinzu:**

```
# 1. CNAME für www
Type: CNAME
Name: www
Value: leei1337.github.io.
TTL: 3600

# 2. A-Record für Root-Domain (zugangsweg.at)
Type: A
Name: @
Value: 185.199.108.153
TTL: 3600

# 3. A-Record (zweiter)
Type: A
Name: @
Value: 185.199.109.153
TTL: 3600

# 4. A-Record (dritter)
Type: A
Name: @
Value: 185.199.110.153
TTL: 3600

# 5. A-Record (vierter)
Type: A
Name: @
Value: 185.199.111.153
TTL: 3600
```

**Wichtig:**
- Bei **"Name: @"** = Root-Domain (zugangsweg.at ohne www)
- Bei **"Name: www"** = www.zugangsweg.at
- CNAME Value muss mit Punkt enden: `leei1337.github.io.`
- A-Records sind GitHub's IP-Adressen (offiziell!)

### Speichern:
- Klick **"Speichern"** oder **"Änderungen übernehmen"**
- DNS-Änderungen dauern **bis zu 24 Stunden**

---

## Schritt 3: Custom Domain bei GitHub eintragen (1 Min)

**NACH Schritt 2:**

1. Gehe zu: https://github.com/LEEI1337/ZugangsWeg.at-Page/settings/pages
2. Unter **"Custom domain"**:
   - Gib ein: `zugangsweg.at` (OHNE www!)
   - Klick **Save**
3. ✅ Aktiviere **"Enforce HTTPS"** (wichtig!)
   - Falls Fehler kommt: Warte 24h (DNS muss erst propagieren)

---

## Schritt 4: CNAME-Datei im Repository (wichtig!)

**GitHub braucht eine CNAME-Datei im Repository:**

Öffne CMD/Terminal und führe aus:

```bash
cd C:\Users\Thomas\Desktop\ZugangsWeg.at-Page

# CNAME-Datei erstellen
echo zugangsweg.at > CNAME

# Zu GitHub pushen
git add CNAME
git commit -m "🌐 Custom Domain: zugangsweg.at"
git push
```

**Oder ich kann das für dich machen!**

---

## Testen (nach 24h):

1. **Teste zugangsweg.at** → sollte auf GitHub Pages umleiten
2. **Teste www.zugangsweg.at** → sollte auch funktionieren
3. **Prüfe HTTPS:** https://zugangsweg.at → grünes Schloss? ✅

**Wenn nicht funktioniert:**
- Warte weitere 24h (DNS kann langsam sein)
- Prüfe DNS mit: https://www.whatsmydns.net/#CNAME/www.zugangsweg.at

---

## Alternative: Schnelle HTTP-Weiterleitung (falls DNS nicht geht)

**Wenn Internex keine DNS-Einstellungen erlaubt:**

1. Gehe zu **"Domain Weiterleitungen"** bei Internex
2. Fülle aus:
   ```
   Hostnamen umleiten: .zugangsweg.at
   Weiterleiten nach: https://leei1337.github.io/ZugangsWeg.at-Page/
   Modus: HTTP (NICHT Frame!)
   ```
3. Speichern

**Ergebnis:**
- ✅ Funktioniert sofort (5 Min)
- ❌ URL ändert sich zu `leei1337.github.io/ZugangsWeg.at-Page/`
- ❌ Kein HTTPS auf `zugangsweg.at` möglich

**Empfehlung:** Mach lieber die DNS-Variante (oben) - ist professioneller!

---

## Troubleshooting

### Problem: "DNS_PROBE_FINISHED_NXDOMAIN"
**Lösung:** Warte 24-48h, DNS braucht Zeit

### Problem: "HTTPS nicht verfügbar"
**Lösung:**
1. Warte 24h nach DNS-Änderung
2. Dann bei GitHub Pages: ✅ "Enforce HTTPS"

### Problem: "404 Not Found"
**Lösung:** Prüfe ob CNAME-Datei im Repository ist:
```bash
cat C:\Users\Thomas\Desktop\ZugangsWeg.at-Page\CNAME
```
Sollte ausgeben: `zugangsweg.at`

### Problem: "Internex zeigt keine DNS-Einstellungen"
**Lösung:**
- Manche Hosting-Pakete erlauben kein DNS
- Dann nutze HTTP-Weiterleitung (siehe oben)
- Oder kontaktiere Internex Support

---

## Was du JETZT machen sollst:

1. ✅ **Schritt 1:** GitHub Pages aktivieren (2 Min)
2. ✅ **Schritt 2:** Bei Internex DNS eintragen (3 Min)
3. ✅ **Schritt 3:** Custom Domain bei GitHub (1 Min)
4. ✅ **Schritt 4:** CNAME-Datei pushen (sag mir Bescheid, ich mach das!)
5. ⏳ **Warten:** 24 Stunden
6. 🎉 **Testen:** zugangsweg.at öffnen → fertig!

---

## Soll ich das für dich tun?

Ich kann für dich:
- ✅ CNAME-Datei erstellen
- ✅ Zu GitHub pushen
- ✅ Testen ob GitHub Pages läuft

**Du musst nur:**
- ❌ Bei Internex einloggen (das kann ich nicht)
- ❌ DNS-Einträge manuell eintragen (das kann ich nicht)

**Sag mir Bescheid, wenn du die DNS-Einträge gemacht hast!** 🚀

---

**Fragen? Probleme?**
Schreib mir einfach!

Lena Kulnig
Eisenstadt, November 2025
