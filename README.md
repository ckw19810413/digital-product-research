# 🔍 數位商品銷售深度調研報告

> 當銷售遇到瓶頸時自動觸發的深度調研報告。用數據驅動決策，找到增長機會。

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Last Updated](https://img.shields.io/badge/Last_Updated-2026--07-green.svg)]()

## 📋 目錄

- [快速開始](#快速開始)
- [調研觸發條件](#調研觸發條件)
- [調研分類](#調研分類)
- [專案結構](#專案結構)
- [使用方式](#使用方式)
- [貢獻指南](#貢獻指南)
- [相關專案](#相關專案)
- [授權條款](#授權條款)

## 🚀 快速開始

這個專案提供了一套完整的數位商品銷售調研框架，幫助你在銷售遇到瓶頸時快速定位問題、找到解決方案。

```bash
# 1. 克隆此倉庫
git clone https://github.com/ckw19810413/digital-product-research.git
cd digital-product-research

# 2. 查看調研報告
cat bottlenecks/weekly-2026-W29.md

# 3. 新增你的調研報告
# 按照現有格式新增新的調研文件到對應資料夾
```

## ⚠️ 調研觸發條件

當以下任一條件成立時，自動啟動深度調研：

- [ ] 連續 4 週收入 < $50
- [ ] 轉換率 < 1%
- [ ] 退款率 > 10%
- [ ] 流量增長停滯（周增長 < 5%）
- [ ] 競品推出新產品

## 📊 調研分類

| 分類 | 內容 | 檔案路徑 |
|------|------|---------|
| 🔴 瓶頸分析 | 轉換漏斗瓶頸、客戶流失原因 | `bottlenecks/` |
| 🟡 競品分析 | 競品定價、功能、市場策略 | `competitor-analysis/` |
| 🔵 行銷渠道 | 各渠道 ROI、CAC、轉換率 | `marketing-channels/` |
| 🟢 促銷策略 | 折扣策略、捆绑銷售、限時促銷 | `promotional-strategies/` |
| 🟣 定價研究 | 價格彈性、市場定價基準 | `pricing-research/` |

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
│   └── PULL_REQUEST_TEMPLATE.md
├── CODE_OF_CONDUCT.md        # 行為準則
├── SUPPORT.md                # 支援文件
├── LICENSE                   # MIT 授權
└── README.md
```

## 💡 關鍵功能

- 🎯 **自動觸發機制**：明確的觸發條件，知道何時該調研
- 📊 **多維度分析**：涵蓋瓶頸、競品、行銷、促銷、定價五大面向
- 📝 **報告模板化**：標準化格式，每次調研都有完整記錄
- 🔄 **持續迭代**：每週更新，追蹤趨勢變化

## 🎯 適用場景

- 數位商品創作者需要定期檢視銷售表現
- 團隊需要結構化的問題診斷流程
- 產品經理需要數據驅動的產品迭代依據
- 行銷人員需要競品和市場分析框架

## 🔗 相關專案

- [📈 Product Tracking](https://github.com/ckw19810413/product-tracking) — 數位商品銷售追蹤工具
- [🎮 Qwen3.6-27B Tiny Games](https://github.com/ckw19810413/qwen3.6-27b-tiny-games) — AI 生成的微型遊戲
- [📄 Digital Product Landing](https://github.com/ckw19810413/digital-product-landing) — 數位商品 Landing Page
- [📦 Gumroad Products](https://github.com/ckw19810413/gumroad-products) — Gumroad 上架產品包

## 🤝 貢獻指南

歡迎貢獻！請先 Fork 此專案，然後建立 Pull Request：

1. Fork 本仓库
2. 建立特性分支 (`git checkout -b feature/amazing`)
3. 提交變更 (`git commit -m '新增 amazing 功能'`)
4. 推送到分支 (`git push origin feature/amazing`)
5. 開啟 Pull Request

請確保：
- 遵循 [行為準則](CODE_OF_CONDUCT.md)
- 使用 [Issue Templates](.github/ISSUE_TEMPLATE/) 回報問題
- 使用 [PR Templates](.github/PULL_REQUEST_TEMPLATE.md) 提交變更

## 📜 授權條款

本專案採用 [MIT License](LICENSE) 授權。