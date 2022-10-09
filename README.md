# add-dakuten（濁点付与）

- VSCodeで、選択された文字列に濁点を付与する拡張機能
    - 「え」→「え゙」みたいな、本来濁点が付かない文字に付与することを想定

## 機能

- **選択文字列に対し、設定で選択された濁点を付与**
    - 実行方法
        - コマンドパレットから「濁点の付与／除去」を選択
            - デフォルトではショートカットキーを設定していません
        - 文字列選択時、右クリックから「濁点の付与／除去」を選択
        - 文字列選択時、右上に出るロゴをクリック
- **文字列内に既に濁点が存在する場合、文字列内の濁点を除去**
    - 二重に濁点が付与されてしまうことを防ぐ

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
### 0.0.2
ロゴ画像を追加
