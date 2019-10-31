# denoとは

* 公式: https://github.com/denoland/deno
* 読み方は ディノ または デノ
* 恐竜を意味する ダイナソー と似た発音から マスコットは恐竜 ということらしい
* node.jsの失敗を元に 次世代 javascript 実行エンジンとして開発されている
* もともとは Typescript の実行エンジンとして開発されたぽいが、後にjavascript も実行可能に

## denoの特徴

* npmモジュールを利用せず、git等のURL指定でモジュールを利用できる
* package.jsonによるモジュール管理の廃止
* denoを実行する際に、ファイルやネットワークアクセスに対して制限を設けることができる

例えば、denoで実行するTypescriptに環境変数へのアクセスを許可する場合は以下のようになる

```
$ deno script.ts --allow-env
```

### 実行エンジン
内部で利用している javascript 実行エンジンにはV8を利用

* V8 は Googleが開発したオープンソースな実行エンジン
* Google chrome や node.js でも内部で利用されている

### 言語

* TypeScript (63.1%)

javascriptのコードをC++のstringとしてV8にわたすことでjavascriptが実行されるため、以下の言語の実装もある

* Rust (27.4%)
* C++ (3.6%)


## denoはプロダクションに使えるか

作者のRyan氏曰くまだ実戦投入はできないとのこと。。。


