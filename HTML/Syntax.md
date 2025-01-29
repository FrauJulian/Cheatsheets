# HTML-Syntax

### Grundstruktur einer HTML-Tag-Deklaration
Ein HTML-Tag besteht aus:
- **Öffnendem Tag**: Beginnt das Element.
- **Attributen** (meist optional): Zusätzliche Informationen über das Element.
- **Inhalt** (optional): Zwischen dem öffnenden und schließenden Tag.
- **Schließendem Tag** (nicht immer erforderlich): Beendet das Element.

### Standard Zusammensetzung:

```html
<TAG <!-- Attribute --> > <!-- Öffnendem Tag -->
    <!-- Inhalt -->
</TAG> <!-- Schließendem Tag -->
```

zum Beispiel:

```html
<p class="text">
    Hallo Welt!
</p>
```

- `<p>` - öffnende Tag
- `class="text"` - ein Attribut
- `Hallo Welt!` - der Inhalt (können auch andere Tags sein | verschachtlung)
- `</p>` - schließende Tag.

### Kommentare in HTML

Mit `<!--` kann ein Kommentar geöffnet werden, mit `-->` wiederum geschlossen.

```html
<!-- Dies ist ein Kommentar -->
```
