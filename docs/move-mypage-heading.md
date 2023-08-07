# マイページの見出しをヘッダーの直下に移動

```css
/*================ Mypage ================*/
.p-account__inner__content__title {
  justify-content: center;
  margin-top: 100px;
  margin-bottom: 80px;
  font-weight; bold;
}
@media screen and (max-width: 719px) {
  .p-account__inner__content__title {
    margin-top: 50px;
    margin-bottom: 45px;
  }
}

```

```js
$(function(){

  // Move mypage header
  let mypage_header = $('.p-account__inner__content__title, .p-list_header__inner__title');
  if(mypage_header.length > 0){

    mypage_header.clone().prependTo('main');
    mypage_header.remove();
  }

});
```