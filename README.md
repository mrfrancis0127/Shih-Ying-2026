# 張仕穎 競選網站

> **2026 年員林市西區（第四選區）市民代表參選人 ・ 台灣民眾黨提名**
>
> 「穎在您心，幸福起航。改變，從我們的選票開始。」

---

## 候選人資訊

| 項目 | 內容 |
| --- | --- |
| 候選人 | 張仕穎（Chang Shih-Ying） |
| 政黨 | 台灣民眾黨 |
| 參選職位 | 員林市市民代表 |
| 選區 | 員林市西區 ・ 第四選區 |
| 候選號次 | 04 |
| 現職 | 員林市三義里里長（112.12.25 至今） |
| 學歷 | 國立台灣體育運動大學 體育學系 |
| 核心理念 | 幸福家園，專業監督 |
| 競選口號 | 穎在您心，幸福起航。改變，從我們的選票開始。 |

---

## 檔案結構

```
zhangshiying_site/
├── index.html         主網頁（單頁式設計，所有 CSS/JS 內嵌）
├── README.md          本說明文件
└── image/             圖片資料夾
    ├── hero.jpg       候選人形象照（首頁主視覺）
    ├── basketball.jpg 自費更換籃網（服務實績）
    ├── cleanup.jpg    社區環境整理（服務實績）
    ├── community.jpg  里鄰長文康活動（服務實績）
    └── mothersday.jpg 母親節傳統美食體驗（服務實績）
```

---

## 使用方式

### 在電腦本機預覽

直接用瀏覽器（Chrome、Edge、Safari 等）打開 `index.html` 即可瀏覽，不需要任何伺服器或網路連線。

### 上架到網路

可選擇以下任一免費或低成本的方案：

1. **GitHub Pages**（免費）：把整個資料夾推上 GitHub repo，到 Settings → Pages 啟用即可。
2. **Netlify Drop**（免費）：到 [app.netlify.com/drop](https://app.netlify.com/drop) 把整個資料夾拖進去，立刻有公開網址。
3. **Cloudflare Pages**（免費）：類似 Netlify，速度更快、台灣用戶體驗較佳。
4. **虛擬主機 / 自架網域**：把整個資料夾透過 FTP 上傳到主機根目錄。

> 強烈建議申請一個自有網域（例如 `chang-shihying.tw`），會比子網域更專業、更有可信度。

---

## 網站結構

| 區段 | 錨點 | 內容 |
| --- | --- | --- |
| 主視覺 | `#top` | 形象照、口號、選區編號 04 |
| 認識仕穎 | `#about` | 個人背景、學經歷、社團經驗、家庭 |
| 核心理念 | `#vision` | 民生優先、新政實踐、世代橋樑 |
| 服務實績 | `#service` | 四張服務照片與說明 |
| 政見規劃 | `#policy` | 五項具體政策承諾 |
| 行動呼籲 | `#cta` | 投票引導與選票視覺 |

---

## 修改指南

### 替換圖片

把新圖放進 `image/` 資料夾，**檔名保持一致**即可（例如新形象照覆蓋 `hero.jpg`）。如果要新增照片，記得在 HTML 裡同步加入 `<img src="image/新檔名.jpg">`。

> 建議圖片寬度不超過 1600px、單檔大小控制在 500KB 以內，避免網頁載入太慢。

### 修改文字內容

打開 `index.html`，使用任何文字編輯器（推薦 [VS Code](https://code.visualstudio.com/)）搜尋要修改的句子直接編輯。重點區塊位置：

- **競選口號**：搜尋「穎在您心」
- **政見規劃**：搜尋「五項承諾」
- **聯絡資訊**：搜尋「FOOTER」區塊

### 修改主色調

在 HTML 開頭的 `<style>` 區塊有一段 `:root` 變數定義，可直接調整：

```css
:root{
  --teal:#0d4a4f;        /* 主色：深湖綠 */
  --teal-deep:#08363a;   /* 主色加深 */
  --mint:#a8d5b8;        /* 民眾黨薄荷綠 */
  --accent:#d97645;      /* 強調色：橘紅 */
  --paper:#f6f1e6;       /* 米白底色 */
}
```

---

## 待補資訊

以下欄位目前留白或為占位內容，請盡快更新：

- [ ] **競選總部地址**（footer）
- [ ] **服務專線電話**（footer，建議使用辦公室電話而非個人手機）
- [ ] **Facebook 粉絲專頁連結**（footer）
- [ ] **Instagram / LINE 官方帳號**（如有）
- [ ] **政見子頁面或 PDF 政策白皮書**（如要更深入的論述）
- [ ] **競選團隊照片**（如要強化「組織戰」印象）
- [ ] **Google Analytics / Meta Pixel 追蹤碼**（如要追蹤流量）

---

## 個資與安全注意事項

- 網站**不包含**身分證字號、戶籍地址、家屬個資、孩子生日等敏感資訊。
- PDF 提名表上的個人手機號碼（0954-010182）**未公開於網站**，建議改用辦公室專線。
- 提名表上的私人 email 已放在 footer，如要保留請評估隱私風險。

---

## 技術規格

- 純 HTML + CSS + JavaScript，**不依賴任何框架**。
- 響應式設計，桌機 / 平板 / 手機皆可正常瀏覽。
- 使用 Google Fonts 提供的 Noto Serif TC、Noto Sans TC、Cormorant Garamond、DM Mono 字體。
- 所有 CSS 與 JS 內嵌於 `index.html`，沒有外部相依檔案（除字體與圖片）。
- 通過 W3C HTML5 規範。

---

## 設計概念

整體走「**現代雜誌 ✕ 在地溫度**」的編輯風格，刻意避開傳統候選人網站的飽和大紅大綠、密集口號排版。主色取自候選人形象照 polo 衫的深湖綠，搭配米白底色與民眾黨識別的薄荷綠，並用橘紅作為強調色製造記憶點。

候選號次「**04**」貫穿全站作為視覺記憶錨——主視覺背景的巨型義大利體數字、形象照旁的裝飾數字、CTA 區的全屏底紋、最後的選票視覺——強化「投 4 號張仕穎」的聯想。

---

## 授權

本網站由候選人張仕穎委託製作，著作權歸屬候選人本人。圖片素材皆為候選人提供之公開照片。

字體授權：
- Noto Sans TC / Noto Serif TC：[SIL Open Font License](https://fonts.google.com/noto/specimen/Noto+Sans+TC/license)
- Cormorant Garamond：[SIL Open Font License](https://fonts.google.com/specimen/Cormorant+Garamond/license)
- DM Mono：[SIL Open Font License](https://fonts.google.com/specimen/DM+Mono/license)

---

**最後更新**：2026 年 5 月

*本網站僅作為候選人個人理念宣傳之用，不接受任何形式的政治獻金或商業合作邀約。如需與候選人聯繫，請透過上述聯絡方式。*
