# Disclaimer of credit #

This project is a fork. Take a look at the [Main repo](https://github.com/senchalabs/cssbeautify) .
このプロジェクトはフォークです。 [Main repo]（https://github.com/senchalabs/cssbeautify）をご覧ください。

# CSS Beautify #

CSS Beautify is a JavaScript implementation of reindenter and reformatter for styles written in [CSS](http://www.w3.org/Style/CSS/).

Given the following style:

CSS Beautifyは、[CSS]（http://www.w3.org/Style/CSS/）で記述されたスタイルのreindenterとリフォーマッターのJavaScript実装です。

次のスタイルを考えます：

```css
menu{color:red} navigation{background-color:#333}
```

CSS Beautify will produce:

CSS Beautifyは以下を生成します。

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

Try it online at [amirmehrabi.github.io/cssstyler/](https://amirmehrabi.github.io/cssstyler/).

For more examples, see also its [test suite](http://cssbeautify.com/test/).


# Screenshots #

![screencapture-localhost-cssstyler-index-en-html-2019-10-15-15_36_23](https://user-images.githubusercontent.com/3878847/66830108-93ad8700-ef61-11e9-95d9-df30792b5aef.png)

## Using cssbeautify() function ##

Since CSS Beautify is written in pure JavaScript, it can run anywhere that JavaScript can run.

The API is very simple:


 Learn to pronounce
[cssbeautify.com]（http://cssbeautify.com）でオンラインで試してください。のために
コマンドラインを使用して、Node.js [cssbeautify]（https://npmjs.org/package/cssbeautify）パッケージをインストールします。

その他の例については、[テストスイート]（http://cssbeautify.com/test/）も参照してください。




## cssbeautify（）関数の使用##

CSS Beautifyは純粋なJavaScriptで記述されているため、JavaScriptが実行できる場所であればどこでも実行できます。

APIは非常に簡単です。

```javascript
var result = cssbeautify(style, options);
```

**options** is an optional object to adjust the formatting. Known options so far are:

  *  <code>indent</code> is a string used for the indentation of the declaration (default is 4 spaces)
  *  <code>openbrace</code> defines the placement of open curly brace, either *end-of-line* (default) or *separate-line*.
  *  <code>autosemicolon</code> always inserts a semicolon after the last ruleset (default is *false*)

Example call:

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


これにより、コピーを入手した人に無料で許可が与えられます
このソフトウェアおよび関連するドキュメントファイル（「ソフトウェア」）の
権利を含むがこれに限定されないソフトウェアの制限なし
使用、コピー、変更、マージ、公開、配布、サブライセンス、販売
ソフトウェアのコピー、およびソフトウェアの所有者を許可するため
次の条件に従って、そのように提供されます。

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
