# 📄 GOLDEN DMS - 發文管理系統 V1.1

> 黑金奢華風格的專業發文字號管理系統

![Version](https://img.shields.io/badge/version-1.1-gold)
![License](https://img.shields.io/badge/license-MIT-blue)
![Status](https://img.shields.io/badge/status-stable-success)

## ✨ 系統特色

### 🎨 視覺設計
- **黑金奢華風格**：深黑色背景搭配金色漸層，展現專業品質
- **玻璃擬態效果**：柔和的霧面質感與動態光暈
- **響應式設計**：完美適配手機、平板、電腦
- **Material Icons**：圓潤現代的圖示系統

### 🚀 核心功能
- ✅ 發文字號自動生成（格式：公司代碼+部門代碼+字+第+日期+流水號+號）
- ✅ 臨時號碼快速產生
- ✅ 自訂發文日期
- ✅ 公司/部門選擇（53家公司、22個部門）
- ✅ 自訂公司代碼
- ✅ 智能流水號防重複
- ✅ 即時搜尋與篩選
- ✅ 編輯與刪除功能
- ✅ 統計資料儀表板
- ✅ CSV 匯出功能
- ✅ 本地儲存（不需伺服器）

## 📦 檔案結構

```
發文管理系統/
├── index.html          # 主程式（單一檔案，開箱即用）
├── README.md           # 使用說明（本檔案）
├── LICENSE             # MIT 授權條款
└── docs/
    ├── 使用手冊.md      # 詳細操作說明
    └── 部署指南.md      # 部署教學
```

## 🚀 快速開始

### 方法一：直接開啟（最簡單）
1. 下載 `index.html`
2. 用瀏覽器開啟檔案
3. 立即開始使用！

### 方法二：本地伺服器
```bash
# 使用 Python 啟動簡易伺服器
python -m http.server 8000

# 或使用 Node.js
npx http-server
```
然後開啟瀏覽器訪問 `http://localhost:8000`

### 方法三：GitHub Pages 部署
1. 上傳到 GitHub 倉庫
2. 進入 Settings > Pages
3. 選擇 main 分支
4. 系統自動部署完成！

## 💡 使用方式

### 新增文號
1. 點擊底部中央的 ➕ **新增** 按鈕
2. 選擇公司與部門
3. 選擇發文日期
4. 填寫主旨與受文者（選填）
5. 點擊「完整建檔」或「臨時號碼」

### 管理文號
- **搜尋**：使用頂部搜尋框
- **篩選**：點擊「全部文件」、「臨時號碼」、「已完成」
- **編輯**：點擊文件卡片中的 ✏️ 按鈕
- **刪除**：點擊文件卡片中的 🗑️ 按鈕
- **完成**：臨時號碼可點擊「完成」按鈕補充資料

### 查看統計
點擊右上角的 📊 統計按鈕，查看：
- 總文號數
- 已完成數量
- 臨時號碼數量
- 今日新增數量

### 匯出資料
1. 點擊底部右側 ⚙️ **設定** 按鈕
2. 點擊「匯出 CSV 檔案」
3. 檔案會自動下載

## 🏢 公司與部門清單

### 支援的公司（53家）
宇軒能源、宇軒綠能、兆明升、兆飛鴻、兆明科技、晁星能源、永煜能源、晁田能源、晶天下、昊陽電業、浩陽精工、浩陽電業、利高光電、雪芙、宸君投資、利晁光電、昊田、介碩、昊天、昊能、永恩電業、昊克、昊鴻、昊恩、昊碩、昊明電業、昊升電業、宇軒電業、昊瑞電業、昊瑞、昊儒、昊煜電業、昊升一號、昊升二號、昊升三號、昊軒一號、昊軒二號、昊軒三號、晁明電業、昊明綠能、晁明一號、晁明二號、晁明三號、昊儒電業、昊星電業、昊升、兆明升電業、兆明升一號、兆明升二號、昊勤能源、昊農、浩陽養殖、嘉義算力

### 支援的部門（22個）
稽核室、總經理室、法務室、財務處、財務部、會計部、總管理處、人資部、管理部、資訊部、品質管理部、採購處、採購部、倉管部、工程管理處、工程部、維運部、設計規劃處、設計規劃部、事業開發暨專案管理處、業務部、新產品事業部

## 📱 系統需求

- **瀏覽器**：Chrome 90+、Firefox 88+、Safari 14+、Edge 90+
- **裝置**：電腦、平板、智慧型手機
- **網路**：首次載入需要網路（載入字體與圖示），之後可離線使用
- **儲存**：使用瀏覽器 localStorage（無需資料庫）

## 🔒 資料安全

- ✅ 所有資料儲存在本地瀏覽器
- ✅ 不會上傳到任何伺服器
- ✅ 資料隨時可匯出備份
- ✅ 使用相同瀏覽器資料會保留
- ⚠️ 清除瀏覽器資料會導致資料遺失（建議定期匯出備份）

## 🎯 文號格式說明

**格式**：`公司代碼` + `部門代碼` + `字` + `第` + `民國年月日` + `流水號` + `號`

**範例**：
- `昊陽財務字第114123001號`
  - 公司：昊陽
  - 部門：財務
  - 日期：114年12月30日
  - 流水號：001

**智能流水號**：
- 系統會自動計算當日同公司同部門的文號數量
- 流水號從 001 開始，自動遞增
- 防止重複編號

## 🛠️ 技術架構

- **前端框架**：純 HTML + JavaScript（無需安裝依賴）
- **CSS 框架**：Tailwind CSS（CDN）
- **字體**：Google Fonts
  - Noto Sans TC（繁體中文）
  - Playfair Display（襯線英文）
  - Cinzel（標題英文）
- **圖示**：Material Icons Round
- **儲存**：localStorage API
- **相容性**：ES6+ JavaScript

## 📝 版本歷史

### V1.1 (2024-12-30) - Golden Edition
- ✨ 全新黑金奢華風格設計
- ✨ 新增發文日期選擇功能
- ✨ 金色發光框文號顯示
- 🎨 優化視覺層次與對比
- 🐛 修復已知問題

### V1.0 (2024-12-29)
- 🎉 首次發布
- ✅ 基礎文號管理功能
- ✅ 公司與部門資料建置
- ✅ 智能流水號系統

## 🤝 貢獻與回饋

如有任何問題或建議，歡迎透過以下方式聯繫：
- 📧 Email：[您的聯絡信箱]
- 💬 Issues：[GitHub Issues 連結]

## 📄 授權條款

本專案採用 MIT License 授權

```
MIT License

Copyright (c) 2024

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 🌟 致謝

感謝所有使用本系統的使用者！

---

**GOLDEN DMS** - 讓文件管理更優雅 ✨
