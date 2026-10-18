# BayStay 灣宿指南

靜態種子站：大灣區＋亞洲熱門度假村／酒店目錄（繁中為主）。

## 用途

- 旅客：按地區、價位、親子、標籤篩選住宿
- 酒店：標準目錄位／Featured 贊助（見 `partner.html`）

## 非博彩硬規則

只推介住宿與度假設施。**不推廣網上博彩、賭場投注或博彩優惠。** 每則 listing 必須 `non_gaming: true`。

## 如何開啟

需用本機靜態伺服器（瀏覽器直接開 `file://` 時 `fetch` 會失敗）：

```bash
cd /workspace/baystay
python3 -m http.server 8080
```

然後開啟 http://127.0.0.1:8080/

## 結構

- `data/listings.json` — 種子目錄
- `index.html` / `listings.html` / `listing.html` / `partner.html` / `about.html`
- `copy/` — 文案原稿
- `assets/style.css` / `assets/common.js`
