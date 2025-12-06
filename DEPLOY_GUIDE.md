# 🚀 Lazarus Master - Render 部署指南

## 📋 部署步驟（5 分鐘完成）

### 步驟 1：註冊 Render 帳號

1. 去 **https://render.com**
2. 點擊右上角 **「Sign Up」**
3. 用 **Google** 或 **GitHub** 帳號登入（最快）
4. 或者用 Email 註冊

> 💡 **提示：** Render 免費版已經足夠使用，唔需要信用卡。

---

### 步驟 2：建立新 Web Service

1. 登入後，點擊 **「New +」** → **「Web Service」**
2. 選擇 **「Build and deploy from a Git repository」**
3. 點擊 **「Public Git repository」**
4. 輸入你嘅 GitHub 倉庫 URL（如果你已經上傳到 GitHub）

**或者用手動部署（更簡單）：**

1. 點擊 **「New +」** → **「Web Service」**
2. 選擇 **「Deploy from GitHub」** 下面嘅 **「Or, deploy without connecting to Git」**
3. 上傳 ZIP 檔案（我已經準備好）

---

### 步驟 3：配置部署設定

填寫以下資訊：

| 欄位 | 值 |
|------|-----|
| **Name** | `lazarus-master`（或你喜歡嘅名稱） |
| **Region** | `Singapore` 或 `Oregon`（選最近嘅） |
| **Branch** | `main`（如果用 Git） |
| **Root Directory** | 留空 |
| **Environment** | `Node` |
| **Build Command** | `npm install` |
| **Start Command** | `node server.js` |
| **Plan** | **Free**（免費） |

---

### 步驟 4：部署

1. 點擊 **「Create Web Service」**
2. Render 會自動開始部署（約 2-3 分鐘）
3. 等待部署完成，你會見到 **「Live」** 狀態

---

### 步驟 5：取得網址

部署完成後，你會得到一個永久網址，例如：

```
https://lazarus-master.onrender.com
```

複製呢個網址，就可以永久使用！

---

## ✅ 完成！

現在你可以：

1. **打開網址**
2. **去「設定與 API」頁面**
3. **輸入你的 Manus API Key**
4. **開始使用**

---

## 🔧 常見問題

### Q1：部署失敗點算？

**檢查以下設定：**
- Build Command 係咪 `npm install`
- Start Command 係咪 `node server.js`
- Environment 係咪選咗 `Node`

### Q2：網站打唔開？

**等多 1-2 分鐘**，Render 第一次啟動需要時間。

### Q3：免費版有咩限制？

- **每月 750 小時免費運行時間**（足夠 24/7 運行）
- **15 分鐘無活動會自動休眠**（第一次訪問會慢少少）
- **自動 HTTPS**
- **自動重啟**

### Q4：點樣升級到付費版？

去 Render Dashboard → Settings → Plan，選擇 **Starter**（每月 $7 USD）。

---

## 📦 檔案結構

```
lazarus-deploy/
├── index.html          # 主程式
├── server.js           # Node.js 伺服器
├── package.json        # 依賴配置
├── render.yaml         # Render 配置
├── README.md           # 專案說明
├── DEPLOY_GUIDE.md     # 部署指南（本檔案）
└── .gitignore          # Git 忽略檔案
```

---

## 🎯 下一步

- **自訂域名**：去 Render Dashboard → Settings → Custom Domain
- **環境變數**：去 Render Dashboard → Environment
- **查看日誌**：去 Render Dashboard → Logs

---

## 💬 需要幫助？

如果有任何問題，可以：
- 查看 Render 官方文件：https://render.com/docs
- 聯絡 Render 支援：https://render.com/support

---

**祝你使用愉快！🎉**
