# Avis de non-responsabilité en matière de crédit #

Ce projet est un dérivé. Jetez un œil au [dépôt principal](https://github.com/senchalabs/cssbeautify) .


# CSS Beautify #

CSS Beautify est une implémentation JavaScript pour ré-indenter and reformater les styles écrits en [CSS](http://www.w3.org/Style/CSS/).

Avec le style suivant :

```css
menu{color:red} navigation{background-color:#333}
```

CSS Beautify donnera :

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

Essayez-le en ligne sur [amirmehrabi.github.io/cssstyler/](https://amirmehrabi.github.io/cssstyler/).

Pour plus d'exemples, jetez également un coup d'œil sur cette [suite de tests](http://cssbeautify.com/test/).


# Captures d'écrans #

![screencapture-localhost-cssstyler-index-en-html-2019-10-15-15_36_23](https://user-images.githubusercontent.com/3878847/66830108-93ad8700-ef61-11e9-95d9-df30792b5aef.png)

## Utilisation de la fonction cssbeautify() ##

CSS Beautify étant écrit en JavaScript pure, il peut fonctionner partout où JavaScript fonctionne.

L'API est extrêmement simple :

```javascript
var result = cssbeautify(style, options);
```

**options** est un objet optionnel pour ajuster le formatage. Les options actuelles sont :

  *  <code>indent</code> est une chaîne de caractères utilisée pour l'indentation de la déclaration (par défaut 4 espaces)
  *  <code>openbrace</code> définit l'emplacement de l'accolade ouvrante, en fin de ligne *end-of-line* (par défaut) ou sur une ligne séparée *separate-line*.
  *  <code>autosemicolon</code> insère toujours un point-virgule après la dernière règle (la valeur par défaut est *false*)

Exemple d'appel :

```javascript
var beautified = cssbeautify('menu{opacity:.7}', {
    indent: '  ',
    openbrace: 'separate-line',
    autosemicolon: true
});
```

## Contributions ##

Les contributions sont les bienvenus ! Merci de lire le [Guide de contribution](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md) pour plus d'informations.

## License ##

Copyright (C) 2012 Sencha Inc.
Copyright (C) 2011 Sencha Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
