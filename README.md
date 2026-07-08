# AI 驅動的英語語法修正器

##直接點擊網頁版連結使用：https://dvl-studio.github.io/english-corrector/

## 💡 關於此專案

要寫出自然且母語等級的英文充滿挑戰。傳統的語法檢查工具通常只能抓出基本的拼字錯誤，卻無法理解上下文、語氣，或是混淆同音異義詞。

此專案是一個輕量級、無伺服器（Serverless）的網頁應用程式，借助大型語言模型 (LLMs) 的強大能力來扮演專業英語教師的角色。它不僅能修正語法錯誤，還會解釋修正背後的「原因」。

### ✨ 核心功能
* **具備上下文感知的修正：** 修復語法、標點符號以及情境用詞錯誤（例如混淆 "coal" 與 "cool"）。
* **多國語言解釋：** 提供**英文、繁體中文與越南文**的詳細語法筆記與建議，幫助非母語人士真正理解語意間的細微差別。
* **原生語音朗讀 (TTS)：** 使用 Web Speech API 內建朗讀功能，並支援動態語系切換。
* **隱私優先的 API 設定：** 無需後端伺服器。使用者可以安全地輸入自己的 Google Gemini API 金鑰，該金鑰將安全地儲存於瀏覽器的本地空間 (`localStorage`) 中。
* **彈性的網路錯誤處理：** 實作指數退避 (Exponential Backoff) 機制，確保即使在不穩定的行動網路下也能維持穩定的 API 連線。

### 🛠️ 技術堆疊
* **前端：** HTML5, Vanilla JavaScript (原生 JS)
* **樣式排版：** [Tailwind CSS](https://tailwindcss.com/) (透過 CDN 引入)
* **資安防護：** [DOMPurify](https://github.com/cure53/DOMPurify) (防止 XSS 攻擊)
* **AI 引擎：** Google Gemini API (`gemini-2.5-flash`)

---

## 🚀 快速開始

因為這是一個純前端的應用程式，所以**完全不需要建置步驟、不需要安裝 npm，也無需設定任何伺服器。**

### 事前準備
您將需要一組免費的 Google Gemini API Key。
* 在這裡免費申請：[Google AI Studio](https://aistudio.google.com/app/apikey)

### 安裝與使用方式

**本地端與網頁版使用 (最簡單的方式)**
1. 下載或 Clone 此儲存庫：
   ```bash
   git clone [https://github.com/dvl-studio/english-corrector.git](https://github.com/dvl-studio/english-corrector.git)

# AI-Powered English Grammar Corrector

## 💡 About The Project

Writing natural, native-level English can be challenging. Traditional grammar checkers often catch basic spelling errors but fail to understand context, tone, or homophone mix-ups. 

This project is a lightweight, serverless web application that leverages the power of Large Language Models (LLMs) to act as a professional English teacher. It not only corrects grammatical errors but also explains the *why* behind the corrections.

### ✨ Key Features
* **Context-Aware Corrections:** Fixes grammar, punctuation, and contextual word-choice errors (e.g., "coal" vs. "cool").
* **Multilingual Explanations:** Provides detailed grammar notes and suggestions in **English, Traditional Chinese, and Vietnamese** to help non-native speakers truly understand the nuances.
* **Native Text-to-Speech (TTS):** Built-in read-aloud functionality using the Web Speech API with dynamic language switching.
* **Privacy-First API Config:** No backend required. Users securely input their own Google Gemini API key, which is stored locally in their browser (`localStorage`).
* **Resilient Network Handling:** Implements Exponential Backoff to ensure stable API connections even on spotty mobile networks.

### 🛠️ Built With
* **Frontend:** HTML5, Vanilla JavaScript
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (via CDN)
* **Security:** [DOMPurify](https://github.com/cure53/DOMPurify) (XSS Prevention)
* **AI Engine:** Google Gemini API (`gemini-2.5-flash`)

---

## 🚀 Getting Started

Because this is a purely client-side application, there are **no build steps, no npm installations, and no servers to configure.** 

### Prerequisites
You will need a free Google Gemini API Key. 
* Get one here: [Google AI Studio](https://aistudio.google.com/app/apikey)

### Installation & Usage

**Local Usage (The Easiest Way)**
1. Download or clone this repository:
   ```bash
   git clone [https://github.com/dvl-studio/english-corrector.git](https://github.com/dvl-studio/english-corrector.git)
2. Direct link: https://dvl-studio.github.io/english-corrector/
   
