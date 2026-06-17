# 港語傳承中心 · Landing Page
**Cantonese Heritage Learning Centre — 2026–2027 Enrolment Landing Page**

> Registered Charity No. 1215373 · Southampton, UK

---

## Table of Contents · 目錄

1. [Project Overview · 項目簡介](#project-overview)
2. [Features · 功能特色](#features)
3. [File Structure · 文件結構](#file-structure)
4. [Preview Locally · 本地預覽](#preview-locally)
5. [Deploy · 部署方法](#deploy)
6. [Customise · 如何自訂](#customise)
7. [Credits · 鳴謝](#credits)

---

## Project Overview

A **single-file, self-contained HTML landing page** built for the 港語傳承中心 2026–2027 enrolment campaign. Designed to convert BNO Hong Kong immigrant parents in Southampton into enrolments or referrals, using Alex Hormozi's **$100M Offers** framework.

### 項目簡介

這是一個**單一 HTML 文件、完全自足**的招生 Landing Page，專為港語傳承中心 2026–2027 年度招生而建。目標受眾為英國南安普頓的 BNO 港人家長，運用 Alex Hormozi **$100M Offers** 框架設計，目的是將訪客轉化為報名學員或口碑推薦。

---

## Features

| Feature | Detail |
|---|---|
| 📱 **Mobile-first** | CSS built smallest-screen-first; breakpoints at 640px and 1024px |
| 🖼️ **Base64 hero image** | Illustration embedded — no external image files needed |
| ⏱️ **Live countdown** | JavaScript timer counting down to Sept 12, 2026 first class |
| 🪑 **Seats visualiser** | 20-seat grid showing filled vs available spots |
| 📌 **Sticky CTA bar** | Appears on scroll (mobile); hidden on desktop where CTAs are visible |
| 🎯 **Hormozi value stack** | Card list on mobile; full table on desktop (1024px+) |
| ❓ **Accordion FAQ** | Touch-friendly expand/collapse, one open at a time |
| 🔴 **Ticker banner** | Sticky top marquee with urgency messages |
| 🌐 **Zero dependencies** | No frameworks, no CDN JS, no build step — open and it works |
| ♿ **Accessible** | Semantic HTML, `aria-hidden` on decorative elements, keyboard-navigable FAQ |

### 功能特色

| 功能 | 說明 |
|---|---|
| 📱 **手機優先** | CSS 從最小屏幕開始設計，640px 和 1024px 為 Breakpoint |
| 🖼️ **Base64 背景圖** | 插圖直接嵌入，無需外部圖片文件 |
| ⏱️ **即時倒數計時** | JavaScript 倒數至 2026年9月12日正式上課 |
| 🪑 **名額視覺化** | 20格名額顯示已佔用與可報名位置 |
| 📌 **Sticky 報名欄** | 手機滾動後顯示；桌面隱藏（CTA 按鈕已可見） |
| 🎯 **Hormozi 價值堆疊** | 手機顯示卡片列表；桌面（1024px+）顯示完整表格 |
| ❓ **手風琴 FAQ** | 觸控友好展開／摺疊，每次只開一項 |
| 🔴 **跑馬燈橫幅** | 置頂固定緊迫感訊息 |
| 🌐 **零依賴** | 無框架、無 CDN JS、無需 Build — 直接開啟即用 |
| ♿ **無障礙** | 語義化 HTML，裝飾元素加 `aria-hidden`，FAQ 支援鍵盤操作 |

---

## File Structure

```
project/
│
├── chlcentre-landing.html   ← The entire site (HTML + CSS + JS + image, all in one)
└── README.md                ← This file
```

> **Note:** The hero illustration is base64-encoded directly inside the HTML file. No `/images/` folder is needed.

### 文件結構

```
project/
│
├── chlcentre-landing.html   ← 整個網站（HTML + CSS + JS + 圖片，全部合一）
└── README.md                ← 本文件
```

> **注意：** Hero 插圖已 Base64 編碼直接嵌入 HTML，無需 `/images/` 資料夾。

---

## Preview Locally

**Option 1 — Just open it (simplest):**
```bash
# macOS / Windows / Linux
# Double-click chlcentre-landing.html in Finder / Explorer
# OR drag the file into any browser window
```

**Option 2 — Live server (recommended for editing):**
```bash
# If you have Node.js installed:
npx serve .

# If you have Python installed:
python3 -m http.server 8080
# Then open: http://localhost:8080/chlcentre-landing.html
```

**Option 3 — VS Code:**
Install the **Live Server** extension, right-click the file → *Open with Live Server*.

### 本地預覽

**方法一 — 直接開啟（最簡單）：**
```bash
# 在 Finder / 檔案總管中雙擊 chlcentre-landing.html
# 或將文件拖入任何瀏覽器視窗
```

**方法二 — Live Server（建議用於編輯）：**
```bash
# 已安裝 Node.js：
npx serve .

# 已安裝 Python：
python3 -m http.server 8080
# 然後開啟：http://localhost:8080/chlcentre-landing.html
```

**方法三 — VS Code：**
安裝 **Live Server** 擴充套件，右鍵點擊文件 → *Open with Live Server*。

---

## Deploy

Because the page is a single self-contained file, it deploys to **any static host in under 2 minutes.**

### Cloudflare Pages (Recommended · 推薦)
```bash
# 1. Push the file to a GitHub repository
git init
git add chlcentre-landing.html
git commit -m "Initial landing page"
git push origin main

# 2. In Cloudflare Dashboard:
#    Pages → Create Project → Connect GitHub repo
#    Build command: (leave blank)
#    Output directory: /  (or leave blank)
#    → Save and Deploy
```

### GitHub Pages
```bash
# In your GitHub repo:
# Settings → Pages → Source: Deploy from branch → main → / (root)
# Your page will be live at: https://yourusername.github.io/repo-name/chlcentre-landing.html
```

### Netlify
```bash
# Drag-and-drop deploy (no account setup needed):
# 1. Go to https://app.netlify.com/drop
# 2. Drag the chlcentre-landing.html file onto the page
# 3. Done — you get a live URL instantly
```

### 部署方法

由於整個網站是單一文件，可在 **2分鐘內部署到任何靜態主機**。

| 平台 | 難度 | 說明 |
|---|---|---|
| **Cloudflare Pages** | ⭐ 推薦 | 免費、全球 CDN、自訂域名 |
| **GitHub Pages** | ⭐⭐ | 免費，需 GitHub 帳戶 |
| **Netlify Drop** | ⭐ 最快 | 拖放即部署，無需帳戶 |

---

## Customise

### 1. Contact Details · 聯絡資料

Search and replace the following in `chlcentre-landing.html`:

| Placeholder | Your value | Location |
|---|---|---|
| `07704 592 524` | Your WhatsApp number | Hero, Sticky bar, Final CTA, FAQ |
| `info@chlcentre.org.uk` | Your email | Final CTA, Footer |
| `SO16 3GJ` | Your postcode | Timeline, Final CTA, Footer |
| `Cantell School` | Your venue | Timeline, Final CTA, Footer |
| `447704592524` | WhatsApp link number (no spaces) | All `wa.me` links |

### 2. Key Dates · 重要日期

Find and update these strings:

```
9月5日   → Your registration day
9月12日  → Your first class date
2026-09-12T10:00:00+01:00  → ISO date for the countdown timer (line ~530 in the JS)
```

### 3. Seats Available · 可用名額

In the JavaScript section (search for `// ── SEATS VISUAL ──`):

```javascript
// Change 13 to however many seats are already enquired
for (let i = 0; i < 20; i++) {
  s.className = 'seat ' + (i < 13 ? 'taken' : 'open');  // ← change 13
```

### 4. Colours · 顏色

All colours are CSS custom properties at the top of the `<style>` block:

```css
:root {
  --red:    #D72638;   /* Primary CTA colour */
  --gold:   #F4A800;   /* Accent / highlight */
  --navy:   #0D1B3E;   /* Primary dark colour */
  --cream:  #FFF9F0;   /* Page background */
  --green:  #1DB954;   /* Live dot / positive */
}
```

### 5. Hero Image · Hero 背景圖

To swap the hero illustration:

```bash
# Step 1: Convert your new image to base64
base64 -w 0 your-new-image.jpg > new_image_b64.txt

# Step 2: In chlcentre-landing.html, find:
#   background: url("data:image/jpeg;base64,/9j/4AAQ...
# and replace everything between the quotes with:
#   data:image/jpeg;base64,[paste your new base64 here]
```

> **Tip:** Use a Python script for large replacements to avoid editor crashes:
> ```python
> content = open('chlcentre-landing.html').read()
> b64 = open('new_image_b64.txt').read().strip()
> # Find and replace between the url(" and ") center
> ```

### 6. Google Analytics · 數據追蹤

Add before `</head>`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### 7. WhatsApp CTA Tracking · WhatsApp 點擊追蹤

Replace all `href="https://wa.me/447704592524"` with:
```html
href="https://wa.me/447704592524?text=你好，我想查詢2026-2027年度招生詳情"
```
This pre-fills the WhatsApp message, reducing friction for parents.

---

## Hormozi Framework Applied · Hormozi 框架應用

| $100M Offers Element | Implementation |
|---|---|
| **Dream Outcome** | Hero headline — "你的孩子還記得廣東話嗎？" |
| **Problem Agitation** | 4-card problem section targeting BNO parent fears |
| **Value Stack** | 9-item stack with market price estimates totalling £3,000+/yr |
| **Scarcity** | 20-seat visual + countdown timer + ticker |
| **Social Proof** | 3 parent testimonials with star ratings |
| **Risk Reversal** | "試上承諾" — first class satisfaction guarantee |
| **Irresistible CTA** | WhatsApp direct link × 5 touchpoints + sticky bar |
| **Urgency** | Live countdown + "去年全部額滿" reminder |

---

## Credits

- **Design & Development:** Built with [Claude.ai](https://claude.ai) (Anthropic)
- **Copywriting Framework:** Alex Hormozi — *$100M Offers*
- **Hero Illustration:** 港語傳承中心 (provided by client)
- **Fonts:** [Noto Sans TC](https://fonts.google.com/noto/specimen/Noto+Sans+TC) + [Bebas Neue](https://fonts.google.com/specimen/Bebas+Neue) via Google Fonts
- **Hosting Suggestions:** Cloudflare Pages · GitHub Pages · Netlify

### 鳴謝

- **設計及開發：** 使用 [Claude.ai](https://claude.ai)（Anthropic）建構
- **文案框架：** Alex Hormozi — *$100M Offers*
- **Hero 插圖：** 港語傳承中心提供
- **字體：** Google Fonts（Noto Sans TC + Bebas Neue）
- **建議部署平台：** Cloudflare Pages · GitHub Pages · Netlify

---

## Licence · 授權

This page was created specifically for **港語傳承中心 (Cantonese Heritage Learning Centre)**, Registered Charity No. 1215373. All content, copy, and branding belong to the charity. The code structure may be reused for other non-profit education projects with attribution.

本頁面專為**港語傳承中心**（英國慈善機構編號 1215373）製作。所有內容、文案及品牌均屬該慈善機構所有。代碼結構可在註明出處的情況下用於其他非牟利教育項目。

---

*Built with ❤️ for the Hong Kong community in Southampton · 為南安普頓港人社群用心製作*
