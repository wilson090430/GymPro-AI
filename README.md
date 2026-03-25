# GymPro-AI

🏋️‍♂️ GymPro-AI 智慧健身守護者 (Smart Fitness Guardian)

📖 專案簡介 (Project Overview)

GymPro-AI 是一個結合「電腦視覺 (Computer Vision)」與「生成式 AI (Generative AI)」的智慧健身網頁應用程式。
本專題旨在解決健身新手因「姿勢不當」導致的運動傷害風險，以及私人教練費用高昂的問題。透過 24 小時在線的 AI 虛擬教練，提供即時的動作糾錯與客製化訓練建議。

✨ 核心功能 (Core Features)

1. 👁️ 實時動作視覺矯正 (Real-time Pose Correction)

導入 Google MediaPipe 進行全身 33 個骨架點位的 3D/2D 即時追蹤。

專項行程校驗：例如「手臂彎舉」設定 50° 深度收縮門檻，若偵測到反彈或未達標，系統將即時發出語音警示（「要彎舉完全！」）。

2. 💬 真實 AI 互動顧問 (Live AI Coach)

透過 API 串接 Google Gemini 1.5 Flash 大型語言模型。

具備「階段式引導」能力，主動詢問使用者的健身目標與身體狀況，並提供專業且安全的訓練課表與建議。

3. 📊 智慧場館與 IoT 預約系統 (Smart Gym IoT Management)

模擬 16 項健身房器材的物聯網 (IoT) 即時狀態（使用中 / 閒置 / 擁擠）。

結合前端預約表單，使用者可查看即時狀態並預約 07:00-24:00 的時段，資料將即時同步至場館儀表板。

🛠️ 技術堆疊 (Tech Stack)

前端介面: HTML5, Vanilla JavaScript, Tailwind CSS

視覺辨識: MediaPipe Pose Tracker

AI 語言模型: Google Gemini API (gemini-1.5-flash)

UI/UX 套件: Lucide Icons, Flatpickr (日期選擇器)

🚀 如何在本地端執行 (How to Run Locally)

確保您的電腦已安裝 Visual Studio Code。

在 VS Code 的擴充功能商店中安裝 Live Server。

下載或 Clone 本專案。

使用 VS Code 開啟 index.html，點擊右鍵選擇 "Open with Live Server"。

瀏覽器開啟後，請允許「相機權限」以啟動視覺矯正功能。

⚠️ 注意事項: 本專案使用瀏覽器端的相機存取，必須透過 http://127.0.0.1 (Live Server) 或 https:// 環境執行，直接雙擊 HTML 檔案 (file:///) 將無法啟動相機權限。

此專案為 2026 年學術專題研究成果。
