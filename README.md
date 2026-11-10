# LiteratureSynapse

以本地 Markdown 保存研究資料、以 Codex Agent Skills 定義工作流程的個人研究知識庫。不需啟動 App、CLI 或服務，也沒有自訂程式碼。

## 開始使用

在 Codex 開啟本資料夾，確認技能選單列出本專案六個 Skills；若尚未出現，重新開啟工作階段。新技能的自動發現須依 [環境說明](docs/environment.md) 在實際宿主驗證，不能只以檔案存在推定成功。

可直接說：

- 「建立『企業 Agent 可靠性』研究主題。」
- 「把以下摘要整理成 Paper，加入剛才的主題：……」
- 「記錄今天跟教授討論的重點：……」
- 「保存這個靈感，暫時不要指定主題：……」
- 「找出該主題提到 LLM-as-a-Judge 的 Paper。」
- 「更新該主題摘要，再依既有台帳產生 Mermaid 圖譜。」

也可明確指定 `$literature-synapse` 或 `$note-capture` 等本專案 Skill。已知的單一任務直接使用對應 Skill；入口處理混合或不明確任務。

## 文件導覽

| 文件 | 用途 |
| --- | --- |
| [需求](docs/requirements.md) | 原始 v2.0 需求。 |
| [共用資料規範](docs/conventions.md) | metadata、ID、證據、關聯、彙總、圖譜與審核契約。 |
| [操作說明](docs/usage.md) | 日常操作、確認與回復方式。 |
| [宿主能力](docs/environment.md) | Skills 啟用、已驗證工具及降級。 |
| [MVP 工作項目](docs/mvp.md) | M0–M7 交付、依賴與驗收。 |
| [驗收操作](docs/acceptance/README.md)／[驗收紀錄](docs/acceptance/results.md) | 隔離範例、情境與實際驗證範圍。 |

`templates/` 提供八份模板；`.agents/skills/` 放六份自然語言流程。正式 `topics/`、`notes/`、`references/`、`graphs/` 在第一次有相關需求時建立。本次沒有新增正式研究資料。

## 使用原則

筆記與人工整理的台帳保留來源，彙總及圖譜可重建。主題文件的人工區不被重建；要長期保留的文字放在人工區。新增筆記不會自動刷新摘要／圖譜，需要明確要求。

改寫既有筆記、補引用、確認推論關聯與批次改寫，先展示具體變更再確認。私人資料留在本地；不建立腳本、安裝套件、建立資料庫或上傳私人內容來補足工具能力。Mermaid 是正式圖譜來源，SVG 僅為有原生支援時的選配。
