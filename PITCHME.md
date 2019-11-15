## PackageManagers

---

@snap[west]

パッケージマネージャとは…
@color[white](a)
パッケージ管理ツール、パッケージ管理システム
とも呼ばれている。
ソフトウェアのインストールやアンインストール、
アップデートなどが簡単にできるソフトのこと。
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
必要なモジュールなどが含まれているもののこと。
（モジュール > パッケージ > ライブラリ）

@snapend

---

@snap[west]

パッケージ管理ツールを使うことによって…
@color[white](a)
パッケージのインストールなどの作業が、
手動で処理する場合よりも@color[red](高速)に、かつ、@color[red](正確)に
行うことができる！

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
@color[red](Node Package Manager)の略。
JavaScript（Node.js）のパッケージを効率よく
管理する便利なツールのこと。
インストールしたパッケージの情報は、
@color[red](package.json)というファイルに記録される。

@snapend

---

@snap[west]

npmを使うためには？
@color[white](a)
Node.jsをインストールすれば、npmも一緒に
自動でインストールされ、使えるようになる。

@snapend

---

@snap[west]

パッケージのインストール方法
@color[white](a)
・グローバルインストール
・ローカルインストール

@snapend

---

@snap[west]

グローバルインストールって？
@color[white](a)
npmがある場所にパッケージをインストールする。
コマンドのパスが通るので指定なしで実行可能。
下記でhogeパッケージをインストールした場合、
コンソール画面でhogeコマンドとして操作できる。
@color[white](a)
@color[orange](@fa[pen])  `npm install -g hoge`

@snapend

---

@snap[west]

全てのプロジェクトから利用することができるため
よく使うモジュールやしコマンドを使いたい
という場合に便利な方法。
ただし、package.jsonには情報が@color[red](追記されない)。

@snapend

---

@snap[west]

ローカルインストールって？
@color[white](a)
package.jsonと同じ階層に@color[red](node_modules)という
ディレクトリが作成され、インストールされる。
下記のように「--save」をつけると、
package.jsonにバージョン情報が追記される。
@color[white](a)
@color[orange](@fa[pen])  `npm install --save hoge`

@snapend

---

@snap[west]

あるディレクトリにpackage.jsonを配置し、
@color[orange](@fa[pen])  `npm install`を実行すると、インストールしつつ
package.jsonを作成した時と同じ環境が作れる。
複数人で開発環境を揃えることなどに役立つ。
でも、パス付きじゃないとコマンドが実行できない。

@snapend

---

@snap[west]

だめ
@size[1.5em](npm scripts)とは…
@color[white](a)
あらかじめコマンドをpackage.jsonに定義しておき
簡単に呼び出せるようにした仕組みのこと。

@snapend

+++

@snap[west]

だめ
ローカルインストールしたパッケージでも、
npm scriptsに記述するコマンドは、
グローバルインストールと同じコマンドで
パッケージを実行することができる！

@snapend

---

@snap[west]

だめ
例えば、scriptフィールドに下記のように記述する。
@color[orange](@fa[pen]) @size[0.8em](`"scripts":{"hello":"echo \"Hello World!\""}`)
@color[white](a)
下記のコマンドで実行する。
@color[orange](@fa[pen]) `npm run 〇〇〇←タスク名`
（上記の例の場合は、タスク名は"hello"）

@snapend

---

@snap[west]

@size[1.5em](npx)とは…
@color[white](a)
npm scriptを@color[red](使用せずに)、ローカルで
インストールしたコマンドを実行できる。
npmの5.2.0から同梱されるようになったコマンド。
"node_modules/.bin"のパッケージが直接実行可能。

@snapend

---

@snap[west]

・通常の場合（例）
@color[orange](@fa[pen]) node ./node_modules/.bin/webpack
@color[white](a)
・npxを使う場合（例）
@color[orange](@fa[pen]) npx webpack@color[white](aaaaあああ)→ めっちゃシンプル！

@snapend

---

@snap[west]

グローバル環境がきたなくなったり、
手動でpackage.jsonのscriptに書き込んだり、
面倒なことをしなくてもよくなる @color[orange](@fa[hand-holding-heart])

@snapend

---

@snap[west]

@size[1.5em](yarn)とは…
@color[white](a)
npmと同じくNode.jsのパッケージを効率よく
管理する便利なツールのこと。
FaceBookがGoogle等と協力して2016年に公開。
npmと@color[red](互換性がある)ため似たような感覚で使える。

@snapend

---

@snap[west]

yarnを使うためには？
@color[white](a)
・専用のインストーラからダウンロードする
・ScoopやHomebrewからインストールする
・npmからインストールする

@snapend

---

@snap[west]

npmとyarnの違い
@color[white](a)
とにかく@size[1.5em](速い)！ 安心で@size[1.5em](安全)！ 高い@size[1.5em](信頼性)！

@snapend

---

@snap[west]

@color[orange](@fa[splotch]) とにかく速い！
@color[white](a)
yarnは、キャッシュサーバを持っているため、
同一パッケージの2回目以降のインストールが速い。
さらに、タスクを@color[red](並行して実行できる)ため、
パフォーマンスの向上につながっている。

@snapend

+++

@snap[west]

キャッシュがあるおかげで、オフラインでも
インストールが可能。
また、ネットワークの接続に失敗した時は、
自動でリトライしてくれる。

@snapend

---

@snap[west]

@color[orange](@fa[splotch]) 安心で安全！
@color[white](a)
yarnは、コードが実行される前に
@color[red](チェックサム)（誤り検出符号）を使用し、
各パッケージが改ざんされていないかを確認する。
正しいライブラリのみコードの実行が行われる。

@snapend

---

@snap[west]

@color[orange](@fa[splotch]) 高い信頼性！
@color[white](a)
npmでいうshrinkwrapに相当する@color[red](yarn.lock)と
いうファイルによって、インストールした
nodeモジュールのバージョンを固定してくれる。
これを共有すれば、どこでも同じ環境を構築できる。

@snapend

+++

@snap[west]

yarn.lockとは…
@color[white](a)
yarnでパッケージのインストールすると、
自動で生成されるファイルのこと。
パッケージの厳密なバージョン情報が記載されていて
各モジュールがソートされており構成管理が簡単。

@snapend

---

@snap[west]

他にも利点を挙げるなら…
@color[white](a)
・npmと互換性があるため、コマンドが似てたり
　同じpackage.jsonを使用できること。
・複数ある同じパッケージを、1つのインデックスに
　まとめることでインストールする数を減らし、
@color[white](aa)ディスク容量の軽減ができること。
  
@snapend

---

@snap[west]

個人的な感想
@color[white](a)
インストールの速度は環境にもよると思うが、
安全性などの面をみると…
npmより、yarnのほうが魅力があったので、
これからはyarnを使っていこうと思ったヨ @color[orange](@fa[hand-holding-heart])

@snapend

---

@snap[west]

おわります。

@snapend

---
