# Disclaimer of credit #

Proyek ini merupakan *fork*. Lihat pada [Main repo](https://github.com/senchalabs/cssbeautify) .


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

Dipersilahkan untuk berkontribusi! Silahkan baca [Contribution Guide](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md) untuk info lebih lanjut.

## License ##

Hak Cipta (C) 2012 Sencha Inc.
Hak Cipta (C) 2011 Sencha Inc.

Izin menggunakan ini diperbolehkan, bebas untuk mengubah, kepada siapa pun yang mendapatkan salinannya
perangkat lunak ini dan file dokumentasi terkait ("Perangkat Lunak"), untuk menggunakan Perangkat Lunak tanpa batasan, termasuk tanpa batasan untuk menggunakan, menyalin, memodifikasi, menggabungkan, menerbitkan, mensublisensikan, dan / atau menjual salinan Perangkat Lunak, dan untuk mengizinkan orang-orang kepada siapa Perangkat Lunak ini disediakan untuk melakukannya, tunduk pada ketentuan berikut:

Pemberitahuan hak cipta di atas dan pemberitahuan izin ini harus dimasukkan dalam semua salinan atau bagian penting Perangkat Lunak.

PERANGKAT LUNAK INI DISEDIAKAN "SEBAGAIMANA ADANYA", TANPA JAMINAN APA PUN, BAIK TERSURAT MAUPUN TERSIRAT, TERMASUK TETAPI TIDAK TERBATAS PADA JAMINAN PENJUALAN DAGANG, KESESUAIAN UNTUK TUJUAN TERTENTU DAN TIDAK MELIPUTI PELANGGARAN. DALAM KEJADIAN APA PUN PENULIS ATAU PEMEGANG HAK CIPTA TIDAK BERTANGGUNG JAWAB ATAS KLAIM, KERUSAKAN ATAU KEWAJIBAN LAINNYA, BAIK DALAM TINDAKAN KONTRAK, KETENTUAN ATAU KATA LAINNYA, BANGKIT DARI, DI LUAR ATAU DALAM HUBUNGAN DENGAN PERANGKAT LUNAK ATAU PENGGUNAAN LAINNYA.
