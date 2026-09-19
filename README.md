# GitHub Repos Directory

純前端單頁網站，48 筆 GitHub repo 導覽，可搜尋、可依分類篩選、可複製連結或直接開啟。無外部字型或 CDN 依賴，`index.html` 單檔即可部署。

## 部署到 GitHub Pages

1. 建立一個 repo（或使用現有的），將 `index.html` 放在根目錄（或 `docs/` 資料夾）。
2. GitHub repo 設定 → Pages → Source 選擇對應分支/資料夾 → Save。
3. 幾分鐘後即可透過 `https://<你的帳號>.github.io/<repo名稱>/` 存取。

## 這次的修正紀錄（相對於你上傳的舊版）

【確認】以下每一項都是我實際用工具查詢 github.com 後得到的結果，而非憑印象判斷。

### 1. 移除 2 筆重複連結
原始資料共 50 筆，其中：
- #48（標題「system design + interview prep extras」）網址與 #7（`jwasham/coding-interview-university`）完全相同，已移除 #48。
- #50（標題「automation + AI workflows」）網址與 #19（`n8n-io/n8n`）完全相同，已移除 #50。

移除後剩 **48 筆不重複項目**。

### 2. 分類數量修正
舊版標示「8 CATEGORIES」，但篩選器裡的 8 個選項包含 "All"（全部），實際分類只有 **7 個**：AI Core、Agents & Automation、Chat & UI、Dev Tools、Learn & Interview、Memory & RAG、Security & OSINT。新版已改為「48 個 repo · 7 個分類」。

### 3. 5 筆連結指向已改名/轉移的 repo，已更新為目前網址
用 WebFetch 實際開啟每個連結後發現以下 repo 的擁有者或名稱已變更（原網址仍會透過 GitHub 的自動轉址生效，但顯示已非目前名稱）：

| # | 原網址 | 目前網址 | 備註 |
|---|---|---|---|
| 3 | `danistefanovic/build-your-own-x` | `codecrafters-io/build-your-own-x` | 專案轉移組織，已存在多年（Internet Archive 可查到 2022 年紀錄） |
| 4 | `kamranahmedse/developer-roadmap` | `nilbuild/developer-roadmap` | 專案轉移組織 |
| 26 | `geekan/MetaGPT` | `FoundationAgents/MetaGPT` | 專案轉移組織 |
| 34 | `mendableai/firecrawl` | `firecrawl/firecrawl` | 專案轉移組織；舊網址在查詢時回傳 503 錯誤，新網址正常 |
| 46 | `lobehub/lobe-chat` | `lobehub/lobehub` | 專案**改名且重新定位**：原本是「Lobe Chat」AI 聊天框架，目前 repo 說明已改為「Chief Agent Operator」代理程式營運平台，因此頁面上的 tagline/description 也一併更新，不再是「AI chat framework」 |

### 4. 2 筆連結指向組織首頁，非單一 repo
- #45 `github.com/deepseek-ai`（DeepSeek）
- #49 `github.com/langchain-ai`（AI agents ecosystem）

這兩筆原始資料的描述本來就是「curated resources / AI models and research」這類組織層級的敘述，符合連到組織首頁的用法，因此保留原網址，但在卡片上加註「組織首頁」標籤，避免使用者誤以為是單一 repo。

### 5. 未做的事
- 沒有加上 star 數、fork 數等統計數字——這類數字會隨時間變動，寫死在頁面裡很快就會過時且無法驗證，因此沒有加入。
- 除了上述表格列出的 5 筆，其餘 43 筆連結經逐一以 WebFetch 開啟確認，標題與目前 GitHub 頁面一致，未發現其他 404 或改名。

## 檔案結構

```
index.html   ← 唯一需要的檔案，資料已內嵌，無需額外請求
README.md    ← 本說明檔（不影響網站運作，僅供留存修正紀錄）
```
