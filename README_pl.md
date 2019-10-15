# Notka na temat autora #

Ten projekt to fork. Zobacz [główne repozytorium](https://github.com/senchalabs/cssbeautify) .


# CSS Beautify #

CSS Beautify to JavaScriptowa implementacja reformattera dla styli napisanych w [CSS](http://www.w3.org/Style/CSS/).

Przy podaniu nastepujacego stylu:

```css
menu{color:red} navigation{background-color:#333}
```

CSS Beautify zwróci:

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

Wypróbuj online na [amirmehrabi.github.io/cssstyler/](https://amirmehrabi.github.io/cssstyler/).

Dla wiekszej ilosci przykladow, zobacz rowniez [pakiet testowy](http://cssbeautify.com/test/).


# Zrzuty ekranu #

![screencapture-localhost-cssstyler-index-en-html-2019-10-15-15_36_23](https://user-images.githubusercontent.com/3878847/66830108-93ad8700-ef61-11e9-95d9-df30792b5aef.png)

## Używanie funkcji cssbeautify() ##

Dlategom, że CSS Beautify jest napisane w czystym JavaScripcie, może byc uruchomione wszędzie gdzie JavaScript może być uruchomiony.

API jest bardzo proste:

```javascript
var result = cssbeautify(style, options);
```

**options** to opcjonalny obiekt aby dostować formatowanie. Dostępne opcje:

  *  <code>indent</code> to teskt uzywany do wcięć (domyślny to 4 spacje)
  *  <code>openbrace</code> definiuje położenie otwierającej klamerki, albo *end-of-line* (domyślne) albo *separate-line*.
  *  <code>autosemicolon</code> zawsze automatycznie dodaje sredniki po ostatnim zestawie reguł (domyślnie *false*)

Przykładowe użycie:

```javascript
var beautified = cssbeautify('menu{opacity:.7}', {
    indent: '  ',
    openbrace: 'separate-line',
    autosemicolon: true
});
```

## Pomoc ##

Pomoc jest mile widziana! Proszę przeczytaj [Contribution Guide](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md) for more info.

## Licencja ##

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
