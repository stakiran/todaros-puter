# todaros (Puter 版)
<img width="1064" height="699" alt="Image" src="https://github.com/user-attachments/assets/0633ef77-8a1b-4f65-93b2-5bc6756d2611" />

[stakiran/todaros](https://github.com/stakiran/todaros) の Web 版。
サーバーも API キーもなく、データは利用者自身の Puter アカウントに保存されます。

## 使い方

1. `index.html` を GitHub Pages など任意の静的ホスティングに置く
2. ブラウザで開き「Puter でサインイン」を押す（Puter アカウントがなければその場で作れる）
3. 右の `tasks.md` に定期タスクを書いて保存する（書き方は元の todaros と同じ）
4. 左に今日の分が出るので、終わったものを押して消していく

## 元との対応

| 元 (todaros.py)              | この版                                                     |
|------------------------------|------------------------------------------------------------|
| `tasks.md`（手元のファイル） | 利用者の Puter 上の `todaros/tasks.md`（画面右で編集）     |
| `python todaros.py`          | 保存時に自動生成 / 「生成し直す」ボタン                    |
| `daily.md`（行削除で消化）   | 利用者の Puter 上の `todaros/daily.md`（行を押して消化）   |

`daily.md` は 1 行目に `# yyyy/mm/dd` を持ち、日付が変わると開いたときに自動で作り直されます。
`@m @h @k @mon〜@sun @1〜@31 @ss1 @ss2 @sss1〜@sss3` の判定ロジックは `todaros.py` からそのまま移植しています。

## ローカルで試す

`index.html` をそのままブラウザで開いても動きます（Puter のログインポップアップが出ます）。

## 📝
🔒️<https://claude.ai/chat/3b14addb-3a89-4ee6-9890-8d5dda249864>
