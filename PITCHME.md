## PackageManagers

---

@snap[west]

パッケージ管理ツールとは…

@color[white](a)

ソフトウェアのインストールやアンインストール、

アップデートなどが簡単にできるツールのこと。

@color[red](ソフトウェア同士の依存関係)も管理できる。

@snapend

+++

@snap[west]

Aパッケージをインストールするのに、

Bパッケージが先に入っていることが条件な場合 @color[blue](@fa[frown])

@color[white](a)

@fa[arrow-right] 自動的にインストールをしてくれる @color[orange](@fa[laugh-beam])

@snapend

---

@snap[west]

CパッケージとDパッケージは

同時にインストールしてはいけない場合 @color[blue](@fa[frown])

@color[white](a)

@fa[arrow-right] 警告を出してダメということを教えてくれる @color[orange](@fa[laugh-beam])

@snapend

+++

@snap[west]

パッケージとは…

@color[white](a)

ソフトウェアを構成するためのファイルが一式に

まとまったもの。設定ファイルやドキュメント、

プログラム本体、そのプログラムが正しく動くために

必要なライブラリなどが含まれている。

@snapend

---

@snap[west]

パッケージ管理ツールにはたくさんの種類があり、

プログラム言語や開発環境によって異なる。

@color[white](a)

Node.js @color[orange](@fa[handshake]) npm, yarn　  @color[white](ll) Ruby @color[orange](@fa[handshake]) Gem
PHP @color[orange](@fa[handshake]) Composer 　　　Python @color[orange](@fa[handshake]) pip
Linux @color[orange](@fa[handshake]) yum, rpm　　　 MacOS @color[orange](@fa[handshake]) Homebrew

@snapend

---

@snap[west]

パッケージ管理ツールを使うことによって…

@color[white](a)

パッケージのインストールなどの処理が、
手動で処理するよりも@color[red](高速)に、かつ、@color[red](正確)に行うことができる。

@snapend

---

@snap[west]

パッケージマネージャーの誕生経緯

@color[white](a)

JavaScript = フロントエンド言語
↓
時代が進むにつれ、サーバサイドでも処理可能
↓
Node.jsが誕生する

@snapend

---

@snap[west]

@size[1.5em](npm)とは…

@color[white](a)

@color[orange](Node Package Manager)の略。

JavaScript（Node.js）のパッケージを効率よく

管理する便利なツールのこと。

@snapend

---

@snap[west]

npmを使うためには…

@color[white](a)

Node.jsをインストールすれば、

npmも自動的にインストールされ使えるようになる

@snapend

---

@snap[west]

どんなパッケージがあるのか

@color[white](a)

@color[orange](@fa[splotch]) @size[1.5em](express)

@color[white](a)

Node.jsのWebアプリケーション開発で利用できる

Webフレームワーク。高速でかつ軽量、とても人気

@snapend

---

@snap[west]

どんなパッケージがあるのか

@color[white](a)

@color[orange](@fa[splotch]) @size[1.5em](lodash)

@color[white](a)

便利な関数をまとめて提供しているライブラリ。

配列や数値、オブジェクト、文字列の扱いを簡単にす

@snapend

---

@snap[west]

どんなパッケージがあるのか

@color[white](a)

@color[orange](@fa[splotch]) @size[1.5em](chalk)

@color[white](a)

ターミナル上の文字列をスタイリングしてくれる

文字や背景の色を変更したり下線を引いたりできる

@snapend

---

コマンド

---

npmとyarnとの違い

---

npxとは

---

Packageロック.jsonとは

---

nodeっていうフレームワークについて

---

バージョン指定でダウンロードできる

---
