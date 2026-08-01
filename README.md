# 紙どこ 公式ページ

iOSアプリ「紙どこ」の公式 GitHub Pages 用ファイル一式。
Jekyll の Cayman テーマをベースに、ウォーム配色のカスタム CSS で装飾しています。

## ページ構成

| URL | ファイル | 用途 |
|---|---|---|
| `/` | `index.md` | アプリ紹介・使い方 |
| `/support.html` | `support.md` | サポート・FAQ（ASC Support URL） |
| `/privacy.html` | `privacy.md` | プライバシーポリシー（ASC Privacy URL） |
| `/share/` | `share/index.html` | 招待リンク中継ページ（kamidoko-app:// 自動転送） |

## 公開 URL（2026-06-21〜 専用アカウント・user-page repo）

- アプリ紹介: <https://kamidoko.github.io/>
- サポート: <https://kamidoko.github.io/support.html>
- プライバシーポリシー: <https://kamidoko.github.io/privacy.html>
- 共有招待中継: <https://kamidoko.github.io/share/>

旧 URL（`bobshiro.github.io/kamidoko/...`）も後方互換のため当面稼働中。

## ファイル

- `index.md` — アプリ紹介・使い方トップページ
- `support.md` — サポート・FAQ ページ
- `privacy.md` — プライバシーポリシー本文
- `share/index.html` — 招待リンク中継ページ（LINE 等で送られた URL から kamidoko-app:// へ自動転送）
- `_config.yml` — Jekyll 設定（theme: cayman、baseurl: ""）
- `assets/css/style.scss` — Cayman テーマの上書き CSS（フッター/ヘッダー非表示・ウォーム配色カード）

## デプロイ

main ブランチに push すると GitHub Pages が自動でリビルドし、1〜3 分で反映されます。
新サイト (kamidoko.github.io) と旧サイト (bobshiro/kamidoko の Pages) の両方を更新する場合は
それぞれ `git push kamidoko main` と `git push origin main` を実行。
