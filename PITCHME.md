## PackageManagers

---

@snap[west]

パッケージ管理ツールとは…

@color[white](a)

ソフトウェアのインストールやアンインストール、

アップデートなどができるツールのこと。

@color[red](ソフトウェア同士の依存関係)も管理できるのです。

@snapend

+++

@snap[west]

Aパッケージをインストールするのに、

Bパッケージが先に入っていることが条件な場合 @color[blue](@fa[frown])

@color[white](a)

@fa[arrow-right] 自動的にインストールをしてくれる @color[orange](@fa[laugh-beam])

@snapend

+++

@snap[west]

CパッケージとDパッケージは

同時にインストールしてはいけない場合 @color[blue](@fa[frown])

@color[white](a)

@fa[arrow-right] 警告を出してダメということを教えてくれる @color[orange](@fa[laugh-beam])

@snapend

---

@snap[west]

パッケージとは…

@color[white](a)

ソフトウェアを構成する様々なファイルや@color[red](追加情報)、

そのソフトウェアが正しく動作するための命令などが

書かれているファイルをまとめた書庫のようなもの

@snapend

+++

@snap[west]

追加情報 = メタデータと呼ばれる

@color[white](a)

- 概要
- 説明文
- パッケージに含まれているファイルの一覧
- ソフトウェアのバージョン情報とリリース番号
- 構築日時と場所、構築者に関する情報
- 対応するアーキテクチャ
- 含まれるソフトウェアのライセンス情報
- その他

@snapend

---

@snap[west]

@size[1.5em](npm)とは…

@color[white](a)

@color[orange](Node Package Manager)の略。

Node.jsのパッケージを管理するツールのこと。

@snapend

---

@snap[west]

npmを使う

@color[white](a)

Node.jsをインストールすれば、

npmも自動的にインストールされ使えるようになる

@snapend

---

@snap[west]

background:white

npmを使う

@color[white](a)

Node.jsのインストールが完了したら、

npmもちゃんとインストールされてるかを確認する

バージョンが表示されたらOK

@color[white](a)

確認コマンド @fa[arrow-right] 

```

npm -v

```

@snapend

---

### 指定したコードだけハイライト表示


```
var str1 = 'hello world';
var flag = true;
var result = 10 + 20;


console.log( str1 );
console.log( str2 );
console.log( str3 );
```
@[2](flagに「true」を代入)


---


コマンド

---

代表的なパッケージ例

---

使い方

---
