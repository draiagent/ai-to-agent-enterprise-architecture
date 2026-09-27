# AI to Agent Enterprise Architecture

**以任務完成為中心：先做得成，再做得省。**

![企業任務架構總覽](assets/cards/01-overview.png)

AI Coach 益力康陳董 x CGM Coach 血糖教練 | 2026 AI to Agent

版本 **1.0.0** · 2026-09-27 · 方法論基線，尚未完成企業實測 · 保留所有權利

![版本](https://img.shields.io/badge/version-1.0.0-blue)

## 為什麼需要

企業需要管理從提出需求、取得依據、執行操作到驗收交付的完整過程。單次模型價格無法代表整體成本；反覆補問、重試與人工修正都需要被記錄。

## 這是什麼

本專案是方法論、知識圖卡與實作規格集合。六大系統為任務、智能、知識、編排、執行、治理；它們是責任分工，不是固定依序執行的六層流水線。治理貫穿全部系統。

LLM/Agent 是主要理解與規劃核心。Rule、Jev 類結構化模型、檢索與工具依任務選用。本文不承諾特定模型的成本、效能或準確率。

本套件沒有自動化執行程式、可安裝 Skill 或 MCP server；使用範本不等於已完成系統整合。

## 快速開始

1. 閱讀 [方法論](docs/methodology.md) 與 [圖卡導覽](docs/cards.md)。
2. 複製 [VAC 範本](templates/vac-task.json)，填入目標、資料、限制、輸出與驗收。
3. 依 [路徑決策表](docs/routing.md) 選擇最小足夠的知識與工具組合。
4. 交由具備所需權限的 Agent 或人員執行，保留來源與過程紀錄。
5. 填寫 [成本紀錄表](templates/task-cost.csv) 及 [驗收表](templates/evaluation.md)。
6. 只將經審核且可重用的資訊寫入長期知識。

閱讀無需安裝。JSON 與 CSV 可用一般文字編輯器及試算表開啟；執行自動化須另建整合與權限控制。

## 輸入、輸出與驗收

輸入是明確任務規格、已授權資料及預算；輸出是交付成果、來源清單、驗收紀錄及成本紀錄。通過條件由每份 VAC 預先約定，模型自己聲稱完成不算驗收證據。

## 案例

- [個人知識整理](examples/01-personal-knowledge.md)：筆記轉可追溯的行動清單。
- [企業知識問答](examples/02-enterprise-knowledge.md)：依有效 SOP 回答，缺證據時標示不足。
- [跨系統企業任務](examples/03-cross-system.md)：會議轉待辦，檢查權限與重複寫入。

三例均為模擬規格與預期輸出，不是已實測成效。

## 適用範圍與限制

適用於知識整理、研究、會議行動化與企業 Agent 任務設計。不適合直接當作無人監督的高風險決策或交易系統。部署選型、資料合規與業務責任仍需個別評估。

## 文件與素材

| 路徑 | 用途 |
|---|---|
| [docs/methodology.md](docs/methodology.md) | 定義、六系統與閉環 |
| [docs/routing.md](docs/routing.md) | 選路、停止與升級 |
| [docs/cost-model.md](docs/cost-model.md) | Token、TTC 與成功率口徑 |
| [docs/cards.md](docs/cards.md) | 8 張圖片及逐頁替代文字 |
| [docs/visual-style.md](docs/visual-style.md) | 電曜智核視覺規範 |
| [docs/social-post.md](docs/social-post.md) | 社群介紹文章 |
| [docs/publishing.md](docs/publishing.md) | GitHub 上傳與發布說明 |
| [examples/README.md](examples/README.md) | 三個模擬案例索引 |
| [templates/vac-task.json](templates/vac-task.json) | 可填寫任務規格 |
| [templates/task-cost.csv](templates/task-cost.csv) | 執行成本紀錄 |
| [templates/evaluation.md](templates/evaluation.md) | 驗收與寫入審核 |
| [VALIDATION.md](VALIDATION.md) | 本地檢查及未驗證項目 |

## 版本與後續計畫

版本以 [VERSION](VERSION) 為唯一中繼資料來源（project.json 同步）。v1.0.0 表示方法論文件基線，並不表示軟體已達正式生產成熟度。下一階段以三類真實任務驗證成功率、成本與人工修改量，再決定是否建立 Skill 或 MCP 參考實作。

## 授權、版權與貢獻

本 repo 採保留所有權利（All rights reserved），見 [LICENSE](LICENSE)。作者品牌不等於法律權利人，詳見 [COPYRIGHT.md](COPYRIGHT.md) 與 [素材來源聲明](ASSET_SOURCES.md)。修改建議依 [CONTRIBUTING.md](CONTRIBUTING.md) 提交。

**AI Coach 益力康陳董 x CGM Coach 血糖教練 | 2026 AI to Agent**
