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

