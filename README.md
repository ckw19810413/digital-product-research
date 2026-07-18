# digital-product-research

一個用於數位產品市場調查與分析的開源工具集，協助創作者找出高潛力產品點子。

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Last Updated](https://img.shields.io/badge/last%20updated-2025-brightgreen.svg) ![Stars](https://img.shields.io/github/stars/ckw19810413/digital-product-research?style=social) ![Repo Size](https://img.shields.io/github/repo-size/ckw19810413/digital-product-research)

## 📋 目錄
- [快速開始](#快速開始)
- [功能特色](#功能特色)
- [專案結構](#專案結構)
- [使用案例](#使用案例)
- [相關專案](#相關專案)

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

## ✨ 功能特色

- 📊 **市場趨勢分析** — 追蹤市場變化、識別新興趨勢與機會
- 🔴 **瓶頸分析** — 透過轉換漏斗分析找出銷售瓶頸與客戶流失原因
- 🟡 **競爭對手調查** — 競品定價、功能、市場策略的深度分析
- 📈 **產品潛力評估** — 自動觸發機制評估產品成長潛力
- 🟢 **促銷策略指南** — 折扣策略、捆绑銷售、限時促銷實戰指南
- 🟣 **定價研究** — 價格彈性分析、市場定價基準
- 🔵 **行銷渠道分析** — 各渠道 ROI、CAC、轉換率追蹤

### 調研觸發條件

當以下任一條件成立時，自動啟動深度調研：

- [ ] 連續 4 週收入 < $50
- [ ] 轉換率 < 1%
- [ ] 退款率 > 10%
- [ ] 流量增長停滯（周增長 < 5%）
- [ ] 競品推出新產品

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

## 🎯 使用案例

- 🔍 尋找下一個熱門數位產品
- 📊 分析市場需求與供給
- 🎯 評估產品進入點
- 📈 數位商品創作者定期檢視銷售表現
- 🧩 團隊結構化的問題診斷流程
- 📝 數據驅動的產品迭代依據
- 📣 競品和市場分析框架

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

## 📜 授權

MIT License

---

Made with ❤️ by [KWC](https://github.com/ckw19810413)