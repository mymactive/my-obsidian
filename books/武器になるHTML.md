#programming  #html #frontend #a11y

## 書籍情報

- 出版社 : 技術評論者
- 著者 :  柴田宏仙
- [書籍URL](https://gihyo.jp/book/2022/978-4-297-13132-6)

## メモ

### Chapter2 テキストやリストをマークアップしよう

####  br
 
- 文書上の意味の塊での段落で使うべき
- 単に改行したい時はCSSでやるらしい
- CSSではどうやってやるのだろう？

#### small

- 知らなかった
- 著作権とかで使うのが主な用途とのこと
- small=小さいではなく”サイドコメント”であるというのが文書上の意味

#### time

- これも知らなかった
- 文書上の日時を表現する
- yyyy-MM-dd HH:mm:ss以外の形式を使う時はdatetime属性と一緒に使うこと
	- 例えば2022年1月1日を文書上に表現したいときは下記のコードのように使う

```html
<time datetime="2022-01-1">2022年1月1日</time>
```

#### ol

- type属性でローマ数字やアルファベットが使えるとのこと

#### dl & dt & dd

- これらは知らなかった
- dl = description list
- dt = description list term
- dd = definition of description
- コード例はこんな感じ

```html
<dl>
	<dt>Item 1</dt>
	<dd>Item 1 is ...</dd>
	<dt>Item 2</dt>
	<dd>Item 2 is ...</dd>
<dl/>
```

### Chapter3 リンクやコンテンツを埋め込もう

#### a

- a要素のコンテンツモデルはtransparentらしい
	- これは親要素のコンテンツモデルを引き継ぐとのこと
- rel="nofollow"で管理外のリンクであることを明示的に表せるとのこと