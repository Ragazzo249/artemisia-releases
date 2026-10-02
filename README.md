# Artemisia

よもぎサーバー(PowerNukkitX)のプラグイン開発用の、Windows 向けデスクトップアプリです。サーバーの起動・停止、プラグインのビルド、git の状態確認、ログの検索を 1 つの画面で行えます。

このリポジトリは**配布専用**です。インストーラーは [Releases](https://github.com/Ragazzo249/artemisia-releases/releases) からダウンロードできます(ソースコードはここにはありません)。

## インストール

1. [Releases](https://github.com/Ragazzo249/artemisia-releases/releases) から最新の `artemisia-setup-<版>.exe` をダウンロードして実行します(管理者権限は不要です)。
2. 署名していないため「Windows によって PC が保護されました」と出ます。「詳細情報」→「実行」で進めてください。
3. 初めて使う場合は設定タブが開きます。サーバーフォルダを選んで「保存して再起動」を押し、「足りないものを導入」を押します。

ダウンロードしたファイルが壊れていないかは、各リリースに載せている SHA-256 と見比べて確かめられます(PowerShell で `Get-FileHash <ファイル>`)。

## 前提

- Windows 10 / 11(64bit)
- Git と GitHub CLI(gh)が入っていて、`gh auth login` で開発用リポジトリを読めるアカウントにログインしていること
