# [專案名稱 : Syna ]：基於 NLWeb 的智慧化銀行互動式介面

[![Hackathon](https://img.shields.io/badge/Hackathon-2026-blue.svg)](https://github.com/[你的帳號]/[專案名稱])
[![Tech Stack](https://img.shields.io/badge/Tech_Stack-Frontend%20%7C%20NLWeb%20%7C%20Backend-green.svg)](#技術架構)

## 📌 專案願景 (Vision)
隨著銀行業務日益複雜，使用者往往迷失在繁瑣的選單與表單中。本專案旨在透過 **「一個簡單的對話框」**，將複雜的銀行網頁功能轉化為直覺的自然語言操作。透過 Microsoft NLWeb 作為核心橋樑，精準解析使用者意圖並調用後端 API，實現「言即所得」的金融服務體驗。

## 🚀 核心問題 (Problem Statement)
* **介面過於複雜：** 銀行網頁包含轉帳、理財、貸款等多層級選單，導覽成本高。
* **操作門檻：** 特定金融操作（如複雜的理財設定）對一般用戶具備技術門檻。
* **開發維護壓力：** 前端需針對數百個 API 開發專門的 UI，開發週期長。

## 💡 解決方案 (Solution)
* **對話式操作 (Chat-to-Action)：** 使用者只需輸入「幫我把上個月多出的餘額轉入定期定額」，系統自動串接後端 API 完成。
* **NLWeb 意圖編排：** 採用 Microsoft NLWeb 作為中台，動態對齊前端 UI 狀態與後端 API 邏輯。
* **無縫整合：** 在現有的前後端架構中，僅需嵌入 Chat 組件即可操作全站功能。

## 🏗 技術架構 (Architecture)
本專案整合了現有的金融系統基礎設施，並引入智慧化編排層：

1.  **Frontend (現有架構)：** 負責呈現複雜網頁 UI 與 Chat 組件。
2.  **Orchestration Layer (NLWeb)：** 介於前後端之間，負責自然語言解析、API 參數對齊與會話狀態管理。
3.  **Backend (現有架構)：** `提供穩定的金融業務邏輯與 API 接口。

<img width="919" height="1024" alt="image" src="https://github.com/user-attachments/assets/aadd8108-9cd0-4c35-99b8-6b0626d66948" />

> **提示：** 建議在此處附上一張說明 `User -> Chat UI -> NLWeb -> Backend API -> Database` 的系統架構圖，這對評審快速理解系統資料流非常有幫助。

## 🛠 關鍵功能 (Key Features)
* **[功能 1]：** `[請填寫，例如：全站 API 自然語言導航]`
* **[功能 2]：** `[請填寫，例如：複雜表單自動化填充]`
* **[功能 3]：** `[請填寫，例如：多步驟金融流程引導 - 處理缺漏資訊的反問機制]`

## 🔒 安全與合規 (Security & Compliance)
考慮到金融業的特殊性，本專案實施以下機制：
* **意圖二次確認：** 涉及敏感交易（如轉帳）時，系統會調起原有的前端驗證機制。
* **隱私保護：** 對話內容不涉及個人敏感資料 (PII) 的明文存儲。
* **權限管控：** NLWeb 僅能調用當前登入使用者權限內的 API。

## 📈 預期效益 (Expected Impact)
* **提升轉換率：** 簡化操作路徑，預計提升 `[X]%` 的理財申辦率。
* **降低成本：** 減少人工客服導引需求。
* **開發效能：** 透過 NLWeb 減少 `[X]%` 專門 UI 頁面的開發需求。

## 👥 團隊介紹 (Team)
* **[成員姓名]** - `[職位，如：Backend Engineer]`：負責 API 設計與 NLWeb 串接。
* **[成員姓名]** - `[職位，如：Frontend Engineer]`：負責 Chat UI 與網頁架構整合。
* **[成員姓名]** - `[職位]`：`[負責事項]`

## 📝 快速開始 (Getting Started)
### 1. 前置需求
* `[請填寫，例如：Node.js v18+]`
* `[請填寫，例如：Java 17 / Spring Boot]`
* Microsoft NLWeb API Key

### 2. 安裝與啟動
```bash
# 啟動後端
cd backend && ./mvnw spring-boot:run

# 啟動前端
cd frontend && npm install && npm run dev
```
