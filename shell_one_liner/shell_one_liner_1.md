# 1日1問、半年以内に習得 シェル・ワンライナー160本ノック

## 10/28
- bcを使ったワンライナー計算
`echo '1+1' | bc` でechoの出力をbcに入力できる。ほかにもPerlやRubyなどもパイプで入力を受け取られる。
```
$ echo '1+1' | sed 's/.*/echo $((&))/' | bash
$ echo '1+1' | sed 's/^/puts /' | ruby

```

### 'sed'コマンド
- Linux上で文字列を処理するコマンド
- "stream editor"の略で指定したファイルをコマンドに従って処理することができる
- 入力を行単位で読み取り、テキスト変換などの編集をおこない行単位で出力する
- 正規表現に対応している

上で使っているのは「s/置換前文字/置換後文字列/」という方法。`echo '1+1' | ?`という問題からどうやって一行で解答できるかを複数パターン例示している。AtCoderのコードゴルフに使えそう。