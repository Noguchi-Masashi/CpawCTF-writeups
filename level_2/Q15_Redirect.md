Q15.[Web] Redirect
100pt
## 問題文
このURLにアクセスすると、他のページにリダイレクトされてしまうらしい。
果たしてリダイレクトはどのようにされているのだろうか…
http://q15.ctf.cpaw.site

※この問題のサーバへの攻撃はお止め下さい

## 作業環境
Mac OS BigSur 11.6.4
ブラウザ：Chrome

## 知識
リダイレクトとは、WebサイトやページのURLを変更した際、古いURLにアクセスしたユーザーを自動的に新しいURLに転送すること．

## writeup
その他のツール -> デベロッパーツール -> Network を開き，「http://q15.ctf.cpaw.site」のリンクを踏む．

このとき，q15.ctf.cpaw.siteのResponse Headers の中にフラグがあった．