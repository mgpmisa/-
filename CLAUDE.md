# このリポジトリについて

YouTubeチャンネル「ミサp」の制作メモと、毎日のトレンド調査の保管場所です。

## 回答のルール

- 日本語で、わかりやすく答える（専門用語には短い説明を付ける）。
- 利用者はプログラミングの専門家ではないので、手順は具体的に書く。

## トレンド知識の使い方

- 毎朝、自動でトレンド調査が行われ `trends/` フォルダに保存されている。
  - `trends/latest.md` … いちばん新しいレポート
  - `trends/summary.md` … 最近の流れのまとめ（まずここを読む）
  - `trends/daily/YYYY/MM/YYYY-MM-DD.md` … 日ごとのレポート
- 動画の企画・タイトル・概要欄・台本などを考えるときは、まず `trends/summary.md` を読み、最近のトレンドを踏まえて提案する。
- 特定の日の話題が必要なときは `trends/daily/` の該当ファイルを読む。
- トレンド調査そのものの手順は `.claude/skills/trend-research/SKILL.md` にある。

## 評価（★1〜5）の受け付け

- 利用者がチャットで記事の評価を伝えてきたら（例：「9/26 の評価：A1は5、V1は5」）、`trends/ratings/YYYY-MM-DD.md` の該当IDの行の「評価」「メモ」列に書き込む。
- 続けて `.claude/skills/trend-research/SKILL.md` の「好みの学習ルール」に従って `trends/preferences.md` を更新する（「✍️ 手書きメモ」欄は書き換えない）。
- 変更は main ブランチに commit & push する（利用者の許可済み）。
- 好みそのものを文章で伝えられた場合（例：「VRChatの話題は毎回ほしい」）は、`trends/preferences.md` の「✍️ 手書きメモ」に追記してよい。
