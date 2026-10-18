# 聯絡時差評估卡 (Timezone Contact Card)

## 關於本專案 / About
> 一個極簡、離線可用的跨時區聯絡評估工具。專為出國旅行與海外生活打造，幫你快速判斷對方是否有空，在最合適的時間聯繫，貼心避開客戶、家人與朋友的睡眠與休息時間。
> 
> A minimalist, offline timezone tool for international travelers and expats to check contact availability and avoid disturbing clients, family, and friends during rest hours.

### 為什麼需要這個工具？ / Why This Tool?

跨時區旅行或出差時，想跟台灣的家人、朋友或客戶聯絡，每次都要心算時差：「現在台灣到底是幾點？對方方便說話嗎？這時間傳訊息會不會打擾到別人休息？」。

When traveling or working abroad, figuring out when to contact people back in Taiwan always involves mental math: "What time is it there? Is it convenient for them? Am I waking them up?"

「聯絡時差評估卡」用最直覺的多色燈號，自動評估對方是否有空，讓你在打開網頁的瞬間就能確認對方當前的作息狀態，主動避開睡眠與休息時段。

The Time Zone Feasibility Card provides an intuitive multi-color status light that automatically evaluates availability upon loading. It enables users to instantly verify the other party's current routine and avoid reaching out during rest or sleeping hours.

### 核心功能 / Core Features

* **直覺多色狀態燈**：根據你的時間自動評估對方是否有空
* **兩地時差總覽**：選出發地與目的地，立刻看到快慢幾小時，並依所選日期計入夏令時間。
* **聯絡可行性判定**：挑一個時間，判斷現在適不適合聯絡（合適／可以但要留意／不建議），並說明原因。
* **可搜尋的城市庫**：90個城市，可用中文（繁／簡）、英文、日文城市名、國家名、機場代碼（如TPE、LAX）搜尋；找不到時可直接輸入IANA時區名稱（如 Asia/Taipei）。
* **零依賴與離線可用**：單一HTML檔案，無需安裝套件，無網路環境也能隨開隨用。
* **三語介面**：中文／English／日本語，依瀏覽器語言自動選擇。


* **Intuitive Multi-Color Status Light**: Automatically assesses whether the other person is available based on your local time.
* **Dual Time Zone Overview**: Select your origin and destination to immediately see the time difference, automatically accounting for Daylight Saving Time (DST) based on the chosen date.
* **Contact Feasibility Assessment**: Pick a time to evaluate whether it is suitable to initiate contact (Suitable / Acceptable with Caution / Not Recommended), complete with detailed explanations.
* **Searchable City Database**: Features 90 cities searchable in Traditional/Simplified Chinese, English, Japanese, country names, or airport codes (e.g., TPE, LAX). If a city isn't found, direct input of IANA time zone names (e.g., Asia/Taipei) is supported.
* **Zero Dependencies & Offline Support**: Single HTML file with no package installations required—fully functional offline and ready to use anytime.
* **Trilingual Interface**: Supports Traditional Chinese, English, and Japanese, automatically matching your browser's language setting.

### 如何使用？ / How to Use?

#### 方式 1：直接透過 GitHub Pages 線上使用 / Access directly online via GitHub Pages

點擊造訪 Click to Visit：https://ethanhlab.github.io/timezone-contact-card/

#### 方式 2：下載至本機使用 / Download for Local Use

1. 下載本專案中的 `index.html` 檔案。
2. 直接用手機或電腦瀏覽器打開 `index.html` 即可運行。
3. （推薦）在手機瀏覽器中選擇「新增至主畫面」，即可當作原生App隨手點開。

1. Download the `index.html` file from this repository.
2. Open `index.html` directly in your mobile or desktop browser to run it.
3. (Recommended) Select "Add to Home Screen" in your mobile browser to launch it like a native app.

### 技術架構

* **HTML5 / CSS3 / JavaScript (Vanilla JS)**：單一HTML檔，無框架、無第三方函式庫、無建置步驟
* **原生 CSS**：以CSS變數、Grid 與Flexbox排版，自動跟隨裝置的淺色／深色模式
* **Intl API**：時區轉換與夏令時間皆使用瀏覽器內建的 `Intl.DateTimeFormat`（IANA 時區資料庫）
* **Zero-backend**：所有運算與判斷都在瀏覽器本機執行，不會上傳任何資料
* **localStorage**：僅在本機儲存語言、配色與作息偏好
* **Google Fonts**：唯一的外部請求（Noto Sans TC），載入失敗時退回系統字型
