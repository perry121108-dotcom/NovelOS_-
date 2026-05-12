<div align="center">

# 📖 NovelOS — AI 長篇小說開發作業系統
### AI-Powered Long-Form Novel Development Operating System

[![Version](https://img.shields.io/badge/version-v1.0.0-blue.svg)](CHANGELOG.md)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](#)
[![Language](https://img.shields.io/badge/language-繁體中文%20%7C%20English-orange.svg)](#)

> 🇹🇼 [繁體中文說明](#-novelos--ai-長篇小說開發作業系統-1) ・ 🇺🇸 [English Documentation](#-novelos--ai-powered-novel-development-os)

</div>

---

# 🇹🇼 NovelOS — AI 長篇小說開發作業系統

**NovelOS** 是一套專為**長篇小說及 IP 開發**設計的 AI 作業系統。它不只是生成故事的工具，而是一套完整的開發流程管理系統，協調多個 AI 協作，避免長篇創作中最常見的崩壞問題。

## ✨ 為什麼需要 NovelOS？

| 長篇常見問題 | NovelOS 解法 |
|-------------|-------------|
| 世界觀前後矛盾（吃書） | Lore Database + 版本控制 |
| 角色崩壞（OOC） | 角色資料卡 + QA 審查機制 |
| 戰力無限膨脹 | Power Scale Manager + 禁止無代價升級 |
| 伏筆遺忘不回收 | Foreshadow Manager 全程追蹤 |
| 多 AI 協作混亂 | AI Agent SOP 明確分工 |
| 題材盲目開發 | Research Phase 市場研究先行 |

## 🚀 核心功能

- 📊 **市場研究系統** — 開發前先分析趨勢、競品與受眾
- 🧠 **四層記憶管理** — 核心設定、角色記憶、劇情記憶、章節記憶
- 🌍 **世界觀資料庫** — 背景、種族、歷史、魔法 / 科技規則
- 👤 **角色資料庫** — 標準化角色卡，含成長線與關係網
- 🧩 **伏筆管理系統** — 每個伏筆獨立追蹤，確保全部回收
- ⚡ **戰力控制系統** — 防止無代價升級與戰力失衡
- 📈 **情緒曲線規劃** — 設計每篇章的情緒起伏節奏
- 📅 **時間線管理** — 防止時間錯亂與邏輯矛盾
- 🔍 **QA 品質審查** — 完整的設定衝突與角色行為審查
- 📦 **版本控制** — SemVer 版本號 + WORKLOG + CHANGELOG

## 🤖 AI 分工架構

```
Phase 0      Phase 1-4       Phase 5         Phase 6      Phase 7
市場研究  →  世界觀+規劃  →  章節撰寫  →   品質審查  →  出版整合
Gemini      ChatGPT        Claude Code      Gemini      ChatGPT
```

| AI | 角色 | 負責階段 |
|----|------|---------|
| **Gemini** | Research AI | Phase 0 市場研究 |
| **ChatGPT** | PM / Core | Phase 1 初始化、Phase 2 世界觀、Phase 3 角色、Phase 4 規劃、Phase 7 出版 |
| **Claude Code** | Main Developer | Phase 5 章節開發 |
| **Gemini** | QA AI | Phase 6 品質審查 |
| **Codex** | Engineering AI | 全流程技術支援 |

## 📁 專案檔案結構

```
NovelOS_Project/
├── Research/              # Phase 0：市場研究資料
├── PROJECT_RULES.md       # 核心規則與禁止事項
├── WORKLOG.md             # 工作日誌
├── CHANGELOG.md           # 版本紀錄
├── 02_Lore/               # 世界觀資料庫
├── 03_Characters/         # 角色資料庫
├── 04_Timeline/           # 時間線管理
├── 05_Foreshadow/         # 伏筆管理
├── 06_PowerScale/         # 戰力控制
├── 07_EmotionalCurve/     # 情緒曲線
├── 08_Chapters/           # 章節草稿與正稿
├── 09_QA/                 # QA 審查報告
└── 11_Versions/           # 版本備份
```

## ⚡ 快速開始

```
1. 複製本套件的範本文件至你的 NovelOS_Project/ 目錄
2. 在 Gemini 執行 Research Phase（參考 RESEARCH_TEMPLATE.md）
3. 確認題材可行後，在 ChatGPT 使用 SYSTEM_PROMPT.txt 啟動專案
4. 依照 Phase 2 → 3 → 4 → 5 → 6 → 7 順序推進
5. 每次修改立即更新 WORKLOG.md
```

## 📚 說明文件

| 文件 | 說明 |
|------|------|
| [📘 完整說明文件（繁體中文）](NovelOS_NewSkill_Package/NovelOS_說明文件_中文.md) | 完整功能介紹、操作指南、範本說明、FAQ |
| [📗 Full Documentation (English)](NovelOS_NewSkill_Package/NovelOS_Documentation_English.md) | Complete feature overview, operation guide, template reference, FAQ |
| [⚙️ SYSTEM_PROMPT.txt](NovelOS_NewSkill_Package/SYSTEM_PROMPT.txt) | NovelOS AI 系統指令 |
| [📋 PROJECT_RULES.md](NovelOS_NewSkill_Package/PROJECT_RULES.md) | 專案規則與禁止事項 |
| [🤖 AI_AGENT_SOP.md](NovelOS_NewSkill_Package/AI_AGENT_SOP.md) | AI 分工 SOP |

---

# 🇺🇸 NovelOS — AI-Powered Novel Development OS

**NovelOS** is an AI operating system designed for **long-form novel and IP development**. It's not just a story generator — it's a complete development pipeline that coordinates multiple AIs to prevent the most common failures in long-form storytelling.

## ✨ Why NovelOS?

| Common Problem | NovelOS Solution |
|---------------|-----------------|
| Worldbuilding inconsistencies | Lore Database + Version Control |
| Character OOC (Out of Character) | Character Cards + QA Review |
| Unchecked power scaling | Power Scale Manager + No-Free-Upgrade Rule |
| Forgotten foreshadowing | Foreshadow Manager full tracking |
| Multi-AI collaboration chaos | Clear AI Agent SOP |
| Blind development | Research Phase before any creation |

## 🚀 Core Features

- 📊 **Market Research System** — Analyze trends, competitors, and audience before developing
- 🧠 **4-Layer Memory Management** — Core settings, character memory, plot memory, chapter memory
- 🌍 **Lore Database** — Background, races, history, magic/tech system rules
- 👤 **Character Database** — Standardized character cards with growth arcs and relationships
- 🧩 **Foreshadowing Manager** — Individual tracking per foreshadow, ensures all are resolved
- ⚡ **Power Scale Manager** — Prevents cost-free upgrades and power imbalance
- 📈 **Emotional Curve Planning** — Design emotional arcs for each chapter
- 📅 **Timeline Manager** — Prevents time paradoxes and logical errors
- 🔍 **QA Pipeline** — Full setting conflict and character behavior auditing
- 📦 **Version Control** — SemVer + WORKLOG + CHANGELOG enforced

## 🤖 AI Division of Labor

```
Phase 0      Phase 1-4       Phase 5         Phase 6      Phase 7
Research  →  Lore+Planning → Chapter Write → QA Review → Publishing
Gemini      ChatGPT        Claude Code      Gemini      ChatGPT
```

## ⚡ Quick Start

```
1. Copy template files into your NovelOS_Project/ directory
2. Run Research Phase in Gemini (see RESEARCH_TEMPLATE.md)
3. After confirming genre viability, start the project in ChatGPT with SYSTEM_PROMPT.txt
4. Follow Phases 2 → 3 → 4 → 5 → 6 → 7 in sequence
5. Always update WORKLOG.md immediately after any modification
```

## 📚 Documentation

| Document | Description |
|----------|-------------|
| [📘 完整說明文件（繁體中文）](NovelOS_NewSkill_Package/NovelOS_說明文件_中文.md) | Full guide in Traditional Chinese |
| [📗 Full Documentation (English)](NovelOS_NewSkill_Package/NovelOS_Documentation_English.md) | Complete feature overview, operation guide, FAQ |
| [⚙️ SYSTEM_PROMPT.txt](NovelOS_NewSkill_Package/SYSTEM_PROMPT.txt) | NovelOS AI system instructions |
| [📋 PROJECT_RULES.md](NovelOS_NewSkill_Package/PROJECT_RULES.md) | Project rules and prohibitions |
| [🤖 AI_AGENT_SOP.md](NovelOS_NewSkill_Package/AI_AGENT_SOP.md) | AI Agent division SOP |

---

<div align="center">

**NovelOS v1.0.0** — 讓長篇小說開發有序進行，確保世界觀完整與作品質量。

*Keeping long-form novel development structured, ensuring worldbuilding integrity and work quality.*

</div>
