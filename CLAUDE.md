# このリポジトリで作業する Claude へ

このリポジトリは公開されている。中身は誰でも読める。

## 作業の前に
- 設計書・進行表・作業ルールは非公開の `Haru821/rokujo-docs` にある。作業の前に、そちらの `CLAUDE.md` と `tasks.md` を必ず読む。
- このファイルより `rokujo-docs/CLAUDE.md` が優先する。

## ここに置かないもの
- Supabase の秘密の鍵（`sb_secret_` で始まるもの、`service_role`）、データベースのパスワード
- 住民の個人情報、メールアドレス、運営のメモ、お金の話
- 置いてよいのは、公開用の鍵（`sb_publishable_` で始まるもの）と Project URL だけ

## 画面のきまり
- 他人が書いた文字は必ず `textContent` で入れる。`innerHTML` は使わない
- `alert` / `confirm` / `prompt` / `window.open` は使わない
- 読んだデータは、型と長さを確かめてから使う
- 画面の言葉は日本語で短く。数字は算用数字。長いカタカナ語は避ける
- 外から読む部品は版を固定し、`integrity` を付ける（今は supabase-js 2.118.0）
