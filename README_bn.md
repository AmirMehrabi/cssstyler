# অবদান স্বীকার #

এই প্রকল্পটি একটি ফর্ক। [মূল রিপোটি](https://github.com/senchalabs/cssbeautify) দেখুন।


# সিএসএস বিউটিফাই #

সিএসএস বিউটিফাই [সিএসএস](http://www.w3.org/Style/CSS/) এ লিখিত স্টাইলের নতুন রূপ তৈরির জন্য করা জাভাস্ক্রিপ্ট ইমপ্লিমেন্টেশন।

নিচে একটি স্টাইল দেয়া হলোঃ

```css
menu{color:red} navigation{background-color:#333}
```

সিএসএস বিউটিফাই যা করবেঃ

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

[amirmehrabi.github.io/cssstyler/](https://amirmehrabi.github.io/cssstyler/) তে এটি অনলাইনে চেষ্টা করুন।

আরও উদাহরণের জন্য, এর [টেস্ট স্যুট](http://cssbeautify.com/test/) দেখুন।


# স্ক্রিনশট #

![screencapture-localhost-cssstyler-index-en-html-2019-10-15-15_36_23](https://user-images.githubusercontent.com/3878847/66830108-93ad8700-ef61-11e9-95d9-df30792b5aef.png)

## cssbeautify() ফাংশন ব্যবহার ##

সিএসএস বিউটিফাই জাভাস্ক্রিপ্ট দিয়ে লেখা হওয়ায় সেখানে জাভাস্ক্রিপ্ট রান হয়, সেখানে এটিও রান করা যাবে।

এপিআইটি একদম সহজ।

```javascript
var result = cssbeautify(style, options);
```

**options** is an optional object to adjust the formatting. Known options so far are:

  *  <code>indent</code> is a string used for the indentation of the declaration (default is 4 spaces)
  *  <code>openbrace</code> defines the placement of open curly brace, either *end-of-line* (default) or *separate-line*.
  *  <code>autosemicolon</code> always inserts a semicolon after the last ruleset (default is *false*)

কল উদাহরণঃ

```javascript
var beautified = cssbeautify('menu{opacity:.7}', {
    indent: '  ',
    openbrace: 'separate-line',
    autosemicolon: true
});
```

## অবদান রাখুন ##

আপনার অবদান স্বাগতম! আরও তথ্যের জন্য অনুগ্রহপূর্বক [অবদান গাইড](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md) পড়ুন।

## লাইসেন্স ##

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
