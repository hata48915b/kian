<!-- Time-stamp:   <2024.12.18-07:16:52-JST> -->

# kianマクロ

## 概要

TeX（pLaTeX）で日本語の公用文書を書くためのスタイルファイルです。

## 動作環境

pLaTeX2e/upLaTeX2e

## インストール方法

ZIPファイルの中の「kian」を適切な場所に移動させ，
必要であれば，「mktexlsr」又は「texhash」を実行するだけです。

### Windowsの場合

解凍したフォルダ内の「kian」フォルダを，適切なフォルダ
（「C:\texlive\texmf-local\tex\platex」や
「C:\w32tex\share\texmf-dist\tex\platex」等）に移動させ，
必要であれば，コマンドプロンプトで
「mktexlsr」又は「texhash」を実行してください。

TeX Liveをお使いの場合は，
インストーラー「INSTALL-windows.dat」を用意しました。
ただし，TeX Live 2015（Windows 10）環境でしかテストしておりませんので，
ある程度の知識をお持ち方は，手動インストールを強くお勧めします。

### Macintosh，FreeBSD，Linuxの場合

解凍したディレクトリ内の「kian」ディレクトリを，適切なディレクトリ
（「/usr/share/texlive/texmf-dist/tex/platex/」や
「/usr/local/texlive/texmf-local/tex/latex/」等）に移動させ，
必要であれば，ターミナルで
「sudo mktexlsr」又は「sudo texhash」を実行してください。

手動インストールが困難な方のために，
インストーラー「INSTALL-unixlike.sh」を用意しました。
「sudo sh INSTALL-unixlike.sh」と実行してください。
ただし，十分なテストができておりませんので，
ある程度の知識をお持ち方は，手動インストールを強くお勧めします。
また，TeXのディレクトリ構成がOSやディストリビューションによって，
様々であるため，うまく機能しない可能性があります。

## アンインストール方法

### Windowsの場合

インストールした「kian」フォルダを削除し，
必要であれば，コマンドプロンプトで「mktexlsr」又は「texhash」を実行する。

### Macintosh，FreeBSD，Linuxの場合

インストールした「kian」ディレクトリを削除し，
必要であれば，ターミナルで「sudo mktexlsr」又は「sudo texhash」を実行する。

## 使用方法

下記のマニュアルをご覧ください。

[Kianのマニュアルページ](https://raw.githubusercontent.com/hata48915b/kian/refs/heads/main/manual.html)

## 著作権

Copyright © 2016-2024 Seiichiro HATA

## ライセンス

GNU General Public Licenseバージョン3 (GPLv3)又はその後継バージョン

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

## 自己紹介

### 名前

秦　誠一郎（はた　せいいちろう）

### 本業

広島弁護士会所属の弁護士です。

国政法律事務所（広島市中区上八丁堀5番27号アーバンビュー上八丁堀701号）に勤務しています。

### 経歴

#### 広島県立安古市高校

#### 大阪大学理学部物理学科（高エネルギー物理学）

#### 京都大学大学院理学研究科（数理解析研究所）

### 連絡先

[弁護士 秦 誠一郎の公式ページ](https://hata-o.jp/hata48915b/)

[弁護士 秦 誠一郎の連絡先](<mailto:hata48915b@post.nifty.jp>)

## ウェブページ

[ソースコードのページ（github）](https://github.com/hata48915b/kian)

## 免責条項

ライセンスに定められているとおり、本プログラムにより損害が発生したとしても、
著作権者は何らの損害賠償責任も負いませんので、ご注意ください。

作成した文書は、必ず内容を確認し、
意図した内容になっていることを確認したうえで、使用してください。

## ヒストリー

### 2016-10-30 v01(Hiroshima Station)をリリースしました。

- kian-page.styがv01になりました。
- kian-sect.styがv01になりました。
- kian-titl.styがv01になりました。
- kian-opti.styがv01になりました。

### 2017-10-30 v02(Enkobashi-cho)をリリースしました。

- kian-page.styがv02になりました。
    + コードを適正化しました。
    + 強制改行に関するバグを修正しました。
- kian-sect.styがv02になりました。
    + 目次の深さ指定（tocdepth）が効かないバクを修正しました。
    + 目次の題目が長い場合に，点線（dotfill）が消えるバグを修正しました。
    + sectionにオプションを導入しました。
    + 箇条書きの字下げのバグを修正しました。
- kian-titl.styがv02になりました。
    + minutodashを微調整しました。
    + 強制改行に関するバグを修正しました。
    + addressに郵便番号の出力機能を追加しました。
- kian-opti.styがv02になりました。
    + sectionのオプションに対応しました。
    + sectionの表示を微調整しました。

### 2018-11-02 v03(Matoba-cho)をリリースしました。

- kian-page.styがv03になりました。
    + verb関数とverbatim環境での空白の間延びを修正しました。
- kian-sect.styがv03になりました。
    + sectionにlabelが付かないバグを修正しました。
- kian-titl.styがv03になりました。
    + receiverに名前を均等割付けしないオプションを追加しました。
    + sender及びpersonに死亡日の出力機能を追加しました。

### 2019-04-01 v04(Inari-machi)をリリースしました。

- kian-titl.styがv04になりました。
    + 元号「令和」に対応しました。

### 2019-04-26 v05(Kanayama-cho)をリリースしました。

- kian-titl.styがv05になりました。
    + 元号「令和」に追加対応しました。

### 2019-05-29 v06(Ebisu-cho)をリリースしました。

- kian-titl.styがv06になりました。
    + バグを修正しました。

### 2020-06-13 v07(Hatchobori)をリリースしました。

- kian-page.styがv04になりました。
    + stamppagenumber/dontstamppagenumberを追加しました。
    + stampendmark/dontstampendmarkを追加しました。
    + onepageに*オプションを追加しました。
- kian-sect.styがv04になりました。
    + バグを修正しました。
- kian-titl.styがv07になりました。
    + arrangedateが同年，同月，同日に対応しました。
    + バグを修正しました。

### 2021-09-12 v08(Tate-machi)をリリースしました。

- kian-page.styがv05になりました。
    + ページ番号の表示を持続的に設定するStamppagenumber/Dontstamppagenumberを追加しました。
    + 終了マークの表示を設定するStampendmark/Dontstampendmarkを追加しました。
    + onepageに関するバグを修正しました。
- kian-sect.styがv05になりました。
    + itemonkianに関するバグを修正しました。
- kian-titl.styがv08になりました。
    + idcode、idcodes、idcodenumberで年度を指定できるようにしました。
    + idcode、idcodes、idcodenumberに関するバグを修正しました。
    + idcodenumberで事件名も指定できるようにしました。
    + onepageの仕様を大幅に変更しました。後方互換性がないのでご注意ください。
- kian-opti.styがv03になりました。
    + textslbox（斜体）に負の角度を指定できるようにしました。

