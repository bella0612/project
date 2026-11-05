🎬 臺中第二市場專題影展與空間聲影誌

大二影展專題製作成果發表

主題：以「六角時光與常民聲息」重新解構臺中第二市場的空間建築與生活脈動。

📌 成果交付連結 (Submission Links)

請依作業規範繳交以下三個連結：

GitHub Prompt 說明文件（本檔案連結）：

https://github.com/[你的GitHub帳號]/taichung-second-market-filmfest/blob/main/README.md

InfinityFree 首頁網址（Landing Page 畫面）：

http://[你的InfinityFree子網域].infinityfreeapp.com

Vercel 線上部署預覽網址：

https://taichung-second-market-filmfest.vercel.app

💡 Vibe Coding 提示詞（Prompt）工程全紀錄

本專案採用 Vibe Coding（人機協作自然語言導向開發）模式，以清晰的角色定義、階層化的限制條件（大地色系、非對稱排版、檔案分離架構），引導 AI 生成高完成度且具備人文質感的影展官方網站。

以下為本專案生成時所使用的關鍵 Prompt 序列：

階段一：專案立體化與非對稱視覺規劃

使用者情境：跳脫常見的制式置中橫幅或單純列表模板。

Prompt 指令：

你是一位資深前端架構師與影展視覺總監。
我正在製作大二專題：「臺中第二市場專題影展」。
我的專題內容排版不要跟傳統範本一樣，請幫我設計一個跳脫常規模板的架構：
1. 採用「非對稱雙欄雜誌風（Asymmetric Grid Layout）」與「左側固定式空間導覽（Sticky Sidebar）」。
2. 具備多子頁切換功能：首頁策展論述、六角樓建築空間考、清晨到正午的旬味時間軸、參展紀錄片單。
3. 色彩全站採用沉穩典雅的「大地色系（Earth Tone）」：以老市場的赤陶磚紅（#9E4738）為主強調色，搭配暖亞麻紙色底（#F7F5F0）、熟成芥末黃（#C08A3E）與深炭褐文字（#2A2624），營造歲月人文厚度。


階段二：模組化樣式切割與 CSS 架構規範

使用者情境：落實前端專案結構化標準，將樣式解構至專用資料夾。

Prompt 指令：

請嚴格按照以下規範處理前端檔案架構：
1. 將 CSS 樣式徹底模組化切割成三個獨立檔案並放入 `css/` 資料夾：
   - `css/base.css`：定義色彩變數（CSS Variables）、全域 Reset、字體規範。
   - `css/layout.css`：定義頂部 Sticky 導覽列、側邊欄、CSS Grid 系統與 RWD 斷點。
   - `css/components.css`：定義影片卡片、章節標籤、時間軸軌道、引言條與彈窗（Modal）。
2. 圖片檔案獨立放於 `images/` 資料夾。


階段三：語意化 SEO 與行動端 RWD 深度優化

使用者情境：確保手持裝置完整檢視，並提升搜尋引擎最佳化成效。

Prompt 指令：

請為網站注入完整的繁體中文 SEO 元件：
1. 包含 Page Title、Meta Description、Meta Keywords、Open Graph 社群分享標籤。
2. 在 `css/layout.css` 撰寫專屬媒體查詢（Media Queries @media max-width: 960px）：
   - 行動裝置自動將雙欄非對稱佈局轉為直向單欄滿版。
   - 頂部導覽列收合為漢堡選單，點選平滑展開。
   - 確保在手機手持裝置觀看時，所有資訊、卡片及字型層次均能完整顯示且不破版。


階段四：歷史人文與在地田調文本生成

使用者情境：注入第二市場的真實文史肌理（日治新富町、六角樓建築人類學、在地常民名店）。

Prompt 指令：

請以臺中第二市場的歷史脈絡為核心，為各單元產出專業策展文案：
1. 歷史考證：梳理大正六年（1917年）新富町「貴婦市場」與中央木造六角樓作為消防警示中樞的空間功能。
2. 晨昏作息：撰寫「旬味時間軸」，從清晨 04:30 暗夜進料、07:00 王家菜頭粿開爐、11:30 福州意麵與老賴紅茶的蒸氣鼎沸，記錄市場的廿四小時生活聲景。
3. 影展片單：規劃四部具備不同視角（歷史長片、手藝紀錄、純聲音採集、散文詩短片）的虛擬參展片單。


📂 專案檔案結構 (Project Structure)

market-filmfest/
├── index.html              # 影展主頁（含策展總論、六角樓考、時間軸、片單、彈窗互動）
├── css/
│   ├── base.css            # 大地色彩變數、全域 Reset、排版基底
│   ├── layout.css          # 非對稱 CSS Grid、Sticky 側欄、RWD 響應斷點
│   └── components.css      # 卡片模組、時間軸軌道、按鈕、Prompt 彈窗
├── images/
│   ├── hero-bg.jpg         # 影展主視覺背景圖
│   └── ...                 # 各展映劇照與建築歷史影像
└── README.md               # 本說明文件 (Vibe Coding 指令紀錄與連結)


🛠️ 技術亮點與規格檢核

色彩調性：以大地色調體系（Earth Tone Tokens）打造，屏除預設純黑純白，呈現如老膠卷與陶磚的紙感氛圍。

排版技術：採用現代 CSS Grid 與 Flexbox 混合編排，電腦端為左側 310px 空間座標導覽，右側為動態展開的內容展台。

響應式支援 (RWD)：支援桌面寬螢幕、平板與智慧型手機，手機端選單具備平滑摺疊抽屜效果。

模組化分工：樣式表切分清楚，圖片資源獨立存放，符合業界標準規範。

🚀 部署上線指引

1. 替代 InfinityFree 首頁

登入 InfinityFree Control Panel，點選進入帳號之 Online File Manager。

進入 /htdocs/ 資料夾，刪除既有的 index.html 或預設首頁檔案。

建立 css 與 images 資料夾，將本專案的 index.html 上傳至 /htdocs/，CSS 檔案上傳至 /htdocs/css/。

訪問你的 InfinityFree 專屬網址確認首頁已成功更新。

2. 部署至 Vercel

將本專案（包含 index.html、css/、images/、README.md）提交（Push）至個人 GitHub 儲存庫。

登入 Vercel，點擊 "Add New Project" 並授權連接 GitHub 儲存庫。

專案設定保持預設，直接點擊 "Deploy"，約 30 秒即可獲得一組公開的 *.vercel.app 網址。