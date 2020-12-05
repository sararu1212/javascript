# JavaScriptについての勉強

参考：<u> https://www.kagoya.jp/howto/webhomepage/javascript/</u>

**目次**

<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [JavaScriptについての勉強](#javascriptについての勉強)
    - [勉強項目](#勉強項目)
    - [スケジュール](#スケジュール)
    - [構造](#構造)
    - [JavaScript](#javascript)
      - [関連用語](#関連用語)
      - [JavaScriptでできること](#javascriptでできること)
      - [フレームワーク](#フレームワーク)
      - [コーディング方法](#コーディング方法)

<!-- /code_chunk_output -->

### 勉強項目
* git(ブランチ)について
* githubについて
* markdownについて
<br>

* JavaScriptとは
* (JavaScriptの歴史)
* JavaScriptでできること
* JavaScriptの種類
* コーディング方法
* 作りたいもの(目標)
* 

### スケジュール
* 

### 構造
```plantuml
left to right direction 
actor User as user
cloud  Brouser
database Server

user --> Brouser : webを見たい
user <-- Brouser : webを表示
Brouser --> Server : データちょうだい 
Brouser <-- Server : データあげる
note bottom : JavaScriptファイルを渡す
```

### JavaScript
* 特徴：ブラウザ上で画像を拡大表示して見やすくしたり、入力フォームを設置してメッセージを送付するのを可能にするプログラミング言語
<br>

* 歴史：1990年代に登場し、当初は「**LiveScript**」という名前だったが「**Java**」の普及に便乗し「**JavaScript**」に変更された
<br>

* 使用場面：パソコンやスマホのブラウザ

#### 関連用語
* Ajax
    * 概要：JavaScriptライブラリでXML形式のデータを送受信する
    * 用途：GoogleMapsなど
* jQuery
    * 概要：JavaScriptライブラリで手軽に導入できて人気
    * 用途：メニュー、画面表示、検索など

* JSON
    * 概要：データをテキストで表現するための記述方法

* DOM
    * 概要：HTMLファイルなどにアクセスして操作するしくみ

#### JavaScriptでできること
* マウスの動きに伴うメニューの表示・非表示
* 画像の拡大（ポップアップ）表示
* Google マップ
* 画像スライダー(複数枚の画像を次々と切り替えて表示する機能)
    * 参考サイト：https://startmeup.jp/column/digital/2064/#:~:text=%E3%82%B9%E3%83%A9%E3%82%A4%E3%83%80%E3%83%BC%E3%81%A8%E3%81%AF,%E3%81%AE%E4%BB%95%E6%96%B9%E3%81%AF%E6%A7%98%E3%80%85%E3%81%A7%E3%81%99%E3%80%82
* 送信フォームの必須項目が入力済みかのチェック
* Googleのアクセス分析サービスの利用

#### フレームワーク

* 参考サイト：
    * https://eng-entrance.com/javascript-framework
    * https://www.sejuku.net/blog/70110#:~:text=%E3%83%95%E3%83%AC%E3%83%BC%E3%83%A0%E3%83%AF%E3%83%BC%E3%82%AF%E3%81%A8%E3%81%84%E3%81%86%E5%8D%98%E8%AA%9E%E8%87%AA%E4%BD%93,%E6%A7%8B%E9%80%A0%E5%8C%96%E3%81%99%E3%82%8B%E3%82%8F%E3%81%91%E3%81%A7%E3%81%99%E3%80%82

* 概要：
    * 英語で「枠組み・構造」を意味しており、JavaScriptでWebサービスやアプリを開発するうえで、サーバーとの連携、ルーティング、データの送受信(CRUD)など、全体的な処理の流れを構造化する
* メリット：
    * 作業効率の向上(足りない部分だけを集中して開発すれば良いため)
    * ソースコードの統一性の向上
* デメリット：
    * 習得コストがかかる
    * 複数フレームワークの習得が必要
* 種類：
※**太字**は特に有名かつ重要
    * **AngularJS**
        * 概要：
        * 主な機能：
    * **React.js**
        * 概要：
        * 主な機能：
    * **Vue.js**
        * 概要：
        * 特徴：
    * **jQuery**
        * 概要：
        * 主な機能：
    * Backbone.js
        * 概要：
        * 主な機能：
    * Ember.js
        * 概要：
        * 主な機能：
    * Polaris
        * 概要：
        * 主な機能：
    * Knockout.js
        * 概要：
        * 主な機能：
    * Feathers
        * 概要：
        * 特徴：
    * Meteor.js
        * 概要： 
        * 主な機能：

#### コーディング方法
* [基礎](./coding_basic.md)
* [高層関数](./coding_high_rise.md)

[TOPへ](#javascriptについての勉強)