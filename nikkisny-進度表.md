# 🛍️ Nikki's NY Shop（nikkisny.shop）代購系統 進度表

> 📅 建立日期：2026-04-30
> 👤 負責人：Nikki
> 🎯 短期目標：先上線一個漂亮的首頁

---

## 📋 專案基本資訊

| 項目 | 內容 |
|------|------|
| 網站名稱 | Nikki's NY Shop |
| 網域 | nikkisny.shop |
| 網域購買處 | Porkbun |
| 網域到期日 | 2027-04-25 |
| GitHub 帳號 | starlux-travel |
| GitHub Repo | starlux-travel/nikkisny-shop |
| 部署平台 | Vercel（規劃中） |
| 銀行帳戶 | 中國信託 (822) 新店分行 |
| FB 粉專 | https://www.facebook.com/nikkinyshop/ |
| Messenger | https://m.me/hsiaoliliu |
| 開發工具 | VSCode + Live Server |
| 程式碼 | 純 HTML + CSS（單一檔案） |

---

## ✅ 已完成

### 🌐 網域 & 帳號（早上之前）
- [x] 買了 nikkisny.shop 網域（Porkbun）
- [x] 建立 GitHub 帳號（starlux-travel）
- [x] 建立 GitHub repo（nikkisny-shop）
- [x] 設定 GitHub OAuth App
- [x] 完成 GitHub 第一次 commit
- [x] 申請 Vercel 帳號

### 💻 開發環境（今天上午）
- [x] VSCode 已安裝
- [x] Live Server 擴充功能已安裝
- [x] 學會用 Live Server 預覽網頁

### 🎨 首頁設計（今天上午）
- [x] 確定設計風格：精品柔和女性風
- [x] 確定配色：Happy Hues Palette #11
- [x] 確定字體：Quicksand + Noto Sans TC
- [x] 完成首頁 HTML/CSS 程式碼
- [x] 移除所有深藍黑背景（只用在文字）

### 📐 首頁區塊
- [x] 頂部公告條
- [x] Header + Logo + 導覽
- [x] Hero 主視覺
- [x] 數據條（100% / $4000 / FedEx / 21-28天）
- [x] 開團區塊（3 張卡片）
- [x] 雙色塊 CTA（詢價 vs 現貨）
- [x] 品牌跑馬燈
- [x] Footer
- [x] 響應式設計
- [x] 進場動畫

---

## 🚧 進行中

### 🚀 上線部署（現在做這個！）
> 📄 詳細步驟請看同資料夾的：`部署指引-Vercel上線.md`

- [ ] **STEP 1**：VSCode 確認 index.html 已儲存（Ctrl+S）
- [ ] **STEP 2**：git push 到 GitHub（見指引 STEP 2 的指令）
- [ ] **STEP 3**：Vercel 匯入 GitHub repo → 選 `Other` 框架 → Deploy
- [ ] **STEP 4**：Vercel 設定自訂網域 nikkisny.shop
- [ ] **STEP 5**：Porkbun DNS 加 A Record + CNAME（見指引 STEP 4）
- [ ] **STEP 6**：等 DNS 生效（5~30 分鐘）→ 測試 https://nikkisny.shop

---

## 📋 之後要做的

### 🥇 上線後立刻做
- [ ] 填入真實銀行帳號
- [ ] 確認所有連結
- [ ] 在 FB 宣傳上線

### 🥈 本週內
- [ ] 加入詢價表單頁面
- [ ] 加入後台管理
- [ ] 加入訂單追蹤功能

### 🥉 之後
- [ ] 加入完整開團系統
- [ ] 加入品牌故事區
- [ ] 加入運費試算機
- [ ] 加入會員規則頁面

---

## 🎨 設計規範（已確定）

### 顏色
- 背景：#f9f4ef（米白）
- 標題：#020826（深藍黑，只用在字）
- 內文：#716040（棕褐）
- 按鈕：#8c7851（卡其棕）
- 強調：#f25042（珊瑚紅）
- 副色：#eaddcf（淺米）

### 字體
- 英文標題：Quicksand
- 中文：Noto Sans TC（源黑體）

### 風格
- 精品柔和女性風
- 紐約品味、溫暖親切
- 不用深色背景，深色只用在文字

---

## ⚠️ 商業規則

### 收款
- ✅ ATM 轉帳、現金匯存
- ❌ 不刷卡、不貨到付款

### 運費
- 國際運費：每磅 NT$240（含關稅）
- 台灣轉運：NT$80（滿 NT$4,000 免）
- 鞋盒加購：+NT$300
- 黑貓宅配：+NT$170（精品/貴重免費）
- 匯率：當日 +1

### 出貨時間
- 匯款後 21-28 天

### 不代購
- 香水、液體、藥品、蠟燭、咖啡
- 食物、寵物食品、3C 電子
- 保健食品、Outlet 商品

---

## 🔧 常用指令備忘

### Git 指令
```bash
git status              # 看目前狀態
git add .               # 加入所有變更
git commit -m "說明"    # commit
git push                # 推到 GitHub
```

### VSCode 快捷鍵
- 儲存所有檔案：`Ctrl + K` 然後 `S`
- Live Server 預覽：右下角「Go Live」按鈕

---

## 📅 變更紀錄

| 日期 | 內容 |
|------|------|
| 2026-04-30 早 | 建立進度表，重新開始做網站 |
| 2026-04-30 早 | 完成首頁 v1（深藍黑配色） |
| 2026-04-30 早 | v2：移除深色背景 |
| 2026-04-30 早 | v3：字體換成 Quicksand 圓圓體 ✨ |
| 2026-04-30 下午 | 靜態網站部署上線 nikkisny.shop（Vercel + Porkbun DNS）✅ |
| 2026-04-30 下午 | 啟動 Django 後台系統（nikkisny-django 資料夾）|
| 2026-04-30 下午 | 完成 Django 6 個 App 架構 + Migration |
| 2026-04-30 下午 | orders/models.py：9段訂單狀態 + 物流追蹤 ✅ |
| 2026-04-30 下午 | products/models.py：開團/現貨/詢價商品模型 ✅ |
| 2026-04-30 下午 | notifications/service.py：LINE Notify 全流程通知 ✅ |
| 2026-04-30 下午 | orders/admin.py：後台一鍵更新狀態 + 自動 LINE 通知 ✅ |
| 2026-04-30 下午 | accounts/models.py：UserProfile + LINE token 綁定 ✅ |
| 2026-04-30 下午 | products/admin.py：一鍵發布到 FB 社團 + LINE 廣播 ✅ |
| 2026-04-30 下午 | publishing/service.py：FB Graph API + LINE Messaging ✅ |
| 2026-04-30 下午 | accounts/views.py：登入/註冊/個人頁 ✅ |
| 2026-04-30 下午 | Django system check 零錯誤 ✅ |

---

## 🐍 Django 後台系統架構（nikkisny-django）

### ✅ 已完成的模組
| 檔案 | 功能 |
|------|------|
| `orders/models.py` | 訂單模型（9 段狀態 + 物流追蹤）|
| `orders/admin.py` | 後台一鍵改狀態 + 自動 LINE 通知 |
| `products/models.py` | 商品模型（開團/現貨/詢價）|
| `products/admin.py` | 後台一鍵發布到 FB + LINE |
| `notifications/service.py` | LINE Notify 通知（全 9 種模板）|
| `publishing/service.py` | FB Graph API + LINE Messaging API |
| `accounts/models.py` | UserProfile（LINE token + 客戶類型）|
| `accounts/admin.py` | 後台客戶管理（顯示 LINE 綁定狀態）|
| `accounts/views.py` | 前台登入/註冊/個人頁 |

### 🚧 下一步（Django 繼續）
- [ ] `products/views.py` — 商品列表頁、開團詳細頁
- [ ] `products/urls.py` — 商品 URL 路由
- [ ] 購物車 `cart` app — 加入購物車、查看購物車
- [ ] 結帳頁 `orders/views.py` — 填寫收件資訊 + 顯示匯款帳號
- [ ] `inquiry/models.py` — 詢價單模型
- [ ] 前台 templates（套用 nikkisny.shop 設計風格）
- [ ] Railway 部署設定（Procfile + railway.json）
- [ ] 切換 nikkisny.shop DNS → Railway

### 🔑 需要設定的 API Keys（在 .env 裡）
| 變數 | 用途 | 去哪拿 |
|------|------|--------|
| `NIKKI_LINE_NOTIFY_TOKEN` | Nikki 自己收新訂單通知 | notify.line.me |
| `LINE_CHANNEL_ACCESS_TOKEN` | 廣播給所有 LINE 追蹤者 | LINE Developers |
| `FACEBOOK_PAGE_ACCESS_TOKEN` | 發文到 FB 社團 | Meta for Developers |
| `FACEBOOK_GROUP_ID` | FB 社團 ID | FB 社團網址的數字 |
| `BANK_ACCOUNT_NAME` | 匯款通知顯示戶名 | 你的帳戶 |
| `BANK_ACCOUNT_NUMBER` | 匯款通知顯示帳號 | 你的帳戶 |

---

## 🎯 下一個里程碑

**讓 Django 後台可以跑 + 部署到 Railway！** 🚀
