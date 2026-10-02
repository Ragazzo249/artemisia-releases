# Artemisia

よもぎサーバー(PowerNukkitX)のプラグイン開発用の、Windows / Mac 向けデスクトップアプリです。サーバーの起動・停止、プラグインのビルド、git の状態確認、ログの検索を 1 つの画面で行えます。

このリポジトリは**配布専用**です。インストーラーは [Releases](https://github.com/Ragazzo249/artemisia-releases/releases) からダウンロードできます(ソースコードはここにはありません)。

## インストール

### Windows

1. [Releases](https://github.com/Ragazzo249/artemisia-releases/releases) から最新の `artemisia-setup-<版>.exe` をダウンロードして実行します(管理者権限は不要です)。
2. 署名していないため「Windows によって PC が保護されました」と出ます。「詳細情報」→「実行」で進めてください。

### Mac(0.4.0 から)

1. [Releases](https://github.com/Ragazzo249/artemisia-releases/releases) から、お使いの Mac に合うファイルをダウンロードします。
   - Apple Silicon(M1 以降): `artemisia-<版>-mac-arm64.dmg`
   - Intel: `artemisia-<版>-mac-x64.dmg`
2. dmg を開き、Artemisia を「アプリケーション」フォルダへドラッグします。
3. Apple の公証を受けていないため、初回は「開けません」と出ます。「システム設定」→「プライバシーとセキュリティ」の「このまま開く」を押してください。うまくいかない場合は、ターミナルで `xattr -dr com.apple.quarantine /Applications/Artemisia.app` を実行してから開きます。

### 初めて使う場合(共通)

設定タブが開きます。サーバーフォルダを選んで「保存して再起動」を押し、「足りないものを導入」を押します。

ダウンロードしたファイルが壊れていないかは、各リリースに載せている SHA-256 と見比べて確かめられます(Windows は PowerShell で `Get-FileHash <ファイル>`、Mac はターミナルで `shasum -a 256 <ファイル>`)。

## 前提

- Windows 10 / 11(64bit)、または macOS
- Git と GitHub CLI(gh)が入っていて、`gh auth login` で開発用リポジトリを読めるアカウントにログインしていること
