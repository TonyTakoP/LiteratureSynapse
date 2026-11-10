---
schema_version: 1
type: "relation_ledger"
---

# 研究關聯台帳

每列為一條有方向的語意關聯。Agent 推論預設 proposed；confirmed 必須有具體確認紀錄。belongs_to 由筆記 metadata 衍生，不寫入此表。正式檔案位置為 `references/relations.md`，初始化保留空表即可，不添加示範列。

| id | from | relation | to | status | 證據連結 | 理由／適用條件 | proposed_by | created | updated | 確認紀錄 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |

## 審核歷史

記錄具體關聯 ID、舊／新狀態、確認者、時間與所接受草案；新增歷史不刪舊紀錄。無確認時留空。
