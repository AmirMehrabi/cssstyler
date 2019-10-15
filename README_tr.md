# Sorumluluk reddi #

Bu proje çatal repodur. Asıl repoya bakın [Main repo](https://github.com/senchalabs/cssbeautify) .


# CSS Beautify #

CSS Beautify, CSS için yazılmış, kodların satır boşluklarını ve düzenini ayarlamaya yarayan bir JavaScript kütüphanesidir. [CSS](http://www.w3.org/Style/CSS/).


Aşağıdaki css yazıldığında:

```css
menu{color:red} navigation{background-color:#333}
```

CSS Beautify çıktısı:

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

Online olarak denemek için [amirmehrabi.github.io/cssstyler/](https://amirmehrabi.github.io/cssstyler/).

Daha fazla örnek için burayı ziyare et [test suite](http://cssbeautify.com/test/).


# Ekran görüntüleri #

![screencapture-localhost-cssstyler-index-en-html-2019-10-15-15_36_23](https://user-images.githubusercontent.com/3878847/66830108-93ad8700-ef61-11e9-95d9-df30792b5aef.png)

## cssbeautify() fonksiyon kullanımı ##

CSS Beautify saf Javascript ile yazıldığı için, JS çalışan her yerde çalıştırılabilir.

API çok basittir:

```javascript
var result = cssbeautify(style, options);
```

**options** **ayarlar**  düzenleme ayarlarını ayarlamak için opsiyonel bir JS objesidir. Bilinen ayarlar:

  *  <code>indent</code>  yazılan kodun satır başı boşluk bırakmasını sağlar (normal ayar 4 boşluktur)
  *  <code>openbrace</code> Tırtıklı parantezin açılacağı yeri belirler. *end-of-line* (normali) ya da *separate-line*.
  *  <code>autosemicolon</code> her kod parçasının sonuna noktalı virgül ekler. (normali *false*)

Örnek çağrı:

```javascript
var beautified = cssbeautify('menu{opacity:.7}', {
    indent: '  ',
    openbrace: 'separate-line',
    autosemicolon: true
});
```

##  Katkıda bulunmak ##

Katkıda bulunmak serbesttir. Lütfen katkıda bulunmadan önce detaylı bilgi için rehberi okuyun.

## Lisans ##

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