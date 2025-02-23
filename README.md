<div id="top"></div>

## 目次

1. [リポジトリ概要](#リポジトリ概要)
2. [使用技術一覧](#使用技術一覧)
3. [Dockerコンテナ概要](#Dockerコンテナ概要)
4. [環境構築手順](#環境構築手順)

## リポジトリ概要

概要：以下アプリのローカル開発環境用Dockerテンプレート<br>
<br>
対象アプリ：「coachtechフリマ」<br>
※リポジトリURL<br>
[https://github.com/YoshidaChiharu/CoachtechFleaMarket](https://github.com/YoshidaChiharu/CoachtechFleaMarket)

## 使用技術一覧

| 言語・フレームワーク  | バージョン |
| --------------------- | ---------- |
| Laravel               | 11.27.2    |
| PHP                   | 8.3.7      |
| NGINX                 | 1.26.0     |
| MySQL                 | 8.0.37     |
| inertia.js            | 1.3.2      |
| Vue.js                | 3.5.13     |
| tailwindCSS           | 3.4.16     |
| Laravel Breeze        | 2.2.6      |
| Laravel Vite          | 3.4.16     |
| PHP Unit              | 11.5.0     |

## Dockerコンテナ概要

- 【nginx】：Webサーバーソフト稼働用コンテナ
- 【php-fpm】：PHP実行用コンテナ（※）
- 【mysql】：DB用コンテナ（アプリのメインDB）
- 【mysql.test】：DB用コンテナ（PHPUnitテスト用DB）
- 【phpmyadmin】：DB管理ツール「phpmyadmin」稼働用コンテナ
- 【supervisor】：Laravelキュー（queue:work）常時実行用コンテナ
<br>
※「Laravel Vite」使用想定の為、php-fpmコンテナの "5173" ポートを公開

## 環境構築手順

※アプリ側のReadMe記載手順を参照<br>
[https://github.com/YoshidaChiharu/CoachtechFleaMarket/tree/develop?tab=readme-ov-file#%E7%92%B0%E5%A2%83%E6%A7%8B%E7%AF%89%E6%89%8B%E9%A0%86](https://github.com/YoshidaChiharu/CoachtechFleaMarket/tree/develop?tab=readme-ov-file#%E7%92%B0%E5%A2%83%E6%A7%8B%E7%AF%89%E6%89%8B%E9%A0%86)

<p align="right">(<a href="#top">トップへ</a>)</p>
