Q16.[Network+Forensic]HTTP Traffic
100pt
## 問題文
HTTPはWebページを閲覧する時に使われるネットワークプロトコルである。
ここに、とあるWebページを見た時のパケットキャプチャファイルがある。
このファイルから、見ていたページを復元して欲しい。

## 作業環境
Mac OS BigSur 11.6.4

## 知識
パケットキャプチャファイルの拡張子は`pcap`

パケットキャプチャファイルから見ていたWebサイトを復元できることを初めて知った．

## writeup
Wiresharkで開き，File -> Export Objects -> HTTP

さらにフォルダ構成も再現してやる必要がある．csフォルダとjsフォルダを作り，それぞれにcs/lsファイルを移動させた．また，network100, network100(2)には拡張子がなかったため，`.html`を加えたところ成功した．

