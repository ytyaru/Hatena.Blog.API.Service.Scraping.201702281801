# このソフトウェアについて

はてなブログAPIで取得したサービス文書XMLファイルから一部データを抜き取る。

# 開発環境

* Linux Mint 17.3 MATE
* Firefox 42.0
* Python 3.4.3

## Webサービス

* [はてなブログAPI](http://developer.hatena.ne.jp/ja/documents/blog/apis/atom)
    * サービス文書URI(`https://blog.hatena.ne.jp/{はてなID}/{ブログID}/atom`)

# 準備

[こちら](https://github.com/ytyaru/Hatena.Blog.API.Service.Get.201702281505)ではてなブログサービス文書を取得し、XMLファイル保存しておくこと。

# 実行

```sh
python3 main.py
```

# 結果

サービス文書XMLファイルから一部データを抜き取り、コンソールに表示される。

* ブログのタイトル
* <link rel=next>のhref属性値
* <entry>の<title>テキストノード値

# ライセンス

このソフトウェアはCC0ライセンスである。

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")](http://creativecommons.org/publicdomain/zero/1.0/deed.ja)

なお、使用させていただいたライブラリは以下のライセンスである。感謝。

なお、使用させていただいたPythonライブラリは以下のライセンスである。感謝。

Library|License|Copyright
-------|-------|---------
[xmltodict](https://github.com/martinblech/xmltodict)|[MIT](https://opensource.org/licenses/MIT)|[Copyright (C) 2012 Martin Blech and individual contributors.](https://github.com/martinblech/xmltodict/blob/master/LICENSE)
[requests_oauthlib](https://github.com/requests/requests-oauthlib)|[ISC](https://opensource.org/licenses/ISC)|[Copyright (c) 2014 Kenneth Reitz.](https://github.com/requests/requests-oauthlib/blob/master/LICENSE)
[bs4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)|[MIT](https://opensource.org/licenses/MIT)|[Copyright © 1996-2011 Leonard Richardson](https://pypi.python.org/pypi/beautifulsoup4),[参考](http://tdoc.info/beautifulsoup/)

