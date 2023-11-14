## はじめに

※このREADMEは制作中ですので、途中で文章が変更される可能性があります。予めご了承ください。

## TODOリスト

- こちらはTODOの新規作成、表示、編集、削除ができます。
- 予めMySQLに直接SQL文を記述してユーザーを追加しています。

## 機能

- **ログイン、ログアウト機能**
- **CRUD機能**
  - TODOの作成
  - TODOの表示
  - TODOの編集
  - TODOの削除

## 使い方

- **ログイン**
  - 最初はログイン画面のページが出るので、ユーザー名とパスワードを入れてログインする。
  - ログインが成功したら、TODOを作成、今まで作ったTODOを表示するページが表示されます。
  - **ログインせずにTODO作成、編集ページに移動できないようにルーティングを変更しています。**

- **TODOの作成(追加)**
  - 上部に2つのテキストボックスがあって、上から順番にTODOの名前、内容を入力するテキストボックスです。
  - TODO名と内容を書いて、テキストボックスの下にある追加ボタンを押すとページの一番下にTODOが追加されます。
  - **TODO名は上限25文字、TODOの内容は上限50文字にしています。上限を超えて文字を入力して追加や空白のまま追加すると、TODOは追加されずに追加ボタンの下にエラーメッセージが表示されます。**

- **完了、編集、削除ボタン**
  - TODOの右側にある3つのボタンはTODOの完了と編集と削除のボタンです。
  - 緑色の完了ボタンを押すと、背景色が緑色に変更されます。もう一度押すと元の背景色に変更されます。
  - 青色の編集ボタンを押すと、TODOの編集ページに移動します。
    - TODO名と内容の文章を編集し確定ボタンを押すと、TOODが変更されてTODO作成ページに戻ります。
    - 戻るボタンを押すと、確認ダイアログが表示されてOKを押すと、何も変更されずにTODO作成ページに戻ります。
  - 赤色の削除ボタンを押すと、確認ダイアログが表示されてOKを押すと、TODOを削除します。

- **ログアウト**
  - ログアウトボタンを押すと、確認ダイアログが表示されてOKを押すと、ログインページに戻ります。

## 使用した技術

- **言語**
  - PHP
  - SQL

- **データベース**
  - MySQL

- **フレームワーク**
  - Laravel(Breeze)
  - Tailwind CSS

- **その他**
  - XAMPP

## 学習や制作に参考にしたサイトや書籍

- [**Progate**](https://prog-8.com)

  - PHPとSQLの学習に使用したサイトです。PHPとSQLは全てのコースを学習しました。

- [**気づけばプロ並みPHP 改訂版--ゼロから作れる人になる!**](https://amzn.asia/d/dZYudsm)

  - 書籍を参考にして簡単なショッピングサイトをPHPとSQL、XAMPPを使って制作しました。

- [**3ステップでしっかり学ぶ PHP入門**](https://amzn.asia/d/7e3Nypq)

  - progateと上記の書籍を学習した後にPHPの復習として使用しました。

- [**Laravelの教科書(学習サイトのみ)**](https://textpro.addisteria.com/home)

  - Laravelの学習とBreezeの導入などに使用しました。

- [**【Laravel10】breezeでメール認証をテキスト認証に変更する**](https://qiita.com/yukisku/items/d4f77f378f223937473c)

  - breezeはメールアドレスとパスワードで認証するので、メールアドレスではなく、ユーザー名で認証できるように参考にしました。

- [**【Laravel】Bladeで@ifではなく三項演算子を使う**](https://qiita.com/shonansurvivors/items/1e3194cf3eb2ea089039)

  - TODOを完了したときに緑色のボタンを押しときDBのdoneの値が切り替わるのに、背景色が変更されなかったので参考にしました。

## 学習期間

- 2023年8月中旬 ～ 8月末　：Progate(PHP)
- 2023年9月初め ～ 9月下旬：上記2冊の書籍
- 2023年9月下旬 ～ 9月末　：Progate(SQL)とLaravel

## 制作期間

- 2023年10月初め ～ 2023年10月末

  - 完成予定は約2週間と思っていましたが、長く掛かってしまいました。

## なぜ制作期間が長くなったのか

1. 学習ペースを急ぎすぎて、書籍や学習サイトで言語やシステムの設定や機能などを一度だけざっと学習し、すぐに次の内容に進んでしまった。
2. その結果、PHPやSQL、Laravelの設定や機能について十分に理解ができていなかった。
3. 分からない箇所が出てきた際には、自分で検索するよりもChatAIに頼りすぎてしまった。
4. 必要な情報や不明点を主体的に検索して発見するスキルが不足していた。

## 反省点
- **学習面**
  - 学習する際は、理解が得られるまで参考書や問題集を繰り返し読んだり解いたりするように心がける。
  - 自主的に検索する癖を身につけ、必要な情報をすぐに検索して見つけるスキルを向上させる。
- **ChatAI**
  - 今回の制作で現在のChatAIは平気で嘘をつくと実感した。
  - ChatAIを使用する際は、文章の校正や本当に分からない時のみ利用する。
- **制作面** 
  - 制作期間が長引いたため、本来実装する予定だった以下の機能を追加できませんでした。
    - 検索機能
    - TODOの共有(TODOを追加、編集したユーザーを表示させる)
  - 動画形式で紹介するのではなく、レンタルサーバーやPaasなどにデプロイさせてWEBサイトで表示させたかった。
    - レンタルサーバーなどのサーバー、データベースの利用にかかる費用を支払う余裕がなかったため、適切な環境を構築することが難しかった。
    - 自分の技術力がまだ向上途中で、適切なデプロイが難しかった。
 
## 最後に

学習期間はまだ短いですが、IT業界への就職を目指し、言語やシステムなどを着実に理解し、新しいプロジェクトにも挑戦していきたいと考えています。よろしくお願いいたします。

## ライセンス (License)

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).