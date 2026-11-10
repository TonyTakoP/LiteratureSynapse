# MVP 工作項目

交付皆為 Markdown，不使用自動化測試或程式驗證器。[驗收操作](acceptance/README.md) 提供固定案例；[紀錄](acceptance/results.md) 分開已執行與待宿主驗證。

| 項目 | 交付與依賴 | 操作與預期檔案變化 | 驗收 |
| --- | --- | --- | --- |
| M0 環境與契約 | conventions、environment；無依賴 | 閱讀環境與資料規範，核對 .agents/skills 位置及檔案權限。 | 只有 Markdown；六份 Skill frontmatter 齊全、相對參考可達；實際宿主技能選單另驗。 |
| M1 模板與樣本 | 八份 templates 與隔離 fixtures；依 M0 | 依紙上輸入填四類筆記、主題與台帳；正式來源不變。 | 必要欄位、來源分層、穩定 E 編號與留空規則一致；樣本標示測試。 |
| M2 主題管理 | topic-management；依 M1 | 「新增主題與子主題、改名、封存」；僅對應主題檔與 metadata 改變。 | ID／路徑不變、唯一 summary_path、自指與父子循環停止。 |
| M3 筆記記錄 | note-capture；依 M1 | 各新增一篇 Paper／Meeting／Web／Idea，Paper 歸屬兩主題；每筆一檔。 | 不虛構 DOI、作者、教授決議；重複來源先列現有檔，既有改寫需審核。 |
| M4 檢索 | research-retrieval；依 M0、M1 | 交集條件查 LLM-as-a-Judge／Paper／主題；零寫入。 | 回傳正確 ID、證據連結；無結果明說，正式搜尋排除驗收資料。 |
| M5 彙總 | topic-synthesis；依 M1 | 更新主題、變更來源後再更新、移除歸屬後再更新。 | 只改生成區／updated，人工區原樣；新增、移除與衝突皆反映，標記損壞不覆寫。 |
| M6 關聯圖譜 | knowledge-graph；依 M1 | 記 proposed 支持／衝突、接受草案、繪圖；修改台帳及圖譜指定區。 | 每邊有證據，狀態與方向一致；失效證據需重審，超量拆圖，無 SVG 不阻斷。 |
| M7 入口整合 | literature-synapse、usage、驗收紀錄；依 M2–M6 | 「整理論文、加入主題、更新摘要並繪圖」。 | 正確按需載入、審核不跳過、失敗可續接，無關請求不誤用研究流程。 |

M2–M6 各以 M1 的隔離資料驗收，不必先完成其他工作 Skill；整合驗收另看跨流程。後續 Phase 2／3 可增加 literature-analysis、research-review、thesis-writing，但沿用來源、審核及零程式碼邊界，不先建立未實作入口。
