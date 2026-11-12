# miez und wau – Website

Statische Infoseite für **miez und wau – Fellpflege für Hund und Katz** in Tann.
Die Seite besteht nur aus HTML, CSS und Bildern. Es gibt keine Datenbank, kein Formular, keine Cookies und kein Tracking.

## Inhalt der Seite

| Datei | Zweck |
|---|---|
| `index.html` | Startseite: Logo, Begrüßung, Leistungen (Krallen schneiden, Unterwolle entfernen, Ohren reinigen, in Form schneiden, Trimmen, Baden, Föhnen), Terminhinweis mit Telefon- und E-Mail-Link |
| `impressum.html` | Impressum nach § 5 DDG |
| `datenschutz.html` | Datenschutzerklärung nach DSGVO |
| `style.css` | Gesamtes Design (Farben als Variablen, mobil optimiert) |
| `img/logo.jpg`, `img/julia.jpg`, `img/hunde.jpg` | Logo und Fotos |

Termine gibt es nur nach Vereinbarung per Telefon oder E-Mail.

## Veröffentlichen mit GitHub Pages (kostenlos)

1. Account auf [github.com](https://github.com) anlegen.
2. Neues **öffentliches** Repository erstellen (Name: nur Kleinbuchstaben, Zahlen, Bindestriche, z. B. `miez-und-wau`).
3. Alle Dateien dieses Ordners hochladen. Die Startseite muss `index.html` heißen und im Hauptordner liegen.
4. Unter **Settings → Pages** bei „Source" den Branch `main` und den Ordner `/ (root)` wählen und speichern.
5. Nach 1–2 Minuten ist die Seite erreichbar unter `https://BENUTZERNAME.github.io/miez-und-wau`.
6. Optional: eigene Domain beim Registrar kaufen (meist ca. 1–2 € pro Monat), in Settings → Pages eintragen und beim Registrar einen CNAME- bzw. A-Record anlegen. HTTPS wird dann automatisch aktiviert.

Alternativen mit ähnlichem Ablauf: Cloudflare Pages, Netlify, Codeberg Pages.

## Worauf zu achten ist

### Rechtliches
- [x] **Impressum** vorhanden und von jeder Seite im Footer verlinkt. Bei Änderungen (neue Anschrift, Telefonnummer, Umsatzsteuer-ID) aktualisieren. Eine Umsatzsteuer-ID gehört dazu, falls vorhanden (Platzhalter-Kommentar steht in `impressum.html`).
- [x] **Datenschutzerklärung** vorhanden und im Footer verlinkt.
- [x] **Datenschutzerklärung passt zum Hoster:** Der Abschnitt „Hosting und Server-Logfiles" nennt GitHub Pages (GitHub Inc., USA). Wechselst du später den Anbieter (z. B. Cloudflare Pages, Netlify oder IONOS), muss dieser Abschnitt entsprechend geändert werden.
- [x] Beide Telefonnummern (Deutschland und Österreich) stehen im Impressum.

### Datenschutz im Code
- [x] Keine externen Einbindungen (Google Fonts, YouTube, Google Maps, Analytics). Schriften kommen vom Gerät der Besucher.
- [x] Keine Cookies, daher kein Cookie-Banner nötig.
- [ ] **Bei künftigen Änderungen beachten:** Sobald Karten, Videos, Schriften von fremden Servern oder Statistik-Tools eingebaut werden, ändert sich die Rechtslage. Dann Datenschutzerklärung anpassen und ggf. Einwilligung einholen. Für Anfahrt besser nur einen Link auf die Karte setzen statt sie einzubetten.

### Technik und Inhalt
- [x] **Kein Kontaktformular**, stattdessen `tel:`- und `mailto:`-Links. Statische Seiten brauchen für Formulare einen externen Dienst.
- [x] Seite ist für Smartphones optimiert (Viewport-Tag und Media Query vorhanden). Vor dem Livegang auf dem Handy testen.
- [x] Bilder haben Alt-Texte und feste Breiten/Höhen, damit die Seite beim Laden nicht springt.
- [x] **Bilder** sind komprimiert (Fotos ca. 125–195 KB, Logo ca. 50 KB). Neue Bilder vor dem Upload ebenfalls mit einem Tool wie [Squoosh](https://squoosh.app) verkleinern.
- [x] Impressum und Datenschutz sind auf `noindex` gesetzt, damit sie nicht in Suchergebnissen auftauchen.

### Betrieb
- [ ] **Öffentliches Repository:** Alles darin ist für jeden sichtbar. Keine privaten Daten, Passwörter oder unveröffentlichten Entwürfe hochladen. Diese README enthält nur Angaben, die ohnehin auf der Seite stehen.
- [ ] **Eigene Domain statt `github.io`-Adresse:** Wirkt professioneller und ist bei Google leichter zu finden.
- [ ] **Backup:** Eine lokale Kopie aller Dateien aufbewahren (z. B. diese ZIP-Datei), falls ein Account gesperrt wird.
- [ ] Nach dem Livegang alle Links testen: Startseite, Impressum, Datenschutz, Telefon- und E-Mail-Links.

## Änderungen vornehmen

Texte stehen direkt in `index.html`, Farben und Layout in `style.css` (Farben oben im Block `:root`). Nach dem Bearbeiten die geänderten Dateien im Repository ersetzen. GitHub Pages aktualisiert die Seite dann automatisch nach ca. 1–2 Minuten.

## Kontakt

Julia Cizek, miez und wau, Denhartener Str. 24, 84367 Tann
E-Mail: julia.cizek@gmx.at
