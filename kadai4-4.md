## 自動販売機（オブジェクト、DOM、イベント処理）のミニレポート
### Q4-1. Itemクラスのメソッドについて説明せよ。
* showItemListがクラスメソッドである理由を考察せよ。
  *すべての商品情報を表示する関数であるため、インスタンスに依存しないことが理由と考えられる。
* buyItemがインスタンスメソッドである理由を考察せよ。
　*特定の商品を購入した際にその商品の在庫を減らす処理をする関数であるため、インスタンスに依存していることが理由と考えられえる。
### Q4-2. 商品の購入ボタンをクリックすると、どのような処理でセルの値が減少するか説明せよ。
* 購入された商品の在庫数のセルをどのようにして特定するのか説明せよ。
  *在庫用のエレメントの抽出をconst itemStock=document.getElementById(`itemstock${this.id}`)で行う。　　商品表の在庫数を指すidを"itemstock${item_list[i].id}"にしておく。
* 特定したセルの値をどのように変更するのか説明せよ。
  *itemStock.textContent=this.stock;でセルの数値を最新の在庫数の値に変更する。
### Q4-3. 感想
* 今回の課題で苦労したこと
  *購入ボタンをクリックしたときのイベント処理が上手くできかったので、ボタン押しても購入処理が行われなくて苦労した。
* 演習を通して理解できたこと
　* DOMの基本的な操作。なかでもノードを取得するgetElementByIdメソッドは良く使ったので理解できた。
* この自動販売機プログラムの追加機能や課題など
　*追加機能として考えられるのは在庫数が0になったらそのボタンを非表示にするか、押せないようにプログラムを修正する 
