# Silas Maissen – Handwerks-Website

Willkommen zur Website von Silas Maissen! Dies ist ein vollständiges, einseitiges Handwerks-Portfolio für Metallbau, Gartenservice und Seilarbeiten in Disentis. Die Website ist sofort einsatzbereit und für GitHub Pages optimiert.

---

## 📖 Inhaltsverzeichnis

- [Schnellstart](#schnellstart)
- [Bearbeitung der Website](#bearbeitung-der-website)
- [Bilder ersetzen](#bilder-ersetzen)
- [GitHub Pages Deployment](#github-pages-deployment)
- [Häufig gestellte Fragen](#häufig-gestellte-fragen)
- [English Version](#english-version)

---

## 🚀 Schnellstart

### Lokal testen (vor dem Upload zu GitHub Pages)

1. Öffnen Sie die Datei `index.html` direkt in Ihrem Browser (per Doppelklick oder Drag & Drop).
2. Die Website sollte sofort vollständig funktionieren, einschließlich:
   - Sticky-Navigation mit Ankern
   - Parallax-Effekt auf dem Hero-Bild
   - Funktionierendes Kontaktformular (öffnet Ihr Standard-E-Mail-Programm)
   - Lightbox für Portfolio-Bilder
   - Mobiles Hamburger-Menü

**Hinweis:** Das Kontaktformular funktioniert nur, wenn Sie einen E-Mail-Client konfiguriert haben, der `mailto:` Links unterstützt.

---

## ✏️ Bearbeitung der Website

Die Website ist so gestaltet, dass Sie alles direkt in `index.html` bearbeiten können. **Alle Bearbeitungspunkte sind deutlich mit deutschen Kommentaren gekennzeichnet.**

### Schritt 1: Datei öffnen

Öffnen Sie die Datei `index.html` mit einem Texteditor (z.B. VS Code, Notepad++, Sublime Text).

### Schritt 2: Nach „BEARBEITEN:" Kommentaren suchen

Suchen Sie im Texteditor nach dem Wort **`BEARBEITEN:`** um alle Stellen zu finden, die angepasst werden sollten.

### Wichtige Bearbeitungspunkte (in dieser Reihenfolge):

#### 🔧 **Meta-Daten & SEO** (oben im `<head>`)
```html
<title>Silas Maissen – Metallbau & Umgebungsarbeiten in Disentis</title>
<meta name="description" content="...">
```
- Ändern Sie den Seitentitel und die Meta-Beschreibung für Suchmaschinen.

#### 📞 **Kontaktnummern** (Hero & Kontakt-Sektion)
```html
<a href="tel:+41791234567" class="btn btn-primary">Jetzt anrufen</a>
<a href="https://wa.me/41791234567?text=..." class="btn btn-secondary">WhatsApp schreiben</a>
```
- Ersetzen Sie `+41791234567` mit Ihrer echten Telefonnummer (mit Ländercode +41).
- **Wichtig:** Bei WhatsApp muss die Nummer ohne + sein: `41791234567`

#### 🏠 **Hero-Sektion**
- H1 Überschrift (Seitentitel und Keywords)
- Intro-Paragraph (kurze Beschreibung)

#### 💼 **Leistungen (Services)**
Drei Service-Karten mit:
- Titel (z.B. „Metallbau")
- Beschreibung (Kurzer Text)
- Aufzählung typischer Aufgaben
- Icon (einfach ersetzen: `🔧`, `🌿`, `🧗`)

#### 👤 **Über Silas**
- Name
- Bio und Hintergrund
- Qualifikationen
- Persönliche Note (z.B. Ski-Info)

#### 📸 **Portfolio**
Suchen Sie nach `<!-- BEARBEITEN: Portfolio-Einträge -->`. Jedes Projekt:
```javascript
onclick="openLightbox('images/portfolio-X.jpg', 'Titel', 'Beschreibung')"
```
- Passen Sie Bilder, Titel und Beschreibungen an.

#### 📧 **Kontaktformular**
```html
<a href="mailto:silas@example.com?subject=...">
```
- Ersetzen Sie `silas@example.com` mit Ihrer echten E-Mail-Adresse.
- Das Formular sendet automatisch ein E-Mail-Fenster mit den Feldern.

#### 🗺️ **Google Maps Link**
```html
<a href="https://maps.google.com/?q=Disentis,Graubünden,Schweiz">
```
- Falls gewünscht, können Sie die Koordinaten anpassen.

#### 📋 **Impressum & Datenschutz** (Footer)
- Name, Adresse, Telefon, E-Mail eintragen.
- Berufshaftpflichtversicherung hinzufügen.
- Datenschutzhinweis bei Bedarf ergänzen.

#### 🎨 **Farben anpassen** (optional, oben im `<style>`)
```css
:root {
    --color-pine: #2d4a3e;        /* Tiefes Tannengrün */
    --color-slate: #4a5568;       /* Schiefergrau */
    --color-beige: #d4c5b9;       /* Warmes Beige */
    --color-accent: #b8956a;      /* Akzentfarbe */
}
```

---

## 🖼️ Bilder ersetzen

### Portrait-Bild (Über Silas)

1. Bereiten Sie Ihr Bild vor (empfohlen: JPG, ~400×400px, optimiert für Web).
2. Speichern Sie es als `silas-portrait.jpg` in den `images/` Ordner.
3. Keine weitere Bearbeitung nötig – das Bild wird automatisch angezeigt.

**Placeholder-Bild:** `images/silas-portrait.jpg`

### Portfolio-Bilder (6 Projekte)

1. Bereiten Sie 6 Bilder vor (empfohlen: JPG, ~400×300px, optimiert).
2. Speichern Sie sie als:
   - `images/portfolio-1.jpg` – Terrassengeländer
   - `images/portfolio-2.jpg` – Gartensanierung
   - `images/portfolio-3.jpg` – Fassadensanierung
   - `images/portfolio-4.jpg` – Schmiedetore
   - `images/portfolio-5.jpg` – Baumkrone-Arbeiten
   - `images/portfolio-6.jpg` – Stahlkonstruktion

3. Ändern Sie die Titel und Beschreibungen im entsprechenden `onclick` Attribut in `index.html`:
```javascript
onclick="openLightbox('images/portfolio-X.jpg', 'Neuer Titel', 'Neue Beschreibung')"
```

### Tipps für Bilder

- **Größe optimieren:** Verwenden Sie Tools wie [TinyJPG](https://tinyjpg.com) oder [Squoosh](https://squoosh.app)
- **Format:** JPG für Fotos, PNG für Grafiken mit Transparenz
- **Lazy Loading:** Alle Bilder werden mit `loading="lazy"` geladen (schnellere Seitenladezeit)

---

## 🌐 GitHub Pages Deployment

### Schritt 1: GitHub-Repository erstellen

1. Gehen Sie zu [GitHub.com](https://github.com)
2. Klicken Sie auf **New Repository**
3. **Repository-Name:** `silas-maissen` (oder beliebig, z.B. `username.github.io` für Custom Domain)
4. **Beschreibung:** Optional (z.B. "Handwerks-Website")
5. **Public** (erforderlich für kostenlose GitHub Pages)
6. Klicken Sie auf **Create Repository**

### Schritt 2: Dateien hochladen

#### Option A: Mit Git (empfohlen für Anfänger)

1. Installieren Sie [Git](https://git-scm.com)
2. Öffnen Sie die Terminal/Kommandozeile im Projektordner
3. Führen Sie folgende Befehle aus:

```bash
git init
git add .
git commit -m "Initial commit: Silas Maissen website"
git branch -M main
git remote add origin https://github.com/USERNAME/silas-maissen.git
git push -u origin main
```

Ersetzen Sie `USERNAME` mit Ihrem GitHub-Benutzernamen.

#### Option B: Mit GitHub Desktop (grafisch)

1. Installieren Sie [GitHub Desktop](https://desktop.github.com)
2. Klicken Sie auf **File** → **Add Local Repository**
3. Wählen Sie den `silas-maissen-website` Ordner
4. Klicken Sie auf **Create Repository**
5. Geben Sie eine Commit-Nachricht ein und klicken Sie **Publish Repository**

### Schritt 3: GitHub Pages aktivieren

1. Gehen Sie zum Repository auf GitHub
2. Klicken Sie auf **Settings** (oben rechts)
3. Scrollen Sie zu **GitHub Pages**
4. Unter **Source** wählen Sie **Deploy from a branch**
5. Wählen Sie Branch: **main** und Ordner: **root** (`/`)
6. Klicken Sie **Save**

### Schritt 4: Website aufrufen

Nach ~1–2 Minuten ist Ihre Website verfügbar unter:

```
https://USERNAME.github.io/silas-maissen/
```

oder (falls Sie das Repository `username.github.io` genannt haben):

```
https://USERNAME.github.io/
```

---

## 🌍 Custom Domain einrichten (Optional)

Wenn Sie eine eigene Domain haben (z.B. `silas-handwerk.com`):

### Schritt 1: CNAME-Datei bearbeiten

1. Öffnen Sie die Datei `CNAME` im Repository (oben im Ordner)
2. Ersetzen Sie den Inhalt mit Ihrer Domain:
```
silas-handwerk.com
```
3. Speichern und pushen Sie (Commit)

### Schritt 2: DNS-Einstellungen bei Ihrem Domain-Anbieter

Dies hängt von Ihrem Anbieter ab. **Generelle Schritte:**

1. Melden Sie sich bei Ihrem Domain-Anbieter an (z.B. GoDaddy, Namecheap, Swisscom)
2. Suchen Sie die DNS-Einstellungen / **DNS Records**
3. Erstellen Sie einen **CNAME**-Record:
   - **Name:** `www` (oder Subdomain)
   - **Points to:** `USERNAME.github.io`
4. Erstellen Sie optional einen **A**-Record für die Hauptdomain:
   - Folgen Sie [GitHub Pages Dokumentation](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

**Warten Sie 15–48 Stunden, bis die DNS-Änderungen propagiert sind.**

---

## 🛠️ Erweiterte Konfiguration

### CSS/JS in separate Dateien verschieben

Falls Sie CSS und JavaScript in separate Dateien verschieben möchten:

1. Erstellen Sie:
   - `styles.css` (alle CSS-Regeln aus `<style>`)
   - `script.js` (alle JS aus `<script>`)

2. Ersetzen Sie in `index.html`:
```html
<!-- Alt: -->
<style>... 1000+ Zeilen ...</style>

<!-- Neu: -->
<link rel="stylesheet" href="styles.css">
```

3. Ähnlich für JavaScript unten vor `</body>`:
```html
<!-- Alt: -->
<script>... 200+ Zeilen ...</script>

<!-- Neu: -->
<script src="script.js"></script>
```

### Google Analytics hinzufügen (optional)

Falls Sie Seitenaufrufe tracken möchten (bitte Datenschutzerklärung anpassen):

1. Erstellen Sie Konto auf [Google Analytics](https://analytics.google.com)
2. Kopieren Sie den Tracking-Code
3. Fügen Sie ihn vor dem `</head>` in `index.html` ein

**Wichtig:** Aktualisieren Sie die Datenschutzerklärung im Footer!

---

## ❓ Häufig gestellte Fragen

**F: Das Kontaktformular funktioniert nicht!**  
A: Das Formular öffnet Ihr Standard-E-Mail-Programm. Stellen Sie sicher, dass Sie einen E-Mail-Client (Outlook, Mail, Thunderbird, etc.) konfiguriert haben. Alternativ können Besucher die WhatsApp- oder Telefonlinks nutzen.

**F: Kann ich das Formular an einen Server senden?**  
A: Ja, aber Sie benötigen einen Backend-Service. Optionen:
- [Formspree](https://formspree.io) (kostenlos, 50 E-Mails/Monat)
- [Basin](https://usebasin.com)
- [Getform](https://getform.io)

**F: Kann ich die Farben ändern?**  
A: Ja! Suchen Sie nach `:root` in der `<style>` Sektion und ändern Sie die Hex-Farbwerte.

**F: Wie mache ich die Website schneller?**  
A: 
- Optimieren Sie Bilder (TinyJPG, Squoosh)
- Nutzen Sie moderne Bildformate (WebP statt JPG)
- Verwenden Sie ein CDN (z.B. Cloudflare, kostenlos)

**F: Ist die Website DSGVO-konform?**  
A: Ja! Es gibt:
- ✅ Keine Cookies
- ✅ Kein Tracking
- ✅ Keine Analytics
- ✅ Datenschutzerklärung im Footer
  
Die Website speichert nur Kontaktdaten, wenn ein Besucher das Formular absendet (lokal in seinem E-Mail-Programm).

**F: Kann ich ein anderes Logo/Design verwenden?**  
A: Ja! Passen Sie an:
- Logo (Text in HTML): `.logo { ... }`
- Farben: `:root { ... }`
- Schriftart: `--font-family`
- Hero-Hintergrund (SVG): `.hero-background`

---

## 📱 Responsive Design

Die Website funktioniert perfekt auf:
- 💻 Desktop (1920px+)
- 📱 Tablet (768px–1024px)
- 📱 Smartphone (320px–767px)

Das Hamburger-Menü erscheint automatisch auf kleinen Bildschirmen.

---

## 🔒 Sicherheit & Datenschutz

- **Keine Cookies:** ✅
- **Kein Tracking:** ✅
- **HTTPS auf GitHub Pages:** ✅ (automatisch)
- **SSL-Zertifikat:** ✅ (kostenlos von GitHub)

---

## 📄 Lizenz

Diese Website steht unter der MIT-Lizenz. Siehe `LICENSE` Datei.

---

---

# English Version

## Quick Start

1. **Open locally:** Double-click `index.html` to preview in your browser
2. **Edit content:** Look for `<!-- BEARBEITEN: ... -->` comments in `index.html`
3. **Replace images:** Swap placeholder files in `images/` folder
4. **Deploy to GitHub Pages:** Push to GitHub and enable Pages in Settings

## Key Edit Points

- **Phone number:** Replace `+41791234567` in hero and contact sections
- **WhatsApp:** Update link in hero and contact (without +, e.g., `41791234567`)
- **Email:** Update `silas@example.com` in footer and contact form
- **Services:** Edit titles, descriptions, and task lists
- **Portfolio:** Replace images and update project titles/descriptions
- **Impressum & Privacy:** Update in footer section

## GitHub Pages Setup

1. Create repository on [GitHub.com](https://github.com)
2. Push files (use Git or GitHub Desktop)
3. Enable Pages in **Settings** → **GitHub Pages** → **Deploy from branch** (main, root)
4. Website available at `https://USERNAME.github.io/silas-maissen/`

## Custom Domain (Optional)

1. Edit `CNAME` file → enter your domain (e.g., `silas-handwerk.com`)
2. Configure DNS at your registrar (CNAME record pointing to `USERNAME.github.io`)
3. Wait 15–48 hours for propagation

## Contact Form

The form uses `mailto:` – it opens the visitor's email client with pre-filled subject and message. Update the email address in the contact section and footer.

## Image Optimization

- Use JPG for photos (~400×300px for portfolio, ~400×400px for portrait)
- Optimize with [TinyJPG](https://tinyjpg.com) or [Squoosh](https://squoosh.app)
- Lazy loading is enabled automatically

## FAQs

**Q: How do I change colors?**  
A: Edit `:root` variables in the `<style>` section (hex color codes)

**Q: How do I track visitors?**  
A: Add Google Analytics code before `</head>` (update privacy policy accordingly)

**Q: Can I use a backend email service?**  
A: Yes – replace the mailto: action with a service like Formspree, Basin, or Getform

**Q: Is the site GDPR-compliant?**  
A: Yes – no cookies, no tracking, no analytics. Privacy notice included.

---

## 🎉 Fertig!

Gratulieren Sie sich selbst – Sie haben eine professionelle, vollständig anpassbare Website für Ihr Handwerk! 🔨

**Fragen?** Lesen Sie die Kommentare direkt in `index.html` oder konsultieren Sie die Dokumentation oben.

**Viel Erfolg mit Ihrer Website!** 🚀
