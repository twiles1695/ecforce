# テーマセットアップ

デフォルトのテーマを一括で修正することで効率的にコーディングします。
慣れれば20〜30分ほどで完了します。

## theme_customize.cssの修正

### 修正対象ファイル
`ec_force/assets/theme_customize.css`

### セットアップ事項
- テーマカラー
- フォント
- ボタン

### カラー
フォントカラー一括置換します。

### フォント
Noto Sans JPを使用することが多いため、最初に@importで読み込みます。

### テンプレート

```css
@import url("https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@100;200;300;400;500;600;700;800;900&display=swap");

.u-text--head {
  color: #000000 !important;
  font-size: 25px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-color--head {
  color: #000000 !important;
}
.u-text--subhead {
  color: #000000 !important;
  font-size: 16px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-text--body {
  color: #000000 !important;
  font-size: 14px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-text--strong {
  color: #000000 !important;
  font-size: 14px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-text--link {
  color: #386f81 !important;
  font-size: 14px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-text--head--overlay {
  color: #ffffff !important;
  font-size: 25px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-text--subhead--overlay {
  color: #ffffff !important;
  font-size: 16px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-text--body--overlay {
  color: #ffffff !important;
  font-size: 14px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-text--color--overlay {
  color: #ffffff !important;
}
.u-color__btn--bg {
  background: #386f81 !important;
}
.u-color__btn--bg--overlay {
  background: #386f81 !important;
}
.u-color__btn {
  color: #386f81 !important;
}
.u-text--btn {
  color: #ffffff !important;
  font-size: 14px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-text--btn--overlay {
  color: #ffffff !important;
  font-size: 14px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-color__btn--text {
  color: #ffffff !important;
}
.u-color__btn--text--bg {
  background: #ffffff !important;
}
.u-text--input {
  color: #000000 !important;
  font-size: 14px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-color--input {
  color: #000000 !important;
}
.u-color__input--bg {
  background: #ffffff !important;
}
.u-color__border--input {
  border-color: #bdc1c2 !important;
}
.u-color__bg--base {
  background: #ffffff !important;
}
.u-color__bg--main {
  background: #ffffff !important;
}
.u-color__border--border {
  border-color: #d8dddf !important;
}
.u-color__border--main {
  border-color: #d8dddf !important;
}
.u-font--head {
  font-size: 25px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-font--subhead {
  font-size: 16px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-font--body {
  font-size: 14px !important;
  font-family: "Noto Sans JP", "游ゴシック体", "Yu Gothic", YuGothic,
    "ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo,
    "MS Pゴシック", "MS PGothic", sans-serif;
}
.u-font--bold {
  font-weight: bold;
}
.c-product_item__actions .c-product_item__form--cart {
  display: none;
}

/*================ Fonts ================*/

/*================ Headings ================*/
h1,
.h1,
h2,
.h2,
h3,
.h3,
h4,
.h4,
h5,
.h5,
h6,
.h6 {
  font-family: "游ゴシック", serif;
}

/*================ Variables ================*/
:root {
  --color-text-head: #000000;
  --color-text-body: #000000;
  --color-text-overlay: #ffffff;
  --color-text-link: #386f81;
  --color-btn-bg: #386f81;
  --color-btn-text: #ffffff;
  --color-input-text: #000000;
  --color-input-border: #bdc1c2;
  --color-page-bg: #ffffff;
  --color-page-border: #d8dddf;

  --font-size-text-head: 25px;
  --font-size-text-subhead: 16px;
  --font-size-text-body: 14px;
  --font-size-text-link: 14px;
}

.c-steps_to_order--theme {
  --theme-color: var(--color-btn-bg) !important;
  --text-color: var(--color-btn-text) !important;
}

.p-movie--theme {
  --theme-color: var(--color-btn-bg);
}

```




## util.cssの修正

### 修正対象ファイル
`ec_force/assets/util.css`

### フラッシュメッセージカラー修正
フラッシュメッセージの背景がデフォルトで淡い水色（#F4F8FA）のため、グレー色に一括置換します。


## 留意点

`theme_customize.css`と`util.css`はキャッシュにより反映が遅い時があります。その場合は数分置いて確認します。