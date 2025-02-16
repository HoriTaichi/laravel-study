## 概要
このリポジトリはlaravelの勉強プロジェクトです。

## Larastan
Larastanとは、Laravelに特化した静的解析ツールです。
LarastanはPHPの静的解析ツールであるPHPStanをベースにしており、Laravelのコードに特化したルールを追加しています。

- phpstan.neonについて
https://phpstan.org/config-reference　を参考に。

実行
```
./vendor/bin/phpstan analyse
```
  [OK] No errors  になったらOKです。

静的解析ツール
1. 文法チェック
2. 型の検証
3. 未使用コードの検出
4. 潜在的なバグの検出
5. セキュリティの問題の検出
=> SQLインジェクション、クロスサイトスクリプティングなどを検出できる場合もある。ここ大事。
6. パフォーマンスの最適化
7. Laravel固有のチェック

参考：https://qiita.com/aosan/items/420e339d4b5941aac048#51-larastan%E3%81%A8%E3%81%AF

## Laravel Debugbar
Laravel Debugbarは、デバッグ情報をブラウザ上に表示するツールで、SQLクエリやビュー、リクエストの情報などをリアルタイムで確認できる

参考：https://www.itsolutionstuff.com/post/laravel-11-install-and-configure-laravel-debugbarexample.html


## PHP CS Fixer
コードスタイルを整えてくれるツールです。
プロジェクト内で一貫したコードスタイルを保つために非常に有用で、コードの可読性や保守性が向上します。PSR-2やPSR-12などの標準に基づいてコードを整形できます。

```
./vendor/bin/php-cs-fixer fix app --config=.php-cs-fixer.dist.php
```

自動的にするには、
.git/hooksに『pre-commit』を作成し、php-cs-fixer を実行するコマンドを記述すればOK。

