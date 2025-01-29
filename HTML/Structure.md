# HTML-Struktur

### Beispiel:
```html
<!DOCTYPE html>
<html lang="en">
<head>

    <!-- WEBSEITEN METAINFORMATION -->
    <title>Titel</title>

</head>
<body>

<!-- SICHTBAREN WEBSEITEN INHALT -->
<h1>Sichtbaren Inhalt</h1>

</body>
</html>
```

### `<!DOCTYPE html>`
- Deklariert das Dokument als HTML5.

### `<html lang="en">`
- Der `<html>`-Tag umschließt das gesamte HTML-Dokument.
- Mögliche Attribute:
    - `lang="en"` - Gibt die Sprache des Dokuments an. (`en` für Englisch)
    - `dir="ltr"` - Textausrichtung (`ltr` für Links, `rtl` für Rechts)

## `<head>`
- Enthält Metainformationen über das Dokument (z. B. Zeichensatz, Titel, Stylesheets).
- Typische Metainformationen werden durch folgende Tags definiert:
    - `<meta>` - allgemeine Metadaten
    - `<title>` - den Dokumenttitel
    - `<link>` - externe Ressourcen wie Stylesheets
    - `<style>` - internes CSS
    - `<script>` - JavaScript
    - `<base>` - die Basis-URL des Dokuments

### `<body>`
- Enthält den sichtbaren Inhalt der Webseite.
- Mögliche Attribute:
    - `onload` - Führt eine beliebige Funktion beim Laden der Seite aus.
    - `style` - Direkte CSS-Styles für den gesamten Body.
    - `class` oder `id` - Für CSS-Styling oder JavaScript-Interaktionen.
