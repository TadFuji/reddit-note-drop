# reddit-note-drop

Reddit 日次トレンドの note.com 記事（「Reddit日本語解説 YYYY/MM/DD｜…」）の原稿と表紙を、
VPS から GitHub Actions へ渡すための置き場所です（2026-10-12 作成）。

- VPS の `reddit` プロジェクト（`push_note_github.py`）が毎朝 `{日付}-Reddit-Top30-note.md` と
  `{日付}-Reddit-Top30-cover.png` をここへ置き、TadFuji/Hacker-News の `reddit-note.yml` に合図を送ります。
- 公開処理はこのリポジトリを読み取るだけです。VPS のトークンはこのリポジトリにしか書けません
  （VPS が乗っ取られても、投稿のプログラムと note のログイン情報には届かないようにするため）。
- 中身は数分後に note.com で公開される記事と同じものです。
