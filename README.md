# hackathon-2021-shigyoit

「士業×IT ハッカソン Vol.1」で作った Web アプリ「てんきぶんっ！」の、画面のプログラム。

> 当時の記録として残しているリポジトリです。プログラムは当時のままで、リファクタリングや修正は行っていません。

## 概要

「てんきぶんっ！」は、天気から「あの人」のその日の気分を予想して見せる Web アプリである。総合指数、気分指数、仕事指数、天気痛指数の4つを、星の数で表示する。

このリポジトリには、画面（フロントエンド）だけが入っている。表示している文章と指数は、プログラムに直接書いた見本の値である。

| 項目 | 内容 |
| --- | --- |
| イベント | 【賞金総額100万円】士業×IT ハッカソン Vol.1 |
| 開催時期 | 2021年9月25日〜26日（オンライン） |
| 主催 | SIGYOIT（共催：株式会社ウェザーニューズ） |
| テーマ | 気象データの API サービス「WxTech」を使ったビジネスモデルやアプリの開発 |
| 作成期間 | 2021年9月25日〜26日（2022年1月に、パッケージを更新） |
| イベントのページ | [【賞金総額100万円】士業×IT ハッカソン Vol.1（connpass）](https://sigyo-it.connpass.com/event/217882/) |
| チーム | PichiPichi Ichinensei（デザイナーを含む4人） |
| 構成 | Next.js、React、TypeScript、styled-components、Storybook |

## ディレクトリ構成

| ディレクトリ | 内容 |
| --- | --- |
| `src/pages/` | ページ。トップページの1つだけ |
| `src/components/` | 部品。小さい順に `atoms/`、`molecules/`、`organisms/`、`templates/` に分けている。部品ごとに、本体（`index.tsx`）と Storybook 用の見本（`stories.tsx`）がある |
| `src/styles/` | 色と、全体に適用するスタイル |
| `src/shared/` | 共通の型と画像 |
| `public/` | ロゴ、アイコン、見本の画像 |
| `.storybook/` | Storybook の設定 |

## 実行環境

| ソフトウェア | バージョン | 用途 |
| --- | --- | --- |
| Node.js | 16 | 実行と、パッケージの管理 |
| Next.js | 12.0.7 | Web アプリの枠組み |
| React | 17.0.2 | 画面の部品 |

Next.js と React のバージョンは、`package.json` の記録による。Node.js は、作成した時期の長期サポート版である。

## セットアップ

```sh
npm install
```

## 実行方法

```sh
npm run dev
```

Web ブラウザで <http://localhost:3000> を開く。

部品の一覧は、Storybook で見られる。

```sh
npm run storybook
```

Web ブラウザで <http://localhost:6006> を開く。
