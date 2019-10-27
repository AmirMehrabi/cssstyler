# Αποποίηση ευθυνών #

Αυτό το έργο είναι μια διακλάδωση. Δείτε το στο [Main repo](https://github.com/senchalabs/cssbeautify) .


# CSS Beautify #

CSS Beautify είναι μια JavaScript υλοποίηση επαναδιαμόρφωσης των στυλ γραμμένων σε [CSS](http://www.w3.org/Style/CSS/).

Το ακόλουθο στυλ:

```css
menu{color:red} navigation{background-color:#333}
```

Με το CSS Beautify θα παραχθεί:

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

Δοκιμάστε online στο [amirmehrabi.github.io/cssstyler/](https://amirmehrabi.github.io/cssstyler/).

Για περισσότερα παραδείγματα, δείτε επίσης το [test suite](http://cssbeautify.com/test/).


# Screenshots #

![screencapture-localhost-cssstyler-index-en-html-2019-10-15-15_36_23](https://user-images.githubusercontent.com/3878847/66830108-93ad8700-ef61-11e9-95d9-df30792b5aef.png)

## Χρήση cssbeautify() function ##

Επειδή το CSS Beautify είναι γραμμένο σε καθαρή JavaScript, μπορεί να εκτελεστεί οπουδήποτε μπορεί να τρέξει JavaScript.

Αυτό είναι ένα πολύ απλό API:

```javascript
var result = cssbeautify(style, options);
```

**options** is an optional object to adjust the formatting. Known options so far are:

  *  <code>indent</code> is a string used for the indentation of the declaration (default is 4 spaces)
  *  <code>openbrace</code> defines the placement of open curly brace, either *end-of-line* (default) or *separate-line*.
  *  <code>autosemicolon</code> always inserts a semicolon after the last ruleset (default is *false*)

Παράδειγμα κλήσης:

```javascript
var beautified = cssbeautify('menu{opacity:.7}', {
    indent: '  ',
    openbrace: 'separate-line',
    autosemicolon: true
});
```

## Συνεισφορά ##

Η συνεισφορά είναι ευπρόσδεκτη! Παρακαλούμε διαβάστε το [Contribution Guide](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md) για περισσότερες πληροφορίες.

## Άδεια Χρήσης ##

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
