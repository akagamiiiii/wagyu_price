# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？
リモートリポジトリ  
  ネット上に配置して、複数人で共有するためのリポジトリ。  

ローカルリポジトリ  
 開発者が個人で使用するために自分のPC上に配置するためのリポジトリ。  
  
<br>
<br>
  
## プッシュとマージの違いは何でしょうか？
プッシュ  
  ローカルリポジトリの内容をリモートリポジトリに送り、更新するコマンド。  

マージ  
  ローカルリポジトリ内で、分岐して行った作業を一つに統合するコマンド。  
  複数のブランチを一度に統合することはできない。一つ一つブランチを統合しなければならない。

<br>
<br>

## コミットとプッシュの違い
コミット  
  ローカルリポジトリで行ったそこまでの作業内容を、保存するためのコマンド。  

プッシュ  
  ローカルリポジトリの内容をリモートリポジトリに送り、更新するコマン
  ド。

<br>
<br>

## コミットのメッセージはどのように書いてあげるのが最適でしょうか？
端的に書くのではなく、はっきりとどのような作業をおこなったのかを明記する。  
現場ではプレフィックスと呼ばれるものがよく使用される。  
プレフィックスとは、単語の前に置かれる接頭辞のこと。  
例：int, str, lng等

<br>
<br>

## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？
ローカルでマージする場合、コードをレビューする前にmasterに反映されるので、コードにバグがあっても気づきにくい。  
しかしプルリクエストでマージする場合、プッシュしてレビューをお願いしてからマージするので、コードの確認ができる。

<br>
<br>

## コンフリクトを起こしてしまった場合、どう対処すべきですか？
主に以下3通りのどれかを行う  
1.先にマージされた変更内容を取り込む  
2.後にマージしようとしている変更内容を取り込む  
3.どちらの変更内容も取り込む  

これらのマージ方法では、すべて自分だけで取り込む内容を決めてはならない。  
タスクなどを管理する上長の方や、コンフリクトした対象のタスクの担当者に共有をする。なので、コンフリクト対応の際には、最低2名になる。