# Disconoscimento di crediti #

Questo progetto è un fork. Take a look at the [Repository principale](https://github.com/senchalabs/cssbeautify) .


# CSS Beautify #

CSS Beautify è un'implementazione JavaScript di reindentatori e riformattatori per stili scritti in [CSS](http://www.w3.org/Style/CSS/).

Dato il seguente stile:

```css
menu{color:red} navigation{background-color:#333}
```

CSS Beautify produrrà:

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

Provalo online a [amirmehrabi.github.io/cssstyler/](https://amirmehrabi.github.io/cssstyler/).

Per altri esempi, vedi anche la sua [suite di test](http://cssbeautify.com/test/).


# Screenshot #

![screencapture-localhost-cssstyler-index-en-html-2019-10-15-15_36_23](https://user-images.githubusercontent.com/3878847/66830108-93ad8700-ef61-11e9-95d9-df30792b5aef.png)

## Usare la funzioni cssbeautify() ##

Poiché CSS Beautify è scritto in puro JavaScript, può essere eseguito ovunque JavaScript possa essere eseguito.

L'API è molto semplice:

```javascript
var result = cssbeautify(style, options);
```

**options** è un oggetto opzionale per regolare la formattazione. Le opzioni conosciute finora sono:

  *  <code>indent</code> è una stringa utilizzata per il rientro della dichiarazione (il valore predefinito è 4 spazi)
  *  <code>openbrace</code> definisce il posizionamento della parentesi graffa aperta, *fine linea* (impostazione predefinita) o *linea separata*.
  *  <code>autosemicolon</code> inserisce sempre un punto e virgola dopo l'ultimo set di regole (default è *falso*)

Esempio di chiamata:

```javascript
var beautified = cssbeautify('menu{opacity:.7}', {
    indent: '  ',
    openbrace: 'separate-line',
    autosemicolon: true
});
```

## Contributi ##

I contributi sono i benvenuti! Per favore leggi la [Guida alla contribuzione](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md) per più informazioni.

## Licenza ##

Copyright (C) 2012 Sencha Inc.
Copyright (C) 2011 Sencha Inc.

L'autorizzazione è concessa, gratuitamente, a chiunque ne ottenga una copia
di questo software e file di documentazione associati (il "Software"), da trattare
nel software senza restrizioni, compresi senza limitazione i diritti
per utilizzare, copiare, modificare, unire, pubblicare, distribuire, concedere in licenza e / o vendere
copie del software e per consentire alle persone a cui il software è fornito
di fare ciò, fatte salve le seguenti condizioni:

La suddetta nota sul copyright e questa nota di autorizzazione devono essere incluse in
tutte le copie o parti sostanziali del software.

IL SOFTWARE È FORNITO "COSÌ COM'È", SENZA ALCUN TIPO DI GARANZIA, ESPRESSA O
IMPLICATA, COMPRESO MA NON LIMITATO ALLE GARANZIE DI COMMERCIABILITÀ,
IDONEITÀ A UNO SCOPO PARTICOLARE E DI NON VIOLAZIONE. IN NESSUN CASO GLI
AUTORI O TITOLARI DEL COPYRIGHT SONO RESPONSABILI DI QUALSIASI RECLAMO, DANNI O ALTRO
RESPONSABILITÀ, SE IN AZIONE DI CONTRATTO, TORTO O ALTRO, DERIVANTE DA,
FUORI O IN CONNESSIONE CON IL SOFTWARE O L'USO O ALTRE OFFERTE NEL SOFTWARE.
