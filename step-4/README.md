# レイアウトを整えてカードを完成させよう

`index.html`の12行目、14行目、18行目の`<div>`タグに`class`属性を追加しましょう。

```html
    <div class="header">
      <img src="../image.webp" alt="プロフィール画像">
      <div class="info">
        <h1>名前</h1>
      </div>
    </div>
    <div class="about">
      <p>自己紹介文</p>
```

`style.css`の最後に以下のスタイルを追加しましょう。

```css
.header {
  /* 写真と名前部分を隣に配置 */
  display: flex;
  align-items: center;
}

.info {
  /* 写真と名前部分に余白を指定 */
  margin-left: 3vh;
}

.about {
  /* 自己紹介文とヘッダー部分のあいだに余白を指定 */
  margin-top: 4vh;
}
```
おつかれさまでした！
最後に自己紹介文を書いてカードを完成させましょう。
