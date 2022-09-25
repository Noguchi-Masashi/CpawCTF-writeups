## 問題文
このファイルを開きたいが拡張子がないので、どのような種類のファイルで、どのアプリケーションで開けば良いかわからない。
どうにかして、この拡張子がないこのファイルの種類を特定し、どのアプリケーションで開くか調べてくれ。

## 作業環境
Mac OS BigSur 11.6.4

## writeup
``` bash
$ file <file name>
```
fileコマンド実行後，対象ファイルの情報が出力される．

その中に `Name of Creating Application: Microsoft Office Word` と表示があり，Microsoft Office Wordで開けると分かった．

### その他
自分の作業環境の場合，Finderでどのアプリケーションで開くか指定せずに単に「開く」で自動的に Microsoft Word で開くこともできた．