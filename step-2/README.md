# CSSを導入しよう

以下のコードを`style.css`として保存します。

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

`index.html`から`style.css`を読み込むようにしましょう。  
`head`タグ内に以下のコードを追加します。

```html
<link rel="stylesheet" href="style.css">
```
