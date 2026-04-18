# google-tts-colab-ja

Google Cloud TTS × Colab で日本語ナレーション MP3 を一括生成 | Batch Japanese narration generator via Google Cloud TTS on Colab — no JSON key required.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/thunderblog/google-tts-colab-ja/blob/main/tts_narration.ipynb)

---

## 概要

このノートブックは、**Google Cloud Text-to-Speech API** を使って日本語ナレーション MP3 を一括生成するツールです。

ブログ記事・YouTube 動画と合わせて公開しています。

- 📝 **記事**：[Google Cloud TTS を Colab で使う方法【MP3 一括生成】](#)（公開後にリンクを更新）
- 🎬 **YouTube**：[Google Cloud TTS × Colab 後編 — MP3 一括生成してダウンロード](#)（公開後にリンクを更新）

---

## 特徴

- **JSON キー不要** — Google アカウントだけで認証できる
- **GUI フォーム** — コードを書かずにドロップダウン・スライダーで音声・速度・ピッチを設定
- **一括生成** — ナレーションリストを書いてセルを実行するだけで全件 MP3 化
- **ZIP ダウンロード** — 生成したファイルをまとめてローカルに保存
- **Chirp3 HD 対応** — 最高品質の日本語音声（30 種類）を含む全 41 音声に対応

---

## 使い方

### 1. Colab で開く

上の **「Open in Colab」バッジ**をクリックするか、以下のリンクから開いてください。

- **そのまま試す**：バッジをクリック
- **自分のドライブにコピーして使う**：↓ のリンクを使用

👉 [自分のドライブにコピーして開く](https://colab.research.google.com/github/thunderblog/google-tts-colab-ja/blob/main/tts_narration.ipynb?copy=true)

### 2. 事前準備

実行前に以下の準備が必要です。

1. [Google Cloud Console](https://console.cloud.google.com/) で GCP プロジェクトを作成
2. **課金アカウントを紐付け**（無料枠内でも必須です）
3. **Cloud Text-to-Speech API** を有効化
4. プロジェクト ID を控えておく

> ℹ️ 無料枠（Chirp3 HD / Neural2: 月 100 万文字、Wavenet / Standard: 月 400 万文字）内であれば課金は発生しませんが、課金アカウントの紐付け自体は必須です。

詳細な手順は[記事](#)で解説しています。

### 3. ノートブックを上から順に実行

| ステップ | 内容 |
|---------|------|
| Step 1 | ライブラリのインストール |
| Step 2 | Google アカウント認証 |
| Step 3 | 音声・速度・ピッチの設定 |
| Step 4 | ナレーションリストの編集 |
| Step 5 | TTS 関数の定義 |
| Step 6 | 試聴（任意） |
| Step 7 | 一括生成 |
| Step 8 | ZIP でダウンロード |

---

## 対応音声

| 種別 | 無料枠（月） | 特徴 |
|------|-------------|------|
| Chirp3 HD | 100 万文字 | 最高品質・会話的な自然さ（30 種類） |
| Neural2 | 100 万文字 | 自然な抑揚・感情表現が豊か |
| Wavenet | 400 万文字 | 滑らかで落ち着いたトーン |
| Standard | 400 万文字 | コンパクトで処理が速い |

---

## ライセンス

[MIT License](./LICENSE)
