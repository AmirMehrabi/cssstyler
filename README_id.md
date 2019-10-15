# Disclaimer of credit #

This project is a fork. Take a look at the [Main repo](https://github.com/senchalabs/cssbeautify) .


# CSS Beautify #

CSS Beautify merupakan implementasi JavaScript untuk mempercantik gaya tulis [CSS](http://www.w3.org/Style/CSS/).

Dari gaya tulis berikut:

```css
menu{color:red} navigation{background-color:#333}
```

CSS Beautify akan menuliskan ulang menjadi:

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

Coba secara langsung di [amirmehrabi.github.io/cssstyler/](https://amirmehrabi.github.io/cssstyler/).

Sebagai contoh, lihat juga [test suite](http://cssbeautify.com/test/).


# Screenshots #

![screencapture-localhost-cssstyler-index-en-html-2019-10-15-15_36_23](https://user-images.githubusercontent.com/3878847/66830108-93ad8700-ef61-11e9-95d9-df30792b5aef.png)

## Using cssbeautify() function ##

Karena CSS Beautify ditulis dalam JavaScript murni, ia dapat berjalan di mana saja yang dapat dijalankan JavaScript.

API-nya sangat simpel:

```javascript
var result = cssbeautify(style, options);
```

**options** sebuah objek untuk menentukan gaya penulisan. Opsi yang ada sejauh ini:

  *  <code>indent</code> adalah string yang digunakan untuk lekukan/inden (standarnya adalah 4 spasi)
  *  <code>openbrace</code> mendefinisikan penempatan kurung kurawal terbuka, baik *end-of-line* (standar) atau *separate-line*.
  *  <code>autosemicolon</code> selalu menyisipkan titik koma di-akhir (defaultnya adalah *false*)

Contoh penggunaan:

```javascript
var beautified = cssbeautify('menu{opacity:.7}', {
    indent: '  ',
    openbrace: 'separate-line',
    autosemicolon: true
});
```

## Contributing ##

Contributions are welcomed! Please read the [Contribution Guide](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md) for more info.

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
