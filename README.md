# add-dakuten（濁点付与）

選択された文字列に濁点を付与する拡張機能

## 機能

選択文字列に対し、設定で選択された濁点を付与

## 設定

- `add-dakuten.selector`
    - 濁点の種類を選択
        - 全角濁点（U+309B）
        - 半角濁点（U+FF9E）
        - 結合文字（U+3099）デフォルト
- `add-dakuten.cursor`
    - 選択文字列の変換後、選択を解除して、選択範囲の末尾にカーソルを動かす（デフォルト有効）

## 既知の不具合（？）

- 半濁音「゜」には非対応
    - あまり見かけないので、不要かと思って実装せず
    - 簡単に実装できるため、要望があれば実装します
- コマンドを実行する度にユーザー設定を参照している
    - 設定をよく変える人からすれば、むしろ利点かも
        - （設定変更の度にテキストエディタを再起動しなくて済む）
    - こまめに設定を弄らない人からすれば無駄な処理

## Release Notes
### 0.0.1
リリース

---

## Working with Markdown

You can author your README using Visual Studio Code.  Here are some useful editor keyboard shortcuts:

* Split the editor (`Cmd+\` on macOS or `Ctrl+\` on Windows and Linux)
* Toggle preview (`Shift+Cmd+V` on macOS or `Shift+Ctrl+V` on Windows and Linux)
* Press `Ctrl+Space` (Windows, Linux, macOS) to see a list of Markdown snippets

## For more information

* [Visual Studio Code's Markdown Support](http://code.visualstudio.com/docs/languages/markdown)
* [Markdown Syntax Reference](https://help.github.com/articles/markdown-basics/)

**Enjoy!**
