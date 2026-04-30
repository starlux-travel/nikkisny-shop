# 🚀 nikkisny.shop 部署上線指引

> 📅 建立日期：2026-04-30
> 🎯 目標：讓 nikkisny.shop 透過 Vercel 正式上線

---

## 📋 整體流程

```
本機 VSCode → Git Push → GitHub Repo → Vercel 自動部署 → 設定 DNS → 網站上線 ✅
```

---

## STEP 1：確認 index.html 已儲存

在 VSCode 中：
- 按 **Ctrl + S** 儲存
- 或 **File → Save All**（儲存所有檔案）

確認 `index.html` 是最新版本。

---

## STEP 2：Git Push 上傳到 GitHub

在 VSCode 內開啟 Terminal（Ctrl + ` ），複製貼上以下指令：

```bash
# 進入你的專案資料夾
cd "C:\Users\sam82\OneDrive\桌面\nikkisny.shop"

# 查看目前狀態（確認有 index.html 需要上傳）
git status

# 加入所有變更
git add .

# 建立 commit（說明這次更新）
git commit -m "Update: 完成首頁設計 - 代購網站正式版"

# 推送到 GitHub
git push origin main
```

✅ 完成後去 https://github.com/starlux-travel/nikkisny-shop 確認 index.html 是最新版。

---

## STEP 3：Vercel 匯入 GitHub 專案

1. 前往 https://vercel.com → 登入帳號（nickeyara-3876）
2. 點擊右上角 **「Add New...」→「Project」**
3. 點 **「Import Git Repository」**
4. 選擇 GitHub 帳號 **starlux-travel**
5. 找到 repo **nikkisny-shop** → 點 **Import**
6. 設定頁面：
   - **Framework Preset**：選 `Other`（因為是純 HTML，不是 Next.js）
   - **Root Directory**：保持 `./`（預設）
   - **Build Command**：**留空**
   - **Output Directory**：**留空**（或填 `.`）
7. 點 **Deploy** 🚀

等待約 30 秒 → 你會看到 Vercel 給你一個臨時網址（例如 `nikkisny-shop.vercel.app`）  
→ 點開確認網站正常顯示！

---

## STEP 4：綁定自訂網域 nikkisny.shop

### 4-1 在 Vercel 新增網域

1. 進入你的 Vercel 專案（nikkisny-shop）
2. 點上方 **Settings** → 左側 **Domains**
3. 輸入：`nikkisny.shop` → 點 **Add**
4. 也再加一次：`www.nikkisny.shop`
5. Vercel 會顯示需要設定的 DNS 記錄，**先截圖或抄下來**

你會看到類似這樣的資訊：
```
Type: A
Name: @
Value: 76.76.21.21

Type: CNAME
Name: www
Value: cname.vercel-dns.com
```

### 4-2 在 Porkbun 設定 DNS

1. 前往 https://porkbun.com → 登入
2. 點 **Domains** → 找到 `nikkisny.shop` → 點 **Details**（或右側齒輪）
3. 找到 **DNS** 設定（左側選單 DNS Records）
4. 刪除現有 A 記錄（如果有的話）
5. 新增以下記錄：

| Type | Host | Answer/Value | TTL |
|------|------|-------------|-----|
| A | @ | 76.76.21.21 | 600 |
| CNAME | www | cname.vercel-dns.com | 600 |

6. 儲存設定

> ⚠️ DNS 傳播需要 **5~30 分鐘**，最長可能 24 小時。
> 可以用 https://dnschecker.org 查詢 nikkisny.shop 是否已生效。

---

## STEP 5：Vercel 自動申請 SSL 憑證

綁定網域後，Vercel 會自動幫你申請免費 SSL（https://）  
→ 等 DNS 生效後，https://nikkisny.shop 就可以正常訪問！

---

## 🎉 完成清單

- [ ] STEP 1：index.html 已儲存
- [ ] STEP 2：git push 成功
- [ ] STEP 3：Vercel 部署成功（看到臨時網址）
- [ ] STEP 4-1：Vercel 新增 nikkisny.shop 網域
- [ ] STEP 4-2：Porkbun DNS 設定完成
- [ ] STEP 5：https://nikkisny.shop 正常開啟 ✅

---

## 🔄 之後更新網站的流程

每次你修改 index.html，只需要：

```bash
cd "C:\Users\sam82\OneDrive\桌面\nikkisny.shop"
git add .
git commit -m "Update: 說明你改了什麼"
git push origin main
```

Vercel 會**自動偵測** GitHub 有新的 push → **自動重新部署** ✅  
不需要手動操作 Vercel！

---

## ❓ 常見問題

**Q：git push 時要輸入密碼？**  
A：GitHub 已不支援密碼，需要用 Personal Access Token（PAT）或 SSH。  
建議用 GitHub Desktop 最簡單：https://desktop.github.com/

**Q：Vercel 顯示 404？**  
A：確認 `index.html` 在 repo 根目錄（不是在子資料夾）

**Q：DNS 設好但網站還是打不開？**  
A：等 30 分鐘再試，或用無痕模式測試。

**Q：想改開團內容怎麼辦？**  
A：直接在 VSCode 修改 index.html → 存檔 → git push → 自動上線
