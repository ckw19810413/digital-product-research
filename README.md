# 🔍 Digital Product Research

> 數位商品銷售調研與瓶頸分析框架。自動化的深度研究報告，協助你在銷售遇到瓶頸時快速定位問題、找到解決方案。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Last Updated](https://img.shields.io/badge/Last_Updated-2026--07-brightgreen.svg)]()
[![Stars](https://img.shields.io/github/stars/ckw19810413/digital-product-research?style=social)]()
[![Repo Size](https://img.shields.io/github/repo-size/ckw19810413/digital-product-research)]()

## 📋 目錄

- [快速開始](#快速開始)
- [功能特色](#功能特色)
- [調研觸發條件](#調研觸發條件)
- [研究方法論](#研究方法論)
- [專案結構](#專案結構)
- [相關專案](#相關專案)
- [授權條款](#授權條款)

## 🚀 快速開始

```bash
# 1. 克隆此倉庫
git clone https://github.com/ckw19810413/digital-product-research.git
cd digital-product-research

# 2. 查看最新調研報告
cat bottlenecks/weekly-2026-W29.md

# 3. 新增你的調研報告
# 按照現有格式新增新的調研文件到對應資料夾
```

## ✨ 功能特色

| 分類 | 說明 | 目錄 |
|------|------|------|
| 📊 **市場趨勢分析** | 追蹤市場變化、識別新興趨勢與機會 | `market-trends/` |
| 🔴 **瓶頸分析** | 透過轉換漏斗分析找出銷售瓶頸與客戶流失原因 | `bottlenecks/` |
| 🟡 **競爭對手調查** | 競品定價、功能、市場策略的深度分析 | `competitor-analysis/` |
| 📈 **產品潛力評估** | 自動觸發機制評估產品成長潛力 | `product-evaluation/` |
| 🟢 **促銷策略指南** | 折扣策略、捆绑銷售、限時促銷實戰指南 | `promotional-strategies/` |
| 🟣 **定價研究** | 價格彈性分析、市場定價基準 | `pricing-research/` |
| 🔵 **行銷渠道分析** | 各渠道 ROI、CAC、轉換率追蹤 | `marketing-channels/` |

## 🚨 調研觸發條件

當以下任一條件達成時，自動啟動深度研究：

| 條件 | 閾值 |
|------|------|
| 收入下滑 | 連續 4 週收入低於 $50 |
| 低轉換率 | 轉換率 < 1% |
| 高退款率 | 退款率 > 10% |
| 流量停滯 | 每週增長 < 5% |
| 競爭威脅 | 競爭對手推出新產品 |

## 📐 研究方法論

1. **數據收集** — 從 product-tracking 系統匯總銷售數據
2. **觸發評估** — 檢查當前指標是否符合觸發條件
3. **針對性研究** — 聚焦特定瓶頸分類
4. **報告生成** — 產出可操作的調研結果
5. **建議方案** — 具體可行的下一步建議

### 報告格式

每份調研報告遵循標準格式：

```
標題：[調研分類] — [日期]
觸發條件：[觸發研究的條件]
數據週期：[分析的日期範圍]
發現：
  - 關鍵發現 1
  - 關鍵發現 2
建議：
  - 具體行動項目 1
  - 具體行動項目 2
```

### 常見發現

基於跨多個數位商品類別的重複分析模式：

- **定價差距** — $29–$69 區間產品的轉換率比高價產品高出 2-3 倍
- **渠道集中** — 超過 70% 流量來自單一來源，需要分散
- **內容缺口** — 有詳細操作說明的產品退款率低 40%
- **時機模式** — 週末發布的產品比平日發布高出 25-35%

## 📁 專案結構

```
digital-product-research/
├── bottlenecks/              # 瓶頸分析報告
│   └── weekly-2026-W29.md
├── promotional-strategies/   # 促銷策略指南
│   └── gumroad-upload-guide.md
├── competitor-analysis/      # 競品分析（待新增）
├── marketing-channels/       # 行銷渠道分析（待新增）
├── pricing-research/         # 定價研究（待新增）
├── .github/                  # GitHub 設定檔
│   ├── ISSUE_TEMPLATE/       # Issue 模板
│   │   ├── bug_report.md
│   │   └── feature_request.md
│   └── PULL_REQUEST_TEMPLATE.md
├── CODE_OF_CONDUCT.md        # 行為準則
├── SUPPORT.md                # 支援文件
├── LICENSE                   # MIT 授權
└── README.md
```

## 🔗 相關專案

- [📈 Product Tracking](https://github.com/ckw19810413/product-tracking) — 數位商品銷售追蹤工具
- [📄 Digital Product Landing](https://github.com/ckw19810413/digital-product-landing) — 數位商品 Landing Page
- [📦 Gumroad Products](https://github.com/ckw19810413/gumroad-products) — Gumroad 上架產品包
- [🎓 AI 實戰課程](https://github.com/ckw19810413/ai-practical-course-tw) — 繁體中文 AI 課程
- [🎮 Qwen3.6-27B Tiny Games](https://github.com/ckw19810413/qwen3.6-27b-tiny-games) — AI 生成的微型遊戲

## 📜 授權

[MIT License](LICENSE) — 自由使用、修改、分享。

---

Made with ❤️ by [KWC](https://github.com/ckw19810413)