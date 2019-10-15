## Hinweis für Haftungsauschluss

Dieses Projekt ist nur ein fork. Das orginal Repo findet ihr unter [Main repo](https://github.com/senchalabs/cssbeautify)

# CSS Beautify

CSS Beautify ist eine JavaScript Implementation die in [CSS](http://www.w3.org/Style/CSS/) geschriebenenes automatisch einrückt und formatiert.

Wenn es in der folgenden Syntax angegeben ist:

```css
menu {
  color: red;
}
navigation {
  background-color: #333;
}
```

Wird CSS Beautify folgenden Code ausgeben:

```css
menu {
  color: red;
}

navigation {
  background-color: #333;
}
```

Probiere es online auf [cssbeautify.com](http://cssbeautify.com). Um es mit der Kommandozeile zu nutzen, installiere das Node.js [cssbeautify](https://npmjs.org/package/cssbeautify) Packet.

Für mehr Beispiele, schau dir die [test suite](http://cssbeautify.com/test/) an.

## Die cssbeautify() Funktion benutzen

Da CSS Beautify in purem Javascript geschrieben wurde, kann es überall ausgeführt werden.

Die API ist sehr einfach:

```javascript
var result = cssbeautify(style, options);
```

**options** ist ein optionales Objekt welches genutzt werden kann um die Formatierung anzupassen. Setzbare Optionen:

- <code>indent</code> ist ein String der für die Einrückung verwendet wird (Standard sind 4 Leerzeichen)
- <code>openbrace</code> definiert wo die geschweifte Klammer gesetzt wird, entweder am Ende der Zeile(Standard) oder in einer neuen Zeile.
- <code>autosemicolon</code> immer ein Semikolon nach der letzten CSS Regel anfügen (Standard ist _false_)

Beispiel Aufruf:

```javascript
var beautified = cssbeautify("menu{opacity:.7}", {
  indent: "  ",
  openbrace: "separate-line",
  autosemicolon: true
});
```

## Mitarbeiten

Beiträge sind gerne erwünscht! Bitte lese dir den [Contribution Guide](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md) für mehr Infos durch.

## Lizenz

Copyright (C) 2012 Sencha Inc.
Copyright (C) 2011 Sencha Inc.

Die Erlaubnis wird hiermit kostenlos jeder Person erteilt, die eine Kopie erhält.
Dieser Software und der dazugehörigen Dokumentationsdateien (die "Software"), um mit ihnen umzugehen.
in der Software ohne Einschränkung, einschließlich und ohne Einschränkung der Rechte.
verwenden, kopieren, modifizieren, fusionieren, veröffentlichen, verteilen, unterlizenzieren und/oder verkaufen.
Kopien der Software und um Personen, für die die Software bestimmt ist, zu ermöglichen.
zu diesem Zweck unter den folgenden Bedingungen zur Verfügung gestellt:

Der obige Urheberrechtshinweis und dieser Genehmigungshinweis müssen enthalten sein in
allen Kopien oder wesentliche Teile der Software.

DIE SOFTWARE WIRD "WIE ZU SEHEN" ZUR VERFÜGUNG GESTELLT, OHNE JEGLICHE GARANTIE, WEDER AUSDRÜCKLICH NOCH STILLSCHWEIGEND.
IMPLIZIT, EINSCHLIEßLICH, ABER NICHT BESCHRÄNKT AUF DIE GARANTIEN DER MARKTGÄNGIGKEIT,
EIGNUNG FÜR EINEN BESTIMMTEN ZWECK UND NICHTVERLETZUNG. IN KEINEM FALL DARF DIE
AUTOR ODER URHEBERRECHTSINHABER HAFTEN FÜR JEGLICHE ANSPRÜCHE, SCHÄDEN ODER ANDERE SCHÄDEN.
HAFTUNG, UNABHÄNGIG DAVON, OB ES SICH UM EINE VERTRAGSHANDLUNG, EINE UNERLAUBTE HANDLUNG ODER EINE ANDERE HANDELT,
AUS ODER IN VERBINDUNG MIT DER SOFTWARE ODER DER NUTZUNG ODER ANDEREN GESCHÄFTEN IN DEN BEREICHEN
DER SOFTWARE.
