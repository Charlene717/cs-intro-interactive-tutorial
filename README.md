# 計算機概論 互動式教程 · Introduction to Computer Science

**🌐 Live demo / 線上瀏覽**: <https://charlene717.github.io/cs-intro-interactive-tutorial/>


完整 16 章雙語 (中文 / English) 互動式計算機概論教程，以靜態 HTML/CSS/JS 建構，無需後端伺服器即可瀏覽。涵蓋從計算機發展簡史到 2026 年人工智慧、量子運算與資訊倫理的完整知識體系。

## 課程架構 · Curriculum

四大區塊 (Blocks)，每區塊 4 章：

| Block | Chapters |
|-------|----------|
| **A · 基礎與硬體** | Ch 1 計算機發展簡史 · Ch 2 資料表示法 · Ch 3 數位邏輯與布林代數 · Ch 4 CPU 與計算機組織 |
| **B · 系統與通訊** | Ch 5 記憶體階層與儲存 · Ch 6 作業系統 · Ch 7 電腦網路 · Ch 8 資料庫 |
| **C · 程式與演算法** | Ch 9 程式設計入門 · Ch 10 演算法與複雜度 · Ch 11 資料結構 · Ch 12 軟體工程 |
| **D · 應用與未來** | Ch 13 資訊安全與密碼學 · Ch 14 人工智慧與機器學習 · Ch 15 雲端、邊緣與 IoT · Ch 16 資訊倫理與新興科技 |

加上 **References 參考資料** 與 **Quiz 互動考題（160 題）** 兩個延伸模組。

## 資料夾結構 · Folder Structure

```
Computer_Science/
├── cs-intro-interactive-tutorial-main/    # 主教程：16 章 + hub
│   ├── index.html                          # Hub 首頁
│   ├── styles.css                          # 共用樣式 (royal blue + amber 配色)
│   ├── i18n.js                             # 語言切換 (localStorage: csintro_lang)
│   ├── README.md                           # 本說明
│   ├── history.html ... ethics-future.html # 16 個章節
├── references/
│   └── index.html                          # 16 章節權威來源 (含 DOI/URL)
└── cs-intro-quiz/
    ├── index.html                          # Quiz SPA (Practice / Exam / 錯題複習)
    ├── i18n.js                             # 共享 csintro_lang
    └── data.js                             # 160 題雙語題庫 (16 章 × 10 題)
```

## 互動元件 · Interactive Components

每個章節都包含：

- **Page-Hero with Step Badge** — 標明 `CHAPTER X / 16`
- **多個概念區段** — 雙語對照（`data-zh` / `data-en` 行內切換；`data-lang="zh"/"en"` 段落切換）
- **互動模擬** — Chart.js 圖表 / 純 JS 動畫 (如 Moore's Law 對數圖、二進位/十六進位轉換器、邏輯閘真值表、Stack/Queue 動畫等)
- **決策樹 (Decision Tree)** — `🌳` 標記，提供實務情境判讀
- **Callout** — `tip` (核心觀念) / `warn` (注意事項) / `danger` (常見陷阱)
- **Code-Tabs** — Python + Pseudocode 雙軌示範
- **Quiz** — 每章 3 題雙語自測，含解答與解釋
- **Page-Nav** — Prev / Next 章節導覽

## 技術棧 · Tech Stack

- **Front-end only** — 全靜態 HTML/CSS/JS，雙擊 `index.html` 即可在任何現代瀏覽器執行
- **No build step** — 不需 npm、webpack、編譯
- **Chart.js 4** — CDN 載入用於互動圖表
- **CSS Custom Properties** — `--c-accent` `#1d4ed8` (royal blue), `--c-highlight` `#f59e0b` (amber)
- **i18n** — localStorage key `csintro_lang` (與 quiz 共用，跨頁同步)

## 字型與配色 · Typography & Palette

- **Display:** Crimson Pro (serif) — 標題、強調
- **Body:** DM Sans — 內文
- **Mono:** JetBrains Mono — 程式碼
- **Primary:** #1d4ed8 (royal blue, Tailwind blue-700)
- **Dark accent:** #1e3a8a (blue-900)
- **Highlight:** #f59e0b (amber-500) — 決策樹、強調標題
- **Hero gradient:** midnight (#0f172a) → blue-900 → blue-700 → blue-600

## 如何使用 · Getting Started

1. 直接打開 `cs-intro-interactive-tutorial-main/index.html`（雙擊或拖入瀏覽器）
2. 在右上角點 **EN / 中文** 切換語言（會記住在 localStorage）
3. 從 Hub 點選任意章節進入；底部有「Next →」連續閱讀
4. 完成章節後可至 **Quiz** 做自我測試（支援 Practice / Exam 兩種模式、錯題複習、隨機練習）
5. 學術出處可於 **References** 查閱（含 DOI / URL）

## 內容更新時間 · Last Updated

- **Built:** 2026-05-16
- **Curriculum aligned to:** ACM/IEEE-CS/AAAI CS2023
- **2026 觀察包含：** OWASP Top 10 (2025)、NIST FIPS 203/204/205 (PQC)、HTTP/3 + QUIC (RFC 9114)、GPT-5/Claude 4.6/Gemini 3 LLM 比較、IBM Nighthawk 120-qubit、Google Willow 「below threshold」error correction、EU AI Act 全面執行

## 授權 · License

教學內容僅供學習用途；引用文獻請參照 `references/index.html` 標註的原始 DOI/URL，遵守該文獻的授權條款。本網站介面樣式與互動程式碼可在標註出處的前提下自由再利用。

© Charlene — Introduction to Computer Science · Interactive Tutorial
