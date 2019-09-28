# SQL
Group by → where →select →　order byの順に処理される

縦持ちのデータを横持にしたい場合
From句に元となる縦持ちテーブルをサブクエリで作成
Select句でCase句を用いて、Sum(Case…）とすることで横持にできる。この場合のSumは合計をしたいのではなく、決まりとして覚えておくほうがいい

オプティマイザーとは？
SQLにはオプティマイザーという存在がいる。これはクライアントからSQLを投げられたときにサーバー側にいる存在で、SQLリクエストをDBになげ、どのように処理を行えば最小手でデータをとれるかを考えている。最小手とは、メモリの仕様、ディスクへのアクセス回数、処理速度などがそれにあたる。オプティマイザーはPosgre、MySQLなどSQLの種類ごとに存在する。Oracleの場合はオプティマイザーが複数あったりする
