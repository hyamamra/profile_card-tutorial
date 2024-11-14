# CSSファイルを導入しよう

## CSSファイルを作成する
`profile_card`ディレクトリ内に`style.css`を作成し、以下のコードを記入して保存します。

```css
body {
  /* body内の要素を画面中央に配置 */
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  margin: 0;
  /* body内のフォントを指定 */
  font-family: "Yu Gothic", sans-serif;
  font-weight: 500;
  font-size: 1.3vh;
}

img {
  /* 画像の高さの最大値を指定 */
  max-height: 14vh;
}
```

CSSファイルは、HTMLファイルで記述された要素のスタイルを指定するためのファイルです。
背景色や文字色、フォントサイズなどのスタイルを指定することができます。
また、CSSでは、`/*`と`*/`で囲まれた部分はコメントとして扱われ、実行されません。

今回は、`body`要素と`img`要素に対してスタイルを指定しています。

### body内の要素を画面中央に配置
`body`要素はHTML文書全体を表す要素で、子要素となるプロフィールカードを画面中央に配置するために以下のスタイルを指定しています。
```css
body {
  /* 子要素のレイアウトや表示方法を`flex`に指定 */
  display: flex;
  /* 子要素を画面中央に配置（縦方向） */
  align-items: center;
  /* 子要素を画面中央に配置（横方向） */
  justify-content: center;
  /* body要素の高さを画面の高さいっぱいに設定 */
  height: 100vh;
  /* 余白を0に設定 */
  margin: 0;
}
```

- `display: flex;`：子要素のレイアウトや表示方法を`flex`に指定します。`flex`は、子要素を柔軟に配置するためのレイアウト方法です。
- `align-items: center;`：`align-items`は、デフォルトでは`flex`コンテナ内の子要素を縦方向に配置するプロパティで、`center`を指定することで子要素を中央に配置します。
- `justify-content: center;`：`justify-content`は、デフォルトでは`flex`コンテナ内の子要素を横方向に配置するプロパティで、`center`を指定することで子要素を中央に配置します。
- `height: 100vh;`：`vh`はビューポート、つまり画面の表示領域の高さを表す単位で、画面の高さいっぱいに要素を表示するために`100vh`を指定します。百分率のように0～100の値を指定することができ、小数も使用可能です。
- `margin: 0;`：`margin`は要素の外側の余白を指定するプロパティで、`0`を指定することで余白をなくします。

### body内のフォントを指定
`body`要素内のフォントを指定するために以下のスタイルを指定しています。
```css
body {
  /* body内のフォントを指定 */
  font-family: "Yu Gothic", sans-serif;
  /* フォントの太さを指定 */
  font-weight: 500;
  /* フォントサイズを指定 */
  font-size: 1.3vh;
}
```

- `font-family: "Yu Gothic", sans-serif;`：`font-family`はフォントの種類を指定するプロパティで、`"Yu Gothic", sans-serif`を指定することで、`Yu Gothic`（游ゴシック）というフォントを優先して使用し、`Yu Gothic`がインストールされていない場合は代替フォントとして`sans-serif`を使用します。
- `font-weight: 500;`：`font-weight`はフォントの太さを指定するプロパティで、`500`を指定することで、中程度の太さのフォントを使用します。
- `font-size: 1.3vh;`：`font-size`はフォントサイズを指定するプロパティで、`1.3vh`を指定することで、ビューポートの高さに対して1.3倍のフォントサイズを使用します。

### 画像の高さの最大値を指定
`img`要素に対して画像の高さの最大値を指定するために以下のスタイルを指定しています。
```css
img {
  /* 画像の高さの最大値を指定 */
  max-height: 14vh;
}
```

- `max-height: 14vh;`：`max-height`は要素の高さの最大値を指定するプロパティで、`14vh`を指定することで、画像の高さをビューポートの高さに対して14%までに制限します。

## HTMLファイルからCSSファイルを読み込む
`index.html`から`style.css`を読み込むようにしましょう。
`head`タグ内に以下のコードを追加します。

```html
<link rel="stylesheet" href="style.css">
```

`link`要素は外部ファイルを読み込むための要素で、`rel`属性に`stylesheet`、`href`属性にCSSファイルのURLを指定します。

## 最終的なディレクトリ構造
最終的なディレクトリ構造は以下のようになります。

```bash
profile_card
├── image.jpg
├── index.html
└── style.css
```

## ブラウザでHTMLファイルを開く
ブラウザでHTMLファイルを開いて、プロフィールカードの表示を確認しましょう。
すでにブラウザでHTMLファイルを開いている場合は、リロード（再読み込み）して最新の内容を表示します。
画像が画面中央に表示され、フォントやフォントサイズが指定したスタイルになっていることを確認してください。

## お疲れ様でした！
これでCSSファイルを作成し、HTMLファイルに読み込むことができました。
次のステップではさらにCSSを適用し、プロフィールカードにスタイリングを施していきます。

次のステップ: [`class`を使ってみよう](../step-3/README.md)
