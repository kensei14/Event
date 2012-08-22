メリットとデメリット。

イベントリスナ方式で定義した関数に対して引数を指定する方法。


イベントハンドラとイベントリスナの違い。
http://komitsudo.blog70.fc2.com/blog-entry-116.html


**イベントハンドラ**

書き方

	（html内）input type="button" onclick="sample()"　

	（javascript内）elem.onclick = function() {  ….  }

メリット・デメリット

	簡単に扱える。
	ブラウザの違いをあまり意識する必要がない
	
	HTMLの見た目が汚くなる
	同じ要素に複数のイベントを定義する事が出来ない。
	

**イベントリスナ**

書き方


	elem.addEventListener("click",function() { 
		…. 
	}, fause);
	
メリット・デメリット

	複数のイベントを定義できる。　*定義順に実行される。
	
	ブラウザ対応が必要(IE)