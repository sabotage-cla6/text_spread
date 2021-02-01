# text_spread

MarkDownエディタなどによって、文書ファイルはテキストベースが普及してきました。
しかし、表計算に関してはCSVやTSV以外にテキストベースのフォーマットが存在せず、
書式情報を持ったいたり、関数の使える表*計算* のできるテキストベースのフォーマットというものが存在しない、
または、普及していない状況です。

そのため、テキストベースの表 *計算* のフォーマットの策定、編集ソフトの開発を目指します。

## 要件

- 書式情報の設定・保持ができる
- 関数の設定・保持ができる
- テキストベースでの記録される
- テキストベースで編集できる
- 表ベースで編集ができる
- Githubのmdファイルに埋め込める
- Qiitaに埋め込める
- mdファイルに埋め込むことで、JavaScriptによって処理され、表計算として機能する
- mdファイルへの外部ファイルの埋め込みとして機能する

## 記録形式

Markdownの箇条書きと同様の形式

以下現在の想定


```
<extable>
- columns
-- col1
--- width:20px
--- background-color:#cccccc
-- col2
--- column format
- column_format
-- col1
--- background_color:#eeeeee
--- font-weight:bold
- datarows
-- datarow
--- col1
---- value: aaa
---- color: #ff0000
--- col2
---- value: aaa
---- color: #ff0000
</extable>
```


- columns
-- col1
--- width:20px
--- background-color:#cccccc
-- col2
--- column format
- column_format
-- col1
--- background_color:#eeeeee
--- font-weight:bold
- datarows
-- datarow
--- col1
---- value: aaa
---- color: #ff0000
--- col2
---- value: aaa
---- color: #ff0000
