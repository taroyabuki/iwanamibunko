# 岩波文庫

『岩波文庫解説総目録』に合わせて，ISBN-13の先頭の978400と末尾の1桁，ISBN10の先頭の400と末尾の1桁は割愛している。

## 概要

ファイル名|重要度|内容|補足
-|-|-|-
isbnWithNicds.md|低|ISBNの使い回し|1個のISBNに複数のNCIDが対応する，つまりISBNは同じだがCiNii Booksでは区別されているものを，機械的に抽出した結果
isbnWithNicds2.md|高|ISBNの使い回し|isbnWithNicds.mdのうち，訳者の変更や内容の大幅変更があったもの
isbnWithNicds3.md|中|ISBNの使い回し|isbnWithNicds.md（機械的抽出）には載っていて，isbnWithNicds2.md（深刻なもの）には載っていないもの。（ISBNの使い回しが許容されるかもしれないもの）
titleWithIsbns.md|低|ISBNの変更|ISBNが変わった岩波文庫タイトル。常識的には変わって当然だが，岩波文庫的には例外的
itemWithoutIsbn.md|中|ISBNなし|CiNii Booksに登録されている岩波文庫タイトルで，ISBNがないもの（機械的抽出）

### 補足

シリーズものの場合は第1巻のみを調べている。この方針の欠点はいかのとおり。

* [『水滸伝 : 完訳（全10巻）』](https://ci.nii.ac.jp/ncid/BA37967648)と[『水滸傳（全13巻）』](https://ci.nii.ac.jp/ncid/BN00976053)のように，第1巻のISBNは異なるが，途中（この例では第10巻）のISBNは同じであるようなものは抽出できない。
* [『新訓萬葉集』](https://ci.nii.ac.jp/ncid/BN02932172)の上巻と[『万葉集』](https://ci.nii.ac.jp/ncid/BB11320467)のように，第1巻のISBNは同じだが，他の巻のISBNは異なるようなものは抽出できない。

isbnWithNicds2.mdに掲載されているものが深刻だということには，同意する人が多いと思う。isbnWithNicds3.mdに掲載されているものが深刻ではないということには，疑問を感じる人が多いかもしれない。

* 訳者あとがきが追加された場合（例：社会科学と社会政策にかかわる認識の「客観性」の[1998版]，[1999版
]，[2003版]）

その他

* 『新島襄書簡集』 https://ci.nii.ac.jp/ncid/BB08863996 と https://ci.nii.ac.jp/ncid/BN0868403X は同じに見えるが，CiNiiによると，前者は非売品とのこと。
* titleWithIsbns.mdのうち，『インディアスの破壊についての簡潔な報告』には訳者解説の追加，『テアイテトス』には底本の変更および補註の追加，『歌行灯』と『青年』には解説者の変更，『桜の実の熟する時』と『田舎教師』には解説者の追加，他のものには訳者の変更があったが，そういう例は上記「深刻な使い回し」にもあるため，ISBN変更の真の理由なのかどうかはわからない。

## 岩波文庫の書誌として最も信頼できるのは何か

[『岩波文庫解説総目録』](https://www.amazon.co.jp/dp/4000612093?tag=inquisitor-22)（以下，総目録）の新版（90年版 1927~2016）を堪能したので，これに関連した話を書いておこうと思います。

[![表紙](https://images-fe.ssl-images-amazon.com/images/P/4000612093.09.jpg)](https://www.amazon.co.jp/dp/4000612093?tag=inquisitor-22)

[短い説明](https://github.com/taroyabuki/iwanamibunko)

90年を超える歴史，約6000冊のコレクションを誇る岩波文庫が重要な文庫であることは間違いありません。しかし，その歴史のためか，書誌に関してはいろいろと難しいことがあります（そもそも，6000の数え方がよくわかりません）。次のような問題があります。

1. ISBNの使い回し
2. ISBNのないタイトルの存在
3. 記録に残らない重版時の内容変更

順番に行きます。

### ISBNの使い回し

最も有名なのは，ISBNの使い回し（[Wikipedia](https://ja.wikipedia.org/wiki/%E5%B2%A9%E6%B3%A2%E6%96%87%E5%BA%AB#ISBN.E3.82.B3.E3.83.BC.E3.83.89.E4.BD.BF.E3.81.84.E5.9B.9E.E3.81.97.E5.95.8F.E9.A1.8C)）でしょう。改版時に翻訳者が変わってもISBNはそのままになることがあります。そのせいで，「オンライン書店で新訳を買ったつもりが旧訳が届いた」などというトラブルも発生するようです。参考：[岩波文庫がISBNコードを上書き使用している件について（togetter）](https://togetter.com/li/1053696)

総目録はこの問題の解決には役立ちません。原書が同じものはまとめられ，ISBNは変わったとしても最新のものしか載っていないからです。たとえば『インディアスの破壊についての簡潔な報告』は，[1976年版（ISBNは334271）](https://ci.nii.ac.jp/ncid/BN00931907)と[2013年版（ISBNは358001）](https://ci.nii.ac.jp/ncid/BB13217312)があります。訳者が同じなのにISBNが変わった（岩波文庫としては）珍しい例なのですが，総目録に載っているISBNは358001だけなので，総目録だけを見てもISBNが変わったかどうかはわかりません。（総目録に倣って，ISBN-13の先頭の978400と末尾の1桁，ISBN10の先頭の400と末尾の1桁は割愛しています。）

この問題は，[CiNii Books](https://ci.nii.ac.jp/books/)を使って解決するのがよさそうです。CiNii BooksのデータベースはISBNでなくNCIDという独自のIDを振っているので，ISBNとNCIDの組を調べれば，ISBNの使い回しがわかります。（細かいことですが，，CiNii BooksからGoogle BooksへのリンクにはISBNが使われているので，CiNii BooksからGoogle Booksに飛ぶときは注意が必要です。間違っているものが少なくとも60件はあります。）

CiNii BooksのAPIで，岩波文庫（[親書誌IDがBN00015783](https://ci.nii.ac.jp/ncid/BN00015783)であるもの）を検索し，ISBNは同じでもNCIDは違うもの，つまりISBNが使い回されているものを機械的に抽出した結果がisbnWithNicds.md，そこから，旧字→新字のような，ISBNの使い回しが許容されそうなものを除いた結果がisbnWithNicds2.mdです。

翻訳者が変わったにもかかわらずISBNは変わらなかったものがたくさんあるので，それが岩波文庫の方針のように思えるかもしれませんが，原書は同じでも何らかの理由で違うISBNが振られたものもあります。これは当たり前のことだと思うのですが，岩波文庫では例外的です。こういう例を抽出した結果がtitleWithIsbns.mdです。

### ISBNのないタイトルの存在

1927年に創刊が始まった岩波文庫ですが，ISBNが使われるようになったのは1980年頃なので，その間に刊行されたものには，そもそもISBNが付いていません。CiNii Booksに登録されていて，ISBNがないものを抽出した結果がitemWithoutIsbn.mdです。

ここまでは，CiNii Booksと照会しながら調べてきましたが，CiNii Booksが最も信頼できる情報源なのかというと，そういうわけではありません。

第1に，このデータベースは大学図書館のデータベースなので，大学図書館が所蔵していないものは登録されていません。第2に，NCIDという独自のIDを振っているとは言っても，ISBNがない時代のものには，かなりの混乱がありそうです。

第2の例として，同一の書籍に複数のNCIDが振られているものを14件見つけました。ついでに，翻訳者が間違って登録されていたもの1件，ISBNがあるはずなのに登録されていなかったもの1件，タイトルの「他二編」の漢数字「二」がカタカナの「二」になっているものも見つけました。いずれも報告し，修正してもらいましたが，最後のものは発生理由を想像すると闇を覗いた気になります。

CiNiiがダメなら国会図書館はどうかというと，『人間に就いて』が誤って[『人間について』](http://iss.ndl.go.jp/books/R100000002-I000000840798-00)として登録されているなど，完璧というわけにはいきません。（本稿執筆時点）

### 記録に残らない重版時の内容変更

ISBNの問題を別にすれば総目録は完璧なのかというと，そういうわけではありません。

総目録には，「改版」は記録されていますが，「重版」は記録されていません。ふつうはそれでいいのですが，岩波文庫の場合は，重版時に解説が追加されることがあります。これが記録されていないのは困ります。以下の挙げるのは，記録されるべきだと思われるのに記録されていないものです。（＊の部分は岩波書店の「愛読者の窓」係に教えてもらいました。ありがとうございました。）

* p.122 [『浄土三部経』の「上」（付記あり）](https://ci.nii.ac.jp/ncid/BN11134503)（＊1983年21刷から）
* p.902 [『トオマス・マン短篇集』（141p）](https://ci.nii.ac.jp/ncid/BN06738160)（＊1941年13刷から）
* p.1018 [『スペードの女王 : 他一篇』（145p）](https://ci.nii.ac.jp/ncid/BN03780116)（＊1950年12刷から）
* p.1039 『闇の力』，1927.7.10, 128pの次が1938.9.25, 146pになっていますが，間に「第12刷(1937.12)に解題あり(p129-130)」というのが出版されているようです。[CiNii Books・東京大学ほか](https://ci.nii.ac.jp/ncid/BN01029127)，[国会図書館・横浜市中央図書館](http://iss.ndl.go.jp/books/R100000002-I000000657082-00)（版元では確認できず）
* p.1046 『紅い花』，1937.9.15『紅い花 : 他四篇』の次が1943.3.1の『紅い花 : 他三篇』になっていますが，1937年に『紅い花 : 他三篇』（[国会図書館・千葉県立図書館・広島県立図書館](http://iss.ndl.go.jp/books/R100000001-I074682877-00)）が出版されているのではないでしょうか。（版元では確認できず）
* p.1052 『桜の園』，1927.7.10, 94pの次が1937.4.15, 98pになっていますが，間に「解題: p95-98」を掲載したもの（[京都大学](https://ci.nii.ac.jp/ncid/BB17362550)）が出版されているのではないでしょうか。（版元では確認できず）

版元でも確認できないものについて，現物を確認できる人がいたら教えていただきたいです。

総目録には細かい間違いもあります。

たとえば，手元の総目録初版では，『草の葉』の翻訳者が「杉木喬, 鍋島能弘, 酒本雅之」になっていますが，岩波書店の「愛読者の窓」係に確認したところ，正しくは「酒本雅之」のみだそうです。正誤表の公開が待たれます。

[ウェブサイト](https://www.iwanami.co.jp/search/?search_menu=keyword&tab=3&search_word=%E8%8D%89%E3%81%AE%E8%91%89)は直っていますが，こちらには，旧版（有島武郎選訳とは別）の情報が出てこないという問題があります。

[![表紙](https://images-fe.ssl-images-amazon.com/images/P/4003500210.09.jpg)](https://www.amazon.co.jp/dp/4003500210?tag=inquisitor-22)

総目録では，『草の葉』旧版（上中下）の翻訳者は「杉木喬, 鍋島能弘, 酒本雅之」になっていますが，3人訳なのは上巻だけで，中と下の翻訳者は「鍋島能弘, 酒本雅之」だそうです。この点について，[『岩波文庫の80年』](https://www.amazon.co.jp/dp/4003500210?tag=inquisitor-22)は正しいです。総目録と『岩波文庫の80年』で統一のデータベースを使っているわけではないようです。『岩波文庫の80年』は単なる年表なので，書誌としては不十分なのですが，それでもとりあえず，『岩波文庫の90年』は出してほしいです。[CiNii Booksのデータ](https://ci.nii.ac.jp/ncid/BN01982175)は間違ってますね（本稿執筆時点）。

結論：岩波文庫の書誌として信頼できるものを見つけるのは難しいです。
