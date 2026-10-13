# X Card Helper — Chrome / Edge 拡張

このリポジトリで配布するのは、X Card Validator を補助するブラウザ拡張 **X Card Helper v1.2.0** です。リポジトリ名は `hatena-publisher` ですが、はてなブログへの記事投稿・更新機能は含まれません。

## ダウンロード

- [X Card Helper v1.2.0（ZIP）](./XCardChatGPTHelper_v1.2.0.zip)
- [拡張機能のソースと詳しい使い方](./XCardChatGPTHelper/README.md)

## Chrome / Edgeへの導入

1. 上記 ZIP をダウンロードし、解凍する。
2. Chrome: `chrome://extensions/` / Edge: `edge://extensions/` を開く。
3. 「デベロッパーモード」を有効にする。
4. 「パッケージ化されていない拡張機能を読み込む」を押し、解凍した `XCardChatGPTHelper` フォルダを選ぶ（`manifest.json` が直下にあるフォルダ）。

既に導入済みの場合は、**現在読み込んでいる拡張フォルダの中身を最新版で上書き**し、拡張の管理画面で「再読み込み」を押してください。別フォルダとして新規登録すると二重に追加される可能性があります。

## 動作（v1.2.0）

- ChatGPTから受け取った記事URLをX Card Validatorに渡し、検証操作を試みます。
- Validatorの成功ログ **`Page fetched successfully`** と **`Card loaded successfully`** の両方を検知すると、固定15秒の待機をせずすぐにタブを閉じます。
- 成功を検知できない場合やエラーの場合、タブは自動では閉じません。
- X側のキャッシュ強制更新を保証するものではありません。

## 権限と注意事項

権限、操作条件、制約、検証範囲の詳細は、[同梱README](./XCardChatGPTHelper/README.md) を参照してください。これはChrome Web Store / Edgeアドオンストアでの配布ではなく、手動インストール用です。

## 配布ファイルの同一性

ZIP の SHA-256:

`873b14a430876ecaa55a6c8c00e1616e4e1edea6d468f30af9922d038b324fcc`
