# AI Short Anime Studio

このフォルダは、縦型9:16のAIショートアニメを継続制作するための共通基盤です。

## 基本仕様

- 基本尺: 60〜90秒
- 必要な場合のみ延長
- 最大尺: 180秒以内
- 原則: 1CUT＝1アクション
- 採用済みの設定、台詞、CUTを無断で変更しない
- 動画生成プロンプトにBGM指示を入れない

## Codexで新作を始める流れ

1. `ai-short-anime-studio/templates/new-project/` を複製する。
2. `ai-short-anime-studio/projects/作品名/` として保存する。
3. `PROJECT.md` に企画内容と決定事項を書く。
4. Codexへ次のように依頼する。

```text
このリポジトリのAGENTS.mdを必ず読み、
$vertical-short-anime-story-design を使用してください。

ai-short-anime-studio/templates/new-projectを複製し、
ai-short-anime-studio/projects/PROJECT-NAMEを作成してください。

縦型9:16、基本60〜90秒、最大180秒以内で、
まず企画とストーリー構成だけを作成してください。
採用済み設定は勝手に変更しないでください。
```

5. ストーリー承認後、`$cut-design` と `$camera-direction` を使ってCUT設計を行う。
6. CUT承認後、`$image-prompt-design` で開始・終了画像を設計する。
7. 画像承認後、`$video-prompt-design` で動画生成プロンプトを作成する。

## Skills

共通Skillsはリポジトリ直下の `.agents/skills/` にあります。

- `vertical-short-anime-story-design`: 縦型ショートアニメ構成
- `cut-design`: 1CUT＝1アクションのCUT設計
- `camera-direction`: 縦型画面向けカメラワーク
- `image-prompt-design`: 開始・終了画像プロンプト
- `video-prompt-design`: AI動画生成プロンプト

新作で得た改善点は作品フォルダだけに残さず、再利用価値がある場合は該当Skillへ追記します。
