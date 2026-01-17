---
title: "Hugoをローカルで動かせた日"
date: 2026-01-16
draft: true
tags:
  - log
  - setup
summary: "MacにHugoを入れる中で、localhost表示まで確認したログ。"
summary_en: "[SOLVED] A log of setting up Hugo on macOS while confirming it worked on localhost."
---

今日は、ずっと考えていた「記録を残す場所」を、
Hugoでローカルに立ち上げた。

正直、始める前は少しだけ不安だったけれど、
画面にタイトルが表示された瞬間、
「あ、ここは私の場所だ」と思えた。

---

## 今日やったこと
- HomebrewでHugoをインストール
- `hugo new site` でサイト作成
- PaperModテーマを設定
- `hugo server -D` でローカル起動
- localhost:1313 に表示された画面を確認

## 実行したコマンド

```bash
# Hugoをインストール
brew install hugo

# Hugoのバージョン確認
hugo version

# 新しいサイトを作成
hugo new site hachiware-log

# ローカルサーバーを起動（下書きも表示）
hugo server -D
```

![localhostで表示できた画面](hugo-localhost.png)

*↑ローカルで初めて表示された画面*

## つまずいたこと
- hugo.toml をどこで編集するか少し迷った

  →VSCodeで編集することにした。

- VSCodeでコマンドを実行していいのか不安だった

  →VSCodeのターミナルで実行してもOKなので、場所だけ確認して実行した。

## できたこと
- MacでHugoをローカル起動できた
- 「これは記事にできる」と思えた

---

## 明日の自分へ
この場所は、完成させるためじゃなくて、
歩いた記録を置いていくための場所。

焦らず、でも止まらず続けよう。