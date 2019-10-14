## PackageManagers

---

@snap[west]

パッケージ管理ツールとは…
@color[white](a)
パッケージマネージャー、パッケージ管理システム
とも呼ばれている。
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
必要なライブラリなどが含まれているもの。

@snapend

---

@snap[west]

パッケージ管理ツールを使うことによって…
@color[white](a)
パッケージのインストールなどの処理が、
手動で処理する場合よりも@color[red](高速)に、かつ、@color[red](正確)に
行うことができる！

@snapend

---

@snap[west]

@color[orange](@fa[splotch])パッケージ管理ツールの誕生経緯
@color[white](a)
JavaScript = フロントエンド言語
@color[white](aaa)@fa[sort-down]
時代が進むにつれ、サーバサイドでも処理可能
@color[white](aaa)@fa[sort-down]
Node.jsが誕生する

@snapend

+++

@snap[west]

JavaScriptのフレームワークが開発される
@color[white](aaa)@fa[sort-down]
例えば、そのフレームワークは1000個の
プログラムで構成されている(とする)
@color[white](aaa)@fa[sort-down]
特定のファイルの書き換え、適切な場所への移動、
正常にインストールできたかの確認などを
全て人間が手作業で処理することはかなり困難 @color[blue](@fa[frown])

@snapend

+++

@snap[west]

ましてやバージョン管理なんて絶対無理やん…
@color[white](aaa)@fa[sort-down]
じゃあ、簡単なコマンド入力しただけで、
これらが実現できるようなツール作ってみるか〜 @color[orange](@fa[hand-holding-heart])
@color[white](aaa)@fa[sort-down]
パッケージ管理ツールが誕生！

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

@size[1.5em](npm)とは…
@color[white](a)
@color[orange](Node Package Manager)の略。
JavaScript（Node.js）のパッケージを効率よく
管理する便利なツールのこと。

@snapend

---

@snap[west]

npmを使うためには？
@color[white](a)
Node.jsをインストールすれば、
npmも自動的にインストールされ使えるようになる

@snapend

---

@snap[west]

@size[1.5em](yarn)とは…
@color[white](a)
npmと同じくNode.jsのパッケージを効率よく
管理する便利なツールのこと。
Node.jsをインストールすれば、使用できる。
2016年にFaceBookが公開した。

@snapend

---

@snap[west]

@color[orange](@fa[splotch])npmとyarnの違い
@color[white](a)
・平行処理でのインストール作業については
　npmよりもyarnのほうがスピードが速い
・


@snapend

---

@snap[west]



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
