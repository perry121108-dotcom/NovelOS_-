# NovelOS 新版 Skill 概述

NovelOS 是一套專為 **長篇小說及 IP 開發** 設計的 AI 作業系統。新版 NovelOS 在經典世界觀與角色管理功能之外，新增了 **Phase 0：Research Phase（市場研究階段）**，確保在投入創作前先分析市場趨勢與題材可行性。透過多 AI 分工與嚴格的工作流程，NovelOS 能夠有效管理龐大的世界觀、角色與劇情資料，避免吃書、角色崩壞與戰力膨脹等長篇常見問題。

## 專案工作流程

NovelOS 將長篇開發分為多個階段，每個階段都有明確的負責 AI 與輸出。

### Phase 0：Research Phase（市場研究階段）
在啟動 NovelOS 之後，首先進入 Research Phase，由 **Gemini**（Research AI）負責蒐集與分析市場資料，包含：

- **市場趨勢調查**：分析近期熱門題材與讀者偏好。
- **競品分析**：研究同類型作品的優缺點，找出市場缺口。
- **神話／歷史／科學考據**：提供建立世界觀時可參考的文化與科學素材。
- **爆款元素與情緒點**：提取受眾喜愛的情節元素與情緒節奏。

研究結果需儲存於 `Research/` 目錄下的檔案中，不得直接混入世界觀設定。完成研究後，由創作者決定是否啟動正式開發。

### Phase 1：NovelOS 初始化
由 **ChatGPT** 擔任專案總控 (PM)，建立 NovelOS 專案的基礎檔案結構與規則：

- 產生 `PROJECT_RULES.md`、`WORKLOG.md`、`CHANGELOG.md` 等核心檔案。
- 初始化世界觀資料庫 (Lore Database) 與角色資料庫 (Character Database)。
- 制定禁止事項與版本控制規範。

### Phase 2：世界觀建立
建立完整世界觀設定，包括國家、種族、歷史、能力規則、地圖與宗教等，存於 `02_Lore/` 目錄。確保各設定相互一致，並使用 `Memory System` 記錄不可變規則。

### Phase 3：角色建立
在 `03_Characters/` 目錄中，為每個重要角色撰寫資料卡，包含性格、願望、恐懼、成長線、能力與弱點等。角色檔案應遵循 `CHARACTER_TEMPLATE.md` 的格式。

### Phase 4：長篇規劃
規劃劇情節奏與主要事件，佈局伏筆與回收計畫。使用 `TIMELINE_TEMPLATE.md` 與 `FORESHADOW_TEMPLATE.md` 來編制時間線與伏筆。

### Phase 5：章節開發
由 **Claude Code** 擔任主開發者，根據長篇規劃撰寫各章節，並在每次修改後於 `WORKLOG.md` 記錄。重要修改須更新 `CHANGELOG.md`。

### Phase 6：QA 檢查
完成章節後，交由 **Gemini**（QA AI）檢查設定衝突、角色是否 OOC、時間線矛盾、戰力是否平衡等，並提出修正建議。

### Phase 7：版本同步與出版準備
最終由 ChatGPT 整合修訂內容，更新版本號與版本紀錄，進行翻譯與出版格式準備。

## 檔案與資料夾結構

```
NovelOS_Project/
├── Research/              # 市場與題材研究資料
│   ├── market_trends.md
│   ├── audience_analysis.md
│   ├── myth_science_notes.md
│   └── summary.md
├── PROJECT_RULES.md       # 專案規則與禁止事項
├── WORKLOG.md             # 工作日誌，記錄每次修改
├── CHANGELOG.md           # 版本紀錄
├── 00_Project_Rules/      # 延伸規則檔案（如禁止事項詳述）
├── 01_Requirements/       # 開發需求與題材說明
├── 02_Lore/               # 世界觀資料庫
├── 03_Characters/         # 角色資料庫
├── 04_Timeline/           # 時間線檔案
├── 05_Foreshadow/         # 伏筆管理檔案
├── 06_PowerScale/         # 戰力控制檔案
├── 07_EmotionalCurve/     # 情緒曲線檔案
├── 08_Chapters/           # 章節草稿與最終稿
├── 09_QA/                 # QA 報告與修正建議
├── 10_Worklog/            # 過往工作日誌存檔
└── 11_Versions/           # 歷史版本與備份
```

## 如何使用 NovelOS

1. **啟動專案**：創建 `NovelOS_Project/` 目錄，並使用本包中的範本文件初始化結構。
2. **進行 Research Phase**：使用 Gemini 進行市場調查，將結果存入 `Research/` 目錄並產出 `summary.md`。待創作者確認題材可行後，再進入 Phase 1。
3. **初始化專案**：由 ChatGPT 根據 `SYSTEM_PROMPT` 建立世界觀與角色初稿，生成 `Lore` 和 `Characters` 資料。
4. **按照流程開發**：依序進行世界觀建立、角色建立、長篇規劃、章節開發與 QA。
5. **維護工作日誌與版本紀錄**：任何修改均須記錄於 `WORKLOG.md`，重大變更更新 `CHANGELOG.md`。
6. **遵守禁止事項與 SOP**：所有 AI 必須遵循 `PROJECT_RULES.md` 與 `AI_AGENT_SOP.md`，不可擅自新增設定或忽略研究結果。

透過本 Skill，您可以確保小說開發流程嚴謹、資料整合完整，並避免長篇開發常見的崩壞問題。