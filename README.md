# 臺中第二市場專題影展與常民聲影誌 (Taichung Second Market Film Festival)

本專案為大二「影展專題介紹」成果網站，主題聚焦於**臺中第二市場**。全站跳脫傳統樣板，採用大地色系（Earth Tone）視覺、非對稱雙欄雜誌風格（Asymmetric Magazine Layout）、原生 CSS Grid 響應式系統，並透過 AI 輔助開發（Vibe Coding）完成全站架構、SEO 優化與樣式模組化切割。

---

## 專案交付連結 (Project Deliverables)

- **(1) Vibe Coding Prompt 說明檔 (GitHub Markdown)：**  
  `https://github.com/你的GitHub帳號/你的專案名稱/blob/main/README.md`
- **(2) InfinityFree 首頁成果網址：**  
  `http://你的子網域.infinityfreeapp.com/` （或綁定的個人首頁網址）
- **(3) Vercel 部署上線網址：**  
  `https://你的專案名稱.vercel.app/`

---

## 專案結構與模組化規範

依據專案規格，CSS 樣式與圖形資產皆已完成模組化切割：

```text
market-project/
├── index.html              # 影展與空間策展主頁（含 SEO、OG 標籤、Tab 切換機制）
├── css/
│   ├── base.css            # 大地色系變數 (--c-terracotta 等)、Reset、字型
│   ├── layout.css          # CSS Grid 雙欄 (310px 側欄 + 主舞台)、Navbar、RWD 斷點
│   └── components.css      # 影片卡片、時間軸節點 (Timeline)、提示詞彈窗、徽章
├── images/                 # 影展主視覺、六角樓建築圖、常民市場劇照
└── README.md               # 本文件（Vibe Coding 指令說明與部署紀錄）