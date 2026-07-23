# 數位商品行銷行動計畫 — 2026-W32

**制定日期:** 2026-07-23
**行動期間:** 2026-07-24 ~ 2026-07-30
**目標:** 建立初始流量管道，啟動社群存在

---

## 第一週行動目標（W32）

### 已完成準備工作 ✅

| 項目 | 狀態 | 備註 |
|------|------|------|
| Gumroad 產品上架 | ✅ 6 個產品 | 已驗證 |
| Landing Page 開發 | ✅ Next.js 專案 | digital-product-landing repo |
| 每週收入追蹤 | ✅ cron job 自動執行 | product-tracking repo |
| 瓶頸自動偵測 | ✅ cron job 每日執行 | digital-product-research repo |
| Twitter 內容日曆 | ✅ 7 則推文準備 | marketing-assets/ |
| Twitter 自動發送 | ⚠️ 待修復 | OAuth 2.0 憑證問題 |
| 封面圖生成 | ❌ 待部署 | 需要 ComfyUI/Flux 環境 |

### 本週待執行重點 🎯

---

## 🔴 緊急：Twitter API 憑證問題

**問題：** X (Twitter) API 憑證已失效
- 錯誤訊息：`invalid_client — Value passed for the client id was invalid`
- 可能原因：API Key/Secret 已過期或被吊销
- **需要用戶行動：** 前往 [X Developer Portal](https://developer.x.com/) 重新生成憑證

**步驟：**
1. 登入 https://developer.x.com/
2. 進入 Project → App Settings
3. 重新生成 API Key 和 API Secret
4. 更新 `/home/wayne/.priv/twitter-api-config-digitalproducttw.env`

**臨時替代方案：**
- 手動發送推文（使用 Twitter Web UI 或 X App）
- 使用 Buffer/Later 等第三方工具排程
- 先專注於內容策略，等憑證恢復再自動化

---

## 📋 本週執行清單

### 第 1-2 天（7/24-25）：基礎建設

- [ ] **手動發布第一則 Twitter 推文**
  - 內容：痛點共鳴帖（準備好的 7 則之一）
  - 目的：測試帳號是否正常工作
  - 目標：@digitalProductTW 帳號開始有內容

- [ ] **部署 Landing Page 到 Vercel/Cloudflare**
  - 選項 A：Vercel（推薦，自動部署）
    - 帳號：需要 Vercel 帳號
    - 命令：`vercel deploy --prod`
  - 選項 B：Cloudflare Pages
    - 需要 Cloudflare API Token
    - 執行：`bash scripts/cloudflare-deploy.sh`

- [ ] **建立 Twitter/X 帳號內容計畫**
  - 帳號：@digitalProductTW
  - Bio 內容："🤖 繁體中文 AI 工具與數位生產力 | 每週分享 AI 實戰技巧 | 產品：AI Prompt 庫、AI 課程、飛書模板、ETF 儀表板"
  - 頭像：使用專案 Logo 或品牌形象圖

### 第 3-4 天（7/26-27）：內容行銷啟動

- [ ] **開始 Twitter 每日發文**
  - 頻率：每天 1 則（逐步增加到 2-3 則）
  - 類型：教育內容 → 價值輸出 → 產品介紹
  - 目標：第一週累積 5 則推文

- [ ] **創建 Landing Page 免費資源**
  - 內容：免費 AI Prompt 樣本（5 個）
  - 目的：建立 Email List
  - 工具：Gumroad 免費產品 + 電子報訂閱表單

- [ ] **加入 Reddit 社群**
  - 目標子版面：r/ChatGPT, r/AI, r/Productivity
  - 行動：每週 2-3 則有意義的回應（不是推銷）
  - 目標：建立 Reddit 帳號信誉

### 第 5-7 天（7/28-30）：流量測試

- [ ] **評估 Landing Page 效果**
  - 檢查 Vercel/Cloudflare 部署是否成功
  - 驗證所有產品連結是否正確
  - 測試行動裝置顯示效果

- [ ] **開始 Email List 收集**
  - 如果 Landing Page 已部署
  - 加入 Newsletter Signup 表單
  - 發送第一則電子報（價值內容）

- [ ] **準備第二週推文內容**
  - 增加產品介紹貼文
  - 增加客戶回饋/案例分享
  - 增加工具推薦貼文

---

## 📊 本週 KPI 目標

| 指標 | 目標值 | 測量方式 |
|------|--------|---------|
| Twitter 推文數 | 3-5 則 | Twitter Analytics |
| Landing Page 上線 | ✅ | 網站可訪問 |
| Email List 建立 | 10+ 人 | Email 工具 |
| Reddit 參與 | 5 次有意義回應 | 手動記錄 |
| 總訪客數 | 50+ | Google Analytics |
| 產品點擊 | 10+ 次 | Gumroad Dashboard |

---

## 🔧 技術待辦事項

### 高優先級（本週）

1. **Twitter API 憑證更新** ⚠️ 緊急
   - 用戶需前往 X Developer Portal 重新生成
   - 更新後運行：`python3 scripts/twitter-auto-post.py refresh`

2. **Landing Page 部署**
   - 已準備好 Next.js 專案（digital-product-landing）
   - 需要選擇部署平台：Vercel 或 Cloudflare
   - 執行部署後更新 Gumroad 產品頁面連結

3. **Flux 封面圖生成**
   - 需要 ComfyUI 環境配置
   - 2 個產品缺封面：AI 實戰課程、飛書模板市集
   - 有 Flux 模型可本地生成

### 中優先級（W33+）

4. **SEO 優化 Landing Page**
   - 增加 meta tags 和 OG 圖片
   - 建立 sitemap.xml
   - 加入 Google Search Console

5. **社群媒體擴展**
   - 建立 LinkedIn 頁面
   - 建立 YouTube 短影片頻道
   - 考慮 Medium 部落格

6. **產品評價系統**
   - 向早期用戶收集評價
   - 在 Gumroad 頁面展示評價
   - 增加 Landing Page Testimonials 區

---

## 💰 資源分配建議

### 時間分配（每週）

| 活動 | 時間 | 預期回報 |
|------|------|---------|
| Twitter 發文 | 2 小時 | 品牌曝光 |
| Reddit 參與 | 2 小時 | 精準流量 |
| Landing Page 優化 | 3 小時 | 轉換率提升 |
| 內容規劃 | 2 小時 | 持續性 |
| **總計** | **9 小時** | **基礎建設** |

### 成本預估

| 項目 | 成本 | 備註 |
|------|------|------|
| Vercel 部署 | $0 | 免費方案 |
| Cloudflare Pages | $0 | 免費方案 |
| Email 工具 | $0-20/月 | MailerLite 免費 |
| Twitter 廣告 | $0-100/月 | 可選，初期不建議 |
| **總計** | **$0-120/月** | **低成本啟動** |

---

## ⚠️ 風險與應對

### 已知風險

1. **Twitter API 憑證失效**
   - 影響：自動發文中斷
   - 應對：手動發文 + 第三方工具
   - 嚴重程度：高

2. **零銷售起始點**
   - 影響：士氣低落
   - 應對：聚焦過程（發文、參與），非結果（銷售）
   - 嚴重程度：中

3. **Flux 封面圖未生成**
   - 影響：部分產品頁面不美觀
   - 應對：使用 Canva 手動設計
   - 嚴重程度：低

### 成功關鍵因素

1. **一致性** — 每天發文，每週更新 Landing Page
2. **價值優先** — 80% 教育內容，20% 推銷
3. **互動** — 回應每一則評論和私信
4. **數據驅動** — 每週檢視 Analytics，調整策略

---

## 📈 下週（W33）展望

如果本週目標達成：
- Twitter 帳號建立初始存在感（50+ 追蹤者）
- Landing Page 開始收到自然流量
- Email List 建立基礎
- 第二週內容策略可基於數據調整

**預期下週重點：**
- 根據第一週數據優化內容方向
- 開始小規模 Twitter 廣告測試（$5-10）
- 增加 YouTube 短影片內容
- 評估第一個產品銷售情況

---

*本計畫於 2026-07-23 制定*
*下次檢視：2026-07-28（W33 週報時）*