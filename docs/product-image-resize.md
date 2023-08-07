# 商品詳細ページ splideを使った場合に商品画像が荒れる

`.c-product_img__slider`にsplideが使われているが、規格を選択すると画像がリサイズされ（ファイルパスの最後に`-large`が付く）、画像が荒くなっているように見える。
対策は、規格を選択した時に、パスを上書きする。

```js
  // 規格を選択すると商品画像がサムネイル画像パスになるのでoriginalで上書き
  $(document).on('change', '.input_option_type', function() {
    setTimeout(function(){
      $('.c-product_img__image').each(function(){
        let origin_url = $(this).attr('src').replace(/-large/, '-original');
        $(this).attr('src', origin_url);
      });
    }, 800); // 0.8秒後にすることでecforceのJSより後に実行
  });
```

参照 [jQueryで.changeメソッドが効かなくて困ったこと](https://qiita.com/katsu105/items/774d199bb6bf2bdc945f)