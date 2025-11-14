# CLAUDE.md - ZugangsWeg.at Landing Page

**Dieses Dokument gibt Claude Code (und anderen AI-Tools) Kontext und Tonalitäts-Richtlinien für die Arbeit an diesem Projekt.**

---

## 🎯 Was ist ZugangsWeg.at?

**Kurz:** "HackerOne für Gesellschaft" - Menschen melden Probleme, entwickeln Lösungen, werden für Impact belohnt.

**Lang:**
ZugangsWeg.at ist eine Plattform, die Menschen, KMUs, Senioren, Kinder, Aktivisten und "die Vergessenen" zusammenbringt, um gemeinsam gesellschaftliche Probleme zu lösen.

**Nicht die Politik. Nicht der Staat. Nicht die Großkonzerne.**
Sondern **WIR**.

**Weil wir es verdient haben.**

---

## 📘 Projekt-Kontext

### Status (November 2025):
- **Phase:** ALPHA (bis zum ersten Menschen, dem wir helfen)
- **Team:** Winzig (Lena + wenige Contributors)
- **Budget:** €0
- **Menschen geholfen:** 0 (noch!)
- **Was existiert:** Konzept (Buch 4), Prototyp (Webseitenscanner), diese Landing Page
- **Was fehlt:** ~95% (Nutzerkonten, Bounty-System, Community-Features, etc.)

### Vision:
- **2027:** 50.000 Nutzer, 500 Contributors, ROI 89:1
- **2050:** 2 Milliarden Menschen in eukratischen Systemen

### Inspiration:
- **HackerOne:** Bug Bounties für Sicherheitslücken → ZugangsWeg.at: "Bounties" für gesellschaftliche Probleme
- **Signal:** Non-Profit, datenschutzfreundlich, transparent → ZugangsWeg.at folgt diesen Prinzipien
- **Wikipedia:** Community-moderiert, resistent gegen KI-Flut → ZugangsWeg.at will ähnliche Qualitätskontrolle

---

## ✍️ Tonalitäts-Richtlinien

**Wenn du Code, Content oder Dokumentation für dieses Projekt erstellst, halte dich an diese Prinzipien:**

### 1. Hoffnungsvoll, aber nicht naiv

✅ **RICHTIG:**
> "ZugangsWeg.at ist derzeit in der ALPHA-Phase. Wir haben noch 0 Menschen geholfen - aber wir glauben, dass es möglich ist. Wenn wir zusammenarbeiten."

❌ **FALSCH:**
> "ZugangsWeg.at wird die Welt verändern! Bald helfen wir Millionen!"

**Warum?**
Wir bieten **Hoffnung**, keine **Versprechungen**. Wir zeigen, was **möglich IST**, nicht was wir **garantieren**.

---

### 2. Ehrlich, aber nicht zynisch

✅ **RICHTIG:**
> "Wir haben noch fast nichts - außer einem Konzept, einem Prototyp und viel Arbeit vor uns. Aber das ist okay. Große Dinge fangen klein an."

❌ **FALSCH:**
> "Das System ist kaputt, alles ist hoffnungslos, wir haben keine Chance."

**Warum?**
Ehrlichkeit über den Status schafft Vertrauen. Zynismus lähmt. Wir sind realistisch, aber nicht defätistisch.

---

### 3. Inklusiv, aber nicht herablassend

✅ **RICHTIG:**
> "Egal ob du Entwickler bist, Oma mit Smartphone-Fragen, Aktivist ohne Plattform oder einfach nur frustriert vom System - du bist hier richtig."

❌ **FALSCH:**
> "Auch Nicht-Techniker können mitmachen! Wir erklären alles ganz einfach für euch."

**Warum?**
Wir sprechen **MIT** Menschen, nicht **ÜBER** sie. Wir erklären, ohne zu infantilisieren.

---

### 4. Technisch präzise, aber verständlich

✅ **RICHTIG:**
> "Diese Website ist eine statische GitHub Pages Seite - kein Tracking, keine Cookies, kein JavaScript. Sie funktioniert auf alten Browsern und Screen Readern."

❌ **FALSCH:**
> "Wir nutzen moderne JAMstack-Architektur mit Server-Side Rendering und Edge Functions für optimale Performance."

**Warum?**
Technische Präzision ist wichtig, aber Fachjargon ohne Kontext schließt Menschen aus.

---

### 5. Gemeinschaftlich, nicht individualistisch

✅ **RICHTIG:**
> "ZugangsWeg.at ist nicht MEINE Plattform. Es ist UNSERE. Ich gebe nur den Startschuss."

❌ **FALSCH:**
> "Ich habe ZugangsWeg.at entwickelt, um der Welt zu zeigen, wie man es richtig macht."

**Warum?**
Das Projekt funktioniert nur, wenn **viele** mitmachen. Es ist keine One-Woman-Show.

---

## 🚨 Die Kernbotschaft (IMMER präsent)

### "Weil wir es verdient haben"

**Diese Phrase MUSS auf jeder Seite prominent sein.**

**Kontext:**
- Nach langer Erklärung → "Weil wir es verdient haben."
- Nach Statusbeschreibung → "Und wir bauen es. Weil wir es verdient haben."
- Am Ende von Aufrufen → "Bau mit uns. Weil wir es verdient haben."

**Warum wichtig?**
Es fasst die gesamte Philosophie zusammen: **Wir sollten nicht um gute Systeme betteln müssen. Sie sind unser Recht.**

---

## 📝 Sprach-Regeln

### Deutsch:
- **Standard:** Hochdeutsch (keine starken Dialekte im Fließtext)
- **Du/Sie:** Durchgehend "du" (inklusiver, persönlicher)
- **Gendern:** Neutral formulieren wo möglich ("Entwickler" → "Menschen die entwickeln"), sonst Doppelform ("Nutzer und Nutzerinnen"), KEIN Gendern mit Sternchen/Doppelpunkt in diesem Projekt

### Englisch:
- Nur wo nötig (technische Begriffe: "Bug Bounty", "Open Source")
- Immer erklären beim ersten Vorkommen

### Beispiele:

✅ **RICHTIG:**
> "ZugangsWeg.at funktioniert wie HackerOne (eine Bug-Bounty-Plattform für Sicherheitslücken) - aber für gesellschaftliche Probleme."

❌ **FALSCH:**
> "ZugangsWeg.at ist basically ein crowdsourced impact-driven bounty system."

---

## 🎨 Design-Philosophie

Wenn du Code für diese Website schreibst:

### HTML:
- ✅ Semantisch (`<header>`, `<main>`, `<section>`, `<footer>`)
- ✅ WCAG 2.1 AA (mindestens!)
- ✅ Keyboard-Navigation
- ✅ Screen Reader friendly

### CSS:
- ✅ Mobile-First
- ✅ Keine Frameworks (kein Bootstrap, kein Tailwind)
- ✅ Deutsche Typografie-Standards (max. 30em Zeilenlänge)
- ✅ Linksbündig (KEIN Blocksatz)

### JavaScript:
- ✅ Progressive Enhancement (Seite funktioniert OHNE JS)
- ✅ Kein jQuery, kein React (zu komplex für Landing Page)

### Tracking:
- ❌ **ABSOLUT KEIN TRACKING!**
- ❌ Kein Google Analytics
- ❌ Kein Facebook Pixel
- ❌ Keine Cookies (außer technisch notwendige)

**Warum?**
Datenschutz ist ein **Menschenrecht**, kein Geschäftsmodell. Wir machen es wie Signal.

---

## 🚫 Was NIEMALS tun

### 1. Tracking hinzufügen
❌ "Ich füge Google Analytics hinzu, um die Nutzung zu tracken."
→ **NIEMALS!** Datenschutz ist nicht verhandelbar.

### 2. Komplexität ohne Grund
❌ "Ich baue das mit React um, dann ist es moderner."
→ **NEIN!** Einfachheit ist ein Feature, keine Schwäche.

### 3. False Promises
❌ "ZugangsWeg.at hat bereits 10.000 Nutzer geholfen!"
→ **LÜGE NICHT!** Ehrlichkeit ist alles.

### 4. Exkludierende Sprache
❌ "Für fortgeschrittene User bieten wir..."
→ **NEIN!** Entweder für alle verständlich oder Kontext erklären.

### 5. Individualisierung
❌ "Lena Kulnig's bahnbrechendes Projekt..."
→ **NEIN!** "Unser Projekt", "Wir bauen", nicht "Ich".

---

## ✅ Checkliste für neue Inhalte

Bevor du Content oder Code committest, frage:

1. **Ehrlichkeit:** Ist der ALPHA-Status klar kommuniziert? (0 Menschen geholfen - noch!)
2. **Hoffnung:** Zeige ich Möglichkeiten, nicht Garantien?
3. **Kernbotschaft:** Ist "Weil wir es verdient haben" sichtbar?
4. **Inklusivität:** Können das alle verstehen (Oma, 15-Jähriger, Nicht-Techniker)?
5. **Accessibility:** Funktioniert es mit Keyboard + Screen Reader?
6. **Datenschutz:** Kein Tracking, keine unnötigen Cookies?
7. **Mobile:** Funktioniert es auf einem iPhone SE (320px)?
8. **Gemeinschaft:** Sage ich "WIR" statt "ICH"?

**Wenn alle 8 Fragen "JA" → GOOD!**
**Wenn eine "NEIN" → FIX IT!**

---

## 📚 Kontext-Quellen

Wenn du mehr Kontext brauchst:

### 1. Buch "Digitale Dysbalance: Von Kleben zu Bauen" (Band 4)
**Speziell relevant:**
- **TEIL VIII:** ZugangsWeg.at Konzept (50 Seiten)
- **TEIL VII:** Der Plan (4 Stufen der Teilnahme)
- **TEIL V:** EUKRATIE-Konzept (die "gute Gegenwart")
- **Vorwort:** Warum dieses Buch? (Georg, Sarah, Maria)

### 2. Inspirierende Projekte:
- **Signal:** Non-Profit Messenger (https://signal.org)
- **HackerOne:** Bug Bounty Platform (https://hackerone.com)
- **Wikipedia:** Community-moderiert (https://wikipedia.org)

### 3. Diese Repository:
- **README.md:** Technische Dokumentation
- **index.html:** Kernbotschaften und Struktur
- **datenschutz.html:** Datenschutz-Philosophie

---

## 🎭 Personas (Wen wir ansprechen)

### 1. Georg (56, Fliesenleger)
- **Problem:** Smartwatch vom Arzt verordnet, steckt im Trainingsmodus fest
- **Braucht:** Einfache Hilfe, ohne IT-Studium
- **Tonfall für Georg:** Verständnisvoll, geduldig, keine Fachbegriffe ohne Erklärung

### 2. Sarah (19, Ex-Klimaaktivistin)
- **Problem:** Wollte kleben, hat gesehen dass es nichts bringt, sucht andere Wege
- **Braucht:** Sinnvolle Aktion, Impact sehen
- **Tonfall für Sarah:** Hoffnungsvoll, konkret, nicht zynisch

### 3. Maria (72, Pensionistin)
- **Problem:** ORF-Gebühren bezahlt, trotzdem Inkasso-Brief, hat Angst
- **Braucht:** Sicherheit, einfache Systeme
- **Tonfall für Maria:** Beruhigend, klar, würdevoll

### 4. Entwickler (25-45, Tech-affin)
- **Problem:** Will helfen, weiß nicht wo anfangen
- **Braucht:** Technische Präzision, klare Contribution-Guidelines
- **Tonfall für Devs:** Präzise, ohne Bullshit, Open-Source-Kultur

### 5. Entscheidungsträger (Politik, Verwaltung)
- **Problem:** Sieht Probleme, fühlt sich machtlos im System
- **Braucht:** Fakten, ROI, Machbarkeit
- **Tonfall für Entscheider:** Sachlich, datenbasiert, konstruktiv

---

## 🌍 Österreichischer Kontext

**Wichtig:** ZugangsWeg.at ist ein **österreichisches** Projekt mit **globalem** Anspruch.

### Österreich-Bezüge:
- **Eisenstadt** (Lenas Heimatstadt, PanLab Maker-Space)
- **ID Austria** (digitales Desaster, 22% Adoption)
- **ORF/GIS** (Negativbeispiel: Zwangsgebühren, Bürokratie)
- **Österreichische Neutralität** (Chance für digitale Unabhängigkeit)

### International Vergleichen mit:
- **Estland** (digitaler Vorreiter: 99% e-Government-Nutzung)
- **Singapur** (effiziente Verwaltung)
- **Signal** (USA, aber global, Non-Profit)

**Tonfall:**
- ✅ Stolz auf österreichische Qualität (Handwerk, Präzision)
- ✅ Kritisch gegenüber österreichischer Bürokratie
- ✅ Offen für internationale Best Practices

---

## 💚 Die drei Personen, die ZugangsWeg.at inspiriert haben

### 1. Georg (Fliesenleger, 56)
**Zitat:** "Ich MUSS das tragen (Smartwatch), aber ich KANN es nicht bedienen."
**Lösung:** Oma-Modus für Smartwatches, simple UI

### 2. Sarah (Ex-Aktivistin, 19)
**Zitat:** "Welche anderen Wege? Zeig sie mir. Bitte."
**Lösung:** Von Kleben zu Bauen - FoodShare statt Straßenblockade

### 3. Maria (Pensionistin, 72)
**Zitat:** "Dann bau ein neues."
**Lösung:** Einfache, verständliche Systeme ohne Angst

**Diese drei Menschen sind IMMER im Hinterkopf behalten!**

Wenn Georg, Sarah und Maria das nicht verstehen → vereinfachen!

---

## 🔧 Technische Philosophie

### Open Source (geplant)
- ✅ Code wird veröffentlicht (noch nicht final welche Lizenz)
- ✅ Transparent (jeder kann sehen, wie es funktioniert)
- ✅ Community-Contributions willkommen

### Privacy by Design
- ✅ Datenminimierung (nur was nötig ist)
- ✅ Zweckbindung (nur für das was versprochen wurde)
- ✅ Keine Monetarisierung von Nutzerdaten (NIEMALS!)

### Accessibility by Default
- ✅ WCAG 2.1 AA Minimum (besser: AAA wo möglich)
- ✅ Keyboard-Navigation
- ✅ Screen Reader Support
- ✅ Mobile-First

---

## 🎯 Mission Statement

**Für AI-Tools (du kannst das als Kontext verwenden):**

> ZugangsWeg.at ist eine Bewegung, die Menschen befähigt, gesellschaftliche Probleme gemeinsam zu lösen.
>
> Wir glauben, dass gute Systeme kein Privileg sind, sondern ein Recht.
> Wir glauben, dass Veränderung nicht von oben kommen muss, sondern von uns.
> Wir glauben, dass Datenschutz ein Menschenrecht ist, kein Geschäftsmodell.
>
> Wir sind in der ALPHA-Phase. Wir haben noch fast nichts. Aber wir haben eine Vision, ein Team und die Überzeugung, dass es möglich ist.
>
> Nicht die Politik. Nicht der Staat. Nicht die Großkonzerne.
> Sondern WIR.
>
> **Weil wir es verdient haben.**

---

## 📞 Kontakt für Fragen

**Projektleitung:**
Lena Kulnig
E-Mail: lena@zugangsweg.at

**GitHub Issues:**
https://github.com/LEEI1337/ZugangsWeg.at-Page/issues

---

## 🚀 Abschließende Gedanken

**Wenn du Code für dieses Projekt schreibst:**

1. Denke an **Georg** (steckt im Trainingsmodus fest)
2. Denke an **Sarah** (sucht andere Wege)
3. Denke an **Maria** (hat Angst vor Inkasso)

**Frage dich:**
- Würde das Georg helfen?
- Würde das Sarah Hoffnung geben?
- Würde das Maria beruhigen?

**Wenn JA → du bist auf dem richtigen Weg.**

**Weil sie es verdient haben.**
**Weil WIR es verdient haben.**

---

**Los geht's. JETZT.**

Lena Kulnig
Eisenstadt, November 2025
