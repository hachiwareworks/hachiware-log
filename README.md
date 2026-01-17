# 公開フロー（チェックリスト）

このブログは **Hugo + GitHub Actions + GitHub Pages** で公開しています。  
`public/` は git 管理しません。

---

## 公開手順（最短）

### 1. 記事を作成
- `content/posts/<slug>/index.md`
- 画像は同じフォルダに置く

---

### 2. Front Matter を確認
- [ ] `draft: false`（または draft 行を削除）
- [ ] `date:` が未来日でない
- [ ] `summary:` を記載（OGP / 一覧用）

---

### 3. ローカル確認

```bash
hugo server
```

※ 下書きも見る場合

```bash
hugo server -D
```

### 4. GitHub に反映（＝公開）

```bash
git status
git add content/ static/ layouts/ hugo.toml
git commit -m "post: <title>"
git push
```

### 5. Actions を確認
GitHub → Actions

最新の workflow が 緑（success） になっていること

### 6. 公開URLを確認
https://hachiware-log.com/

よくある原因（表示されない時）
- [ ] git push していない
- [ ] draft: true のまま
- [ ] date が未来
- [ ] Actions が失敗している

### メモ
public/ は Actions が自動生成

ローカル表示 ＝ 公開 ではない
👉 push ＝ 公開

---