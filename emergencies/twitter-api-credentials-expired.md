# 緊急：Twitter API 憑證已失效

**發現日期：** 2026-07-23
**嚴重程度：** 🔴 Critical
**影響：** Twitter 自動發文系統完全無法運作

## 問題描述

所有 Twitter API 認證方式均失敗：
- OAuth 2.0 Client Credentials：`invalid_client — Value passed for the client id was invalid`
- OAuth 2.0 Refresh Token：同樣錯誤
- 現有的 Access Token：`401 Unauthorized`

## 原因分析

1. **API Key/Secret 已過期** — X Developer Portal 的憑證有時效
2. **App 權限被撤回** — 可能 App 被移除或權限被變更
3. **Account 狀態異常** — X 帳號可能有問題

## 修復步驟（需要用戶操作）

### 步驟 1：確認 X Developer Portal 狀態
1. 前往 https://developer.x.com/
2. 登入 `@digitalProductTW` 對應的帳號
3. 確認 App 仍在列表中且狀態正常

### 步驟 2：重新生成憑證
1. 進入 Project → App Settings
2. 如果 App 已刪除，重新創建 App
3. 生成新的 API Key 和 API Secret
4. 確保權限包含：`tweet.read`, `tweet.write`, `users.read`

### 步驟 3：更新憑證文件
將新的 API Key 和 Secret 填入：
```
/home/wayne/.priv/twitter-api-config-digitalproducttw.env
```

### 步驟 4：測試
```bash
python3 /home/wayne/workspace/github/ckw19810413/product-tracking/scripts/twitter-auto-post.py refresh
python3 /home/wayne/workspace/github/ckw19810413/product-tracking/scripts/twitter-auto-post.py send
```

## 臨時替代方案

在 Twitter API 恢復前，可以使用：
1. **手動發文** — 使用 X App 或 Web 介面
2. **Buffer** — 第三方社群媒體管理工具（免費方案）
3. **Later.com** — 另一款社群排程工具
4. **Hootsuite** — 企業級社群管理（免費方案有限）

## 相關檔案

- Twitter API 配置：`/home/wayne/.priv/twitter-api-config-digitalproducttw.env`
- 自動發文腳本：`/home/wayne/workspace/github/ckw19810413/product-tracking/scripts/twitter-auto-post.py`
- 推文內容日曆：`/home/wayne/workspace/github/ckw19810413/product-tracking/marketing-assets/twitter-x-content-calendar.json`
- 已推文記錄：`/home/wayne/workspace/github/ckw19810413/product-tracking/data/tweet-sent.json`

## 備註

- 此問題不影響其他自動化系統（Gumroad 收入追蹤、Landing Page、瓶頸偵測）
- 只有 Twitter 自動發文功能無法使用
- 7 則推文內容已準備好，等待憑證恢復後可立即使用