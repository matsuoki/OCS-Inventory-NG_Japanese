ocsreports_japanese localization
----
# 概要

[OCS Inventory NG](http://www.ocsinventory-ng.org/en/ "OCS Inventory NG") の管理画面で日本語を使えるようにするローカライゼーションファイルです。

* [OCS Inventory NG](http://www.ocsinventory-ng.org/ "")

# インストール
ocsreposts/plugins のディレクトリで下記のファイルを作成・編集します。
 
* language/lang_config.txt の上書き(日本語エントリの追加）
* language/japansese の作成
* language/japansese/japanese./txt の作成
* language/japansese.png の作成

ocsreposts/plugins  は /usr/share/ocsinventory-reports/ocsreports/plugins/ あたりに有ります（FreeBSDの場合） 


# 既知の問題
mb_strtoupper がマルチバイト環境でうまく動かない（mb_strtoupper("あいうえお")=""になる）バグが有ります。
このバグの影響で下記の事象が発生します。

* ローカライズを行ったタブの一部が表示されない
* ソフトウェア一覧でのソフトウェアの頭文字が表示されない、

[launchpad](https://launchpad.net/ocsinventory-ocsreports "launchpad.net") でも順次修正が行われていますが、対応が十分ではありません。

