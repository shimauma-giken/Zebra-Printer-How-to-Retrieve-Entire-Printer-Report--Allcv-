# Zebra-Printer-How to Retrieve Entire Printer Report (Allcv)
## トラブル時に取得すべきプリンタの設定情報（Allcv版）

トラブル時にまず取得すべき情報と言われるallcvコマンド結果。本ページではWindows PC - Zebra Setup Utilites(以降ZSU) を用いてallcvを取得方法について記載する。

本ページではZSU の入手方法、インストール方法、起動方法については記載しない。また、表示言語を英語にした手順となっていることをご了承頂きたい。

<br><br>

# 対象プリンタ

Zebra Link-OS プリンタ

<br><br>

# 手順

1. ZSU を起動する。
1. [Option] を選択する。
1. [Communication Timeout]を"50"以上の値にし、[OK]を選択。


![](https://supportcommunity.zebra.com/servlet/rtaImage?eid=ka10H000000KOht&feoid=00N0H00000K2Eou&refid=0EM0H0000014zrD)

4. [Open communication with printer]を選択。
1. 下記コマンドを入力する。

    ! U1 getvar "allcv"

    * コマンドの末尾には必ず[Enter/CRLF]を追加すること！！
1. 最終行("")が出力するまで待つ。
1. 取得データをテキストとして保存する場合は、下記図のように[Export all received data]を選択して保存すること。

![](https://supportcommunity.zebra.com/servlet/rtaImage?eid=ka10H000000KOht&feoid=00N0H00000K2Eou&refid=0EM0H0000014ztd)
NOTE Please note that the command must be followed by pressing Enter using the keyboard, otherwise the process will not work.


