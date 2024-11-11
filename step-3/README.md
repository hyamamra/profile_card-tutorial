# `class`を使ってみよう

`index.html`の11行目の`<div>`タグに`class`属性を追加してみましょう。

```html
<body>
  <div class="card">
    <div>
```

`style.css`の最後に以下のスタイルを追加してみましょう。

```css
.card {
  /* カードの大きさを指定 */
  width: 50vh;
  height: 30vh;
  /* カードの余白を指定 */
  padding: 4vh;
  /* カードの背景色を指定 */
  background-color: khaki;
  /* カードの角丸を指定 */
  border-radius: 1vh;
  /* カードの影を指定 */
  box-shadow: 0 4vh 2vh rgba(0, 0, 0, 0.2);
}
```
