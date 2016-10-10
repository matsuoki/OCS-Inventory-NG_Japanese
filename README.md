ocsreports_japanese localization
----


[OCS Inventory NG](http://www.ocsinventory-ng.org/en/ "OCS Inventory NG") の[masterにマージ](https://github.com/OCSInventory-NG/OCSInventory-ocsreports/commit/b0fa015d584458a7a98087f9e8430f4987bc6d70 "commit b0fa015d584458a7a98087f9e8430f4987bc6d70")されました。

[This repository merged](https://github.com/OCSInventory-NG/OCSInventory-ocsreports/commit/b0fa015d584458a7a98087f9e8430f4987bc6d70 "commit b0fa015d584458a7a98087f9e8430f4987bc6d70") to [OCS Inventory NG](http://www.ocsinventory-ng.org/en/ "OCS Inventory NG").

# 概要

[OCS Inventory NG](http://www.ocsinventory-ng.org/en/ "OCS Inventory NG") の管理画面で日本語を使えるようにするローカライゼーションファイルです。

* [OCS Inventory NG](http://www.ocsinventory-ng.org/ "")

# インストール
ocsreposts/plugins のディレクトリで下記のファイルを作成・編集します。
 
* language/lang_config.txt に日本語エントリを追加
* language/japansese/japanese.txt の作成
* language/japansese/japanese.png の作成

ocsreposts/plugins  は /usr/share/ocsinventory-reports/ocsreports/plugins/ あたりに有ります。

# 既知の問題
mb_strtoupper がマルチバイト環境でうまく動かない（mb_strtoupper("あいうえお")が空文字を返す）バグが有ります。
このバグの影響で下記の事象が発生します。

* ローカライズを行ったタブの一部が表示されない
* ソフトウェア一覧でのソフトウェアの頭文字が表示されない、

[launchpad](https://launchpad.net/ocsinventory-ocsreports "launchpad.net") でも順次修正が行われていますが、対応が十分ではありません。


