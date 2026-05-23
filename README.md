<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Miya 越式洗髮館｜高雄左營 頭皮舒壓・越式洗髮・肩頸放鬆</title>
  <meta name="description" content="Miya 越式洗髮館位於高雄左營華夏路，提供越式洗髮、頭皮放鬆、臉部與肩頸舒壓。立即透過電話、LINE 或 Google Map 預約放鬆時光。" />
  <style>
    :root {
      --bg: #fffaf4;
      --cream: #fff3e4;
      --brown: #5b3726;
      --brown-2: #7b4b32;
      --gold: #c99754;
      --green: #62785f;
      --text: #2d211b;
      --muted: #7b6d64;
      --white: #ffffff;
      --shadow: 0 22px 60px rgba(91, 55, 38, 0.14);
      --radius: 28px;
    }

    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: -apple-system, BlinkMacSystemFont, "Noto Sans TC", "Segoe UI", sans-serif;
      color: var(--text);
      background: var(--bg);
      line-height: 1.7;
    }

    a { color: inherit; text-decoration: none; }

    .topbar {
      position: sticky;
      top: 0;
      z-index: 50;
      backdrop-filter: blur(18px);
      background: rgba(255, 250, 244, 0.86);
      border-bottom: 1px solid rgba(91,55,38,.08);
    }

    .nav {
      max-width: 1180px;
      margin: auto;
      padding: 14px 22px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 18px;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 12px;
      font-weight: 800;
      color: var(--brown);
      letter-spacing: .5px;
    }

    .logo {
      width: 42px;
      height: 42px;
      border-radius: 50%;
      display: grid;
      place-items: center;
      background: linear-gradient(145deg, var(--gold), #efd3a3);
      color: white;
      box-shadow: 0 8px 24px rgba(201,151,84,.3);
      font-family: Georgia, serif;
      font-size: 24px;
    }

    .nav-links {
      display: flex;
      gap: 18px;
      align-items: center;
      color: var(--muted);
      font-size: 15px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      padding: 13px 20px;
      border-radius: 999px;
      font-weight: 800;
      transition: .2s ease;
      cursor: pointer;
      border: 0;
      white-space: nowrap;
    }

    .btn-primary {
      background: var(--brown);
      color: white;
      box-shadow: 0 14px 32px rgba(91,55,38,.24);
    }
    .btn-primary:hover { transform: translateY(-2px); background: #442719; }

    .btn-line {
      background: #06c755;
      color: white;
      box-shadow: 0 14px 32px rgba(6,199,85,.18);
    }

    .btn-soft {
      background: white;
      color: var(--brown);
      border: 1px solid rgba(91,55,38,.12);
    }

    .hero {
      max-width: 1180px;
      margin: auto;
      padding: 64px 22px 40px;
      display: grid;
      grid-template-columns: 1.05fr .95fr;
      gap: 44px;
      align-items: center;
    }

    .eyebrow {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 8px 14px;
      border-radius: 999px;
      background: rgba(201,151,84,.14);
      color: var(--brown-2);
      font-weight: 800;
      font-size: 14px;
    }

    h1 {
      margin: 20px 0 18px;
      font-size: clamp(42px, 6vw, 76px);
      line-height: 1.05;
      letter-spacing: -2px;
      color: var(--brown);
    }

    .lead {
      font-size: 20px;
      color: var(--muted);
      max-width: 620px;
      margin-bottom: 26px;
    }

    .hero-actions { display: flex; gap: 12px; flex-wrap: wrap; margin-bottom: 26px; }

    .trust-row {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 12px;
      max-width: 610px;
    }

    .trust-card {
      background: rgba(255,255,255,.72);
      border: 1px solid rgba(91,55,38,.09);
      padding: 16px;
      border-radius: 20px;
      box-shadow: 0 10px 28px rgba(91,55,38,.06);
    }
    .trust-card strong { display: block; color: var(--brown); font-size: 20px; }
    .trust-card span { color: var(--muted); font-size: 13px; }

    .hero-visual {
      position: relative;
      min-height: 560px;
      border-radius: 42px;
      overflow: hidden;
      background:
        radial-gradient(circle at 30% 18%, rgba(255,255,255,.95), transparent 32%),
        linear-gradient(145deg, #f7d7b0, #fbefe2 45%, #d7b38b);
      box-shadow: var(--shadow);
      padding: 28px;
      display: flex;
      align-items: flex-end;
    }

    .hero-visual::before {
      content: "";
      position: absolute;
      inset: 34px;
      border-radius: 34px;
      border: 1px solid rgba(255,255,255,.55);
    }

    .visual-card {
      position: relative;
      width: 100%;
      background: rgba(255,255,255,.84);
      border: 1px solid rgba(255,255,255,.8);
      border-radius: 30px;
      padding: 24px;
      box-shadow: 0 18px 60px rgba(91,55,38,.16);
    }

    .visual-card h2 { margin: 0 0 8px; color: var(--brown); font-size: 28px; }
    .visual-card p { margin: 0; color: var(--muted); }

    .floating {
      position: absolute;
      top: 34px;
      right: 30px;
      width: 160px;
      background: rgba(255,255,255,.9);
      padding: 16px;
      border-radius: 24px;
      box-shadow: 0 16px 44px rgba(91,55,38,.13);
      font-weight: 800;
      color: var(--brown);
    }
    .floating small { display: block; color: var(--muted); font-weight: 600; }

    .section {
      max-width: 1180px;
      margin: auto;
      padding: 76px 22px;
    }

    .section-title {
      max-width: 720px;
      margin-bottom: 28px;
    }
    .section-title h2 { font-size: clamp(32px, 4vw, 52px); line-height: 1.12; color: var(--brown); margin: 0 0 12px; }
    .section-title p { color: var(--muted); font-size: 18px; margin: 0; }

    .services {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 18px;
    }

    .service {
      background: white;
      border-radius: var(--radius);
      padding: 26px;
      box-shadow: 0 16px 42px rgba(91,55,38,.08);
      border: 1px solid rgba(91,55,38,.08);
    }
    .service .icon { font-size: 34px; }
    .service h3 { color: var(--brown); margin: 16px 0 8px; font-size: 21px; }
    .service p { color: var(--muted); margin: 0; font-size: 15px; }

    .offer {
      background: linear-gradient(135deg, var(--brown), #8a5736);
      color: white;
      border-radius: 38px;
      padding: 40px;
      display: grid;
      grid-template-columns: 1fr auto;
      gap: 24px;
      align-items: center;
      box-shadow: var(--shadow);
    }
    .offer h2 { margin: 0 0 8px; font-size: 38px; line-height: 1.15; }
    .offer p { margin: 0; color: rgba(255,255,255,.82); font-size: 18px; }
    .price { font-size: 48px; font-weight: 900; color: #ffe1aa; }
    .price small { display: block; font-size: 14px; color: rgba(255,255,255,.7); text-align: right; }

    .packages {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 18px;
    }
    .package {
      background: white;
      border-radius: 30px;
      padding: 30px;
      border: 1px solid rgba(91,55,38,.08);
      box-shadow: 0 16px 40px rgba(91,55,38,.07);
    }
    .package.featured { border: 2px solid var(--gold); transform: translateY(-8px); }
    .tag { display: inline-block; background: var(--cream); color: var(--brown); padding: 6px 12px; border-radius: 999px; font-size: 13px; font-weight: 800; }
    .package h3 { color: var(--brown); font-size: 25px; margin: 18px 0 8px; }
    .package ul { padding-left: 18px; color: var(--muted); margin: 14px 0 22px; }
    .package li { margin: 6px 0; }

    .why {
      display: grid;
      grid-template-columns: .9fr 1.1fr;
      gap: 32px;
      align-items: center;
    }
    .why-box {
      background: var(--cream);
      border-radius: 36px;
      padding: 34px;
      min-height: 360px;
      display: grid;
      place-items: center;
      text-align: center;
      color: var(--brown);
    }
    .why-box .big { font-size: 72px; font-weight: 900; line-height: 1; }
    .why-list { display: grid; gap: 16px; }
    .why-item { background: white; padding: 22px; border-radius: 24px; box-shadow: 0 12px 36px rgba(91,55,38,.07); }
    .why-item strong { color: var(--brown); font-size: 18px; }
    .why-item p { margin: 6px 0 0; color: var(--muted); }

    .location-card {
      background: white;
      border-radius: 38px;
      padding: 34px;
      box-shadow: var(--shadow);
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 26px;
      align-items: center;
    }
    .map-placeholder {
      min-height: 340px;
      border-radius: 30px;
      background:
        linear-gradient(rgba(91,55,38,.2), rgba(91,55,38,.2)),
        radial-gradient(circle at 25% 30%, #d9e2d1, transparent 24%),
        radial-gradient(circle at 70% 40%, #ead3a9, transparent 28%),
        linear-gradient(145deg, #f2eadc, #dbc5a4);
      display: grid;
      place-items: center;
      color: white;
      text-align: center;
      padding: 24px;
      position: relative;
      overflow: hidden;
    }
    .pin { font-size: 58px; filter: drop-shadow(0 12px 24px rgba(0,0,0,.2)); }

    .contact-list { display: grid; gap: 12px; color: var(--muted); }
    .contact-list strong { color: var(--brown); }

    .reviews {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 18px;
    }
    .review {
      background: white;
      border-radius: 28px;
      padding: 24px;
      box-shadow: 0 14px 36px rgba(91,55,38,.07);
      border: 1px solid rgba(91,55,38,.07);
    }
    .stars { color: #d89b24; letter-spacing: 2px; }
    .review p { color: var(--muted); }

    .final-cta {
      text-align: center;
      background: linear-gradient(135deg, #fff7ee, #edd4b5);
      border-radius: 42px;
      padding: 54px 24px;
      box-shadow: var(--shadow);
    }
    .final-cta h2 { font-size: clamp(34px, 4vw, 58px); color: var(--brown); margin: 0 0 14px; line-height: 1.1; }
    .final-cta p { color: var(--muted); margin: 0 auto 24px; max-width: 660px; font-size: 18px; }

    footer {
      padding: 34px 22px 96px;
      text-align: center;
      color: var(--muted);
      font-size: 14px;
    }

    .mobile-cta {
      position: fixed;
      left: 12px;
      right: 12px;
      bottom: 12px;
      z-index: 80;
      display: none;
      gap: 10px;
      background: rgba(255,255,255,.86);
      backdrop-filter: blur(18px);
      padding: 10px;
      border-radius: 999px;
      box-shadow: 0 18px 50px rgba(91,55,38,.2);
    }
    .mobile-cta .btn { flex: 1; padding: 12px 10px; font-size: 14px; }

    @media (max-width: 900px) {
      .nav-links { display: none; }
      .hero, .why, .location-card { grid-template-columns: 1fr; }
      .hero-visual { min-height: 430px; }
      .services, .packages, .reviews { grid-template-columns: 1fr; }
      .trust-row { grid-template-columns: 1fr; }
      .offer { grid-template-columns: 1fr; text-align: left; }
      .price small { text-align: left; }
      .package.featured { transform: none; }
      .mobile-cta { display: flex; }
    }
  </style>
</head>
<body>
  <div class="topbar">
    <nav class="nav">
      <a class="brand" href="#top" aria-label="Miya 越式洗髮館首頁">
        <span class="logo">M</span>
        <span>Miya 越式洗髮館</span>
      </a>
      <div class="nav-links">
        <a href="#services">服務</a>
        <a href="#packages">方案</a>
        <a href="#location">位置</a>
        <a href="#reviews">評價</a>
        <a class="btn btn-primary" href="tel:0900439213">立即預約</a>
      </div>
    </nav>
  </div>

  <main id="top">
    <section class="hero">
      <div>
        <span class="eyebrow">高雄左營｜越式洗髮・頭皮舒壓・肩頸放鬆</span>
        <h1>今天，讓頭皮先替你放假。</h1>
        <p class="lead">Miya 以溫柔洗髮、頭部放鬆、臉部與肩頸舒壓，為忙碌的你安排一段真正能恢復精神的安靜時光。</p>
        <div class="hero-actions">
          <a class="btn btn-primary" href="tel:0900439213">☎ 電話預約</a>
          <a class="btn btn-line" href="https://line.me/R/ti/p/~lienlien1602" target="_blank" rel="noopener">LINE 預約</a>
          <a class="btn btn-soft" href="https://maps.app.goo.gl/hSzXBpwmcEfWkdjK6" target="_blank" rel="noopener">Google Map 導航</a>
        </div>
        <div class="trust-row">
          <div class="trust-card"><strong>70 分鐘</strong><span>放鬆型人氣體驗</span></div>
          <div class="trust-card"><strong>高雄左營</strong><span>華夏路交通便利</span></div>
          <div class="trust-card"><strong>預約優先</strong><span>避免現場久候</span></div>
        </div>
      </div>

      <div class="hero-visual" aria-label="Miya 越式洗髮體驗示意圖">
        <div class="floating">Google 好評<br><small>歡迎查看真實評論</small></div>
        <div class="visual-card">
          <h2>越式洗髮不只是洗頭</h2>
          <p>從頭皮清潔、放鬆按摩，到肩頸舒壓，讓你走出店門時，像重新開機一樣輕盈。</p>
        </div>
      </div>
    </section>

    <section class="section" id="services">
      <div class="section-title">
        <h2>客人最容易愛上的 4 個服務感受</h2>
        <p>網站文案不只介紹服務，而是讓客人立刻想像自己放鬆後的狀態。</p>
      </div>
      <div class="services">
        <div class="service"><div class="icon">💆‍♀️</div><h3>頭部舒壓</h3><p>針對頭皮與頭部壓力感，透過放鬆手法舒緩緊繃。</p></div>
        <div class="service"><div class="icon">🫧</div><h3>溫和洗髮</h3><p>清潔頭皮與髮絲，洗去整天疲憊與悶熱感。</p></div>
        <div class="service"><div class="icon">🌿</div><h3>臉部放鬆</h3><p>搭配臉部輕柔按摩，讓表情與精神一起放鬆。</p></div>
        <div class="service"><div class="icon">🕯️</div><h3>肩頸舒緩</h3><p>久坐、低頭、工作後的肩頸緊繃，在這裡慢慢放下。</p></div>
      </div>
    </section>

    <section class="section">
      <div class="offer">
        <div>
          <h2>第一次來 Miya？從人氣 70 分鐘體驗開始。</h2>
          <p>適合下班後、約會前、旅行中、或只是想好好照顧自己的你。</p>
        </div>
        <div class="price">$990<small>70 分鐘參考方案</small></div>
      </div>
    </section>

    <section class="section" id="packages">
      <div class="section-title">
        <h2>讓客人更容易下單的服務方案</h2>
        <p>正式上線前可依店內實際價格調整；建議保留「入門、人氣、尊榮」三層級，轉換率通常更好。</p>
      </div>
      <div class="packages">
        <div class="package">
          <span class="tag">快速放鬆</span>
          <h3>清爽洗髮方案</h3>
          <ul>
            <li>頭皮清潔</li>
            <li>基礎洗髮</li>
            <li>簡易吹整</li>
          </ul>
          <a class="btn btn-soft" href="https://line.me/R/ti/p/~lienlien1602" target="_blank" rel="noopener">詢問空位</a>
        </div>
        <div class="package featured">
          <span class="tag">最多人選</span>
          <h3>70 分鐘舒壓方案</h3>
          <ul>
            <li>溫和洗髮</li>
            <li>頭部按摩</li>
            <li>臉部・頸肩舒壓</li>
          </ul>
          <a class="btn btn-primary" href="tel:0900439213">立即預約</a>
        </div>
        <div class="package">
          <span class="tag">深度享受</span>
          <h3>尊榮放鬆方案</h3>
          <ul>
            <li>完整越式洗髮體驗</li>
            <li>加強肩頸與頭部放鬆</li>
            <li>適合疲勞感明顯者</li>
          </ul>
          <a class="btn btn-soft" href="https://maps.app.goo.gl/hSzXBpwmcEfWkdjK6" target="_blank" rel="noopener">查看地點</a>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="why">
        <div class="why-box">
          <div>
            <div class="big">Miya</div>
            <p>不是趕時間的洗頭店，<br>而是一段為你保留的放鬆時間。</p>
          </div>
        </div>
        <div class="why-list">
          <div class="why-item"><strong>清楚的預約入口</strong><p>電話、LINE、Google Map 三個按鈕都放在最容易點的位置，降低客人猶豫。</p></div>
          <div class="why-item"><strong>主打「放鬆後的感覺」</strong><p>比起只列服務項目，更能讓客人感覺「我現在就需要」。</p></div>
          <div class="why-item"><strong>適合 Google Map SEO</strong><p>頁面重複強化高雄、左營、越式洗髮、頭皮舒壓等關鍵字，對在地搜尋更友善。</p></div>
        </div>
      </div>
    </section>

    <section class="section" id="location">
      <div class="location-card">
        <div>
          <div class="section-title">
            <h2>高雄左營，想放鬆時就能找到 Miya</h2>
            <p>建議預約後再前往，讓店內能為你保留最舒服的服務時段。</p>
          </div>
          <div class="contact-list">
            <div><strong>地址：</strong>高雄市左營區華夏路557號</div>
            <div><strong>電話：</strong><a href="tel:0900439213">0900-439-213</a></div>
            <div><strong>LINE：</strong><a href="https://line.me/R/ti/p/~lienlien1602" target="_blank" rel="noopener">lienlien1602</a></div>
            <div><strong>Google Map：</strong><a href="https://maps.app.goo.gl/hSzXBpwmcEfWkdjK6" target="_blank" rel="noopener">點我導航到 Miya</a></div>
          </div>
          <div class="hero-actions" style="margin-top:24px">
            <a class="btn btn-primary" href="tel:0900439213">☎ 打電話</a>
            <a class="btn btn-line" href="https://line.me/R/ti/p/~lienlien1602" target="_blank" rel="noopener">LINE 預約</a>
          </div>
        </div>
        <a class="map-placeholder" href="https://maps.app.goo.gl/hSzXBpwmcEfWkdjK6" target="_blank" rel="noopener" aria-label="開啟 Google Map 導航">
          <div>
            <div class="pin">📍</div>
            <h3>點擊開啟 Google Map</h3>
            <p>高雄市左營區華夏路557號</p>
          </div>
        </a>
      </div>
    </section>

    <section class="section" id="reviews">
      <div class="section-title">
        <h2>評價區：讓新客人放心預約</h2>
        <p>上線時建議放入 3–6 則真實 Google 評論截圖或文字，效果會比一般文案更強。</p>
      </div>
      <div class="reviews">
        <div class="review"><div class="stars">★★★★★</div><p>「洗完頭整個人很放鬆，肩頸也舒服很多，下次還會再來。」</p><strong>— Google 顧客評論</strong></div>
        <div class="review"><div class="stars">★★★★★</div><p>「環境舒服，服務親切，很適合下班後讓自己休息一下。」</p><strong>— Google 顧客評論</strong></div>
        <div class="review"><div class="stars">★★★★★</div><p>「第一次體驗越式洗髮，比想像中更放鬆，推薦預約。」</p><strong>— Google 顧客評論</strong></div>
      </div>
    </section>

    <section class="section">
      <div class="final-cta">
        <h2>現在就幫自己預約一段放鬆時間</h2>
        <p>頭皮乾淨了，肩頸鬆了，心情也會跟著變輕。Miya 在高雄左營等你。</p>
        <div class="hero-actions" style="justify-content:center">
          <a class="btn btn-primary" href="tel:0900439213">☎ 立即電話預約</a>
          <a class="btn btn-line" href="https://line.me/R/ti/p/~lienlien1602" target="_blank" rel="noopener">LINE 詢問空位</a>
          <a class="btn btn-soft" href="https://maps.app.goo.gl/hSzXBpwmcEfWkdjK6" target="_blank" rel="noopener">Google Map 導航</a>
        </div>
      </div>
    </section>
  </main>

  <div class="mobile-cta">
    <a class="btn btn-primary" href="tel:0900439213">電話</a>
    <a class="btn btn-line" href="https://line.me/R/ti/p/~lienlien1602" target="_blank" rel="noopener">LINE</a>
    <a class="btn btn-soft" href="https://maps.app.goo.gl/hSzXBpwmcEfWkdjK6" target="_blank" rel="noopener">地圖</a>
  </div>

  <footer>
    © Miya 越式洗髮館｜高雄左營越式洗髮・頭皮舒壓・肩頸放鬆<br />
    本頁為高轉換一頁式網站範本，正式上線前請確認營業時間、價格與服務內容。
  </footer>

<!--
README.md

# Miya 越式洗髮館｜高轉換品牌網站

一個為高雄 Miya 越式洗髮館打造的高質感、高轉換率 Landing Page。

## ✨ 品牌理念

Miya 不只是洗髮。
而是讓疲憊的人，在繁忙生活中，重新找回放鬆與被照顧的感覺。

我們相信：
真正好的服務，不只是技術，
而是客人離開時，整個人的狀態變好了。

---

## 🌿 Website Features

- 高轉換一頁式設計
- 手機版優化（Mobile First）
- Google Map 導流
- LINE 一鍵預約
- SEO 關鍵字設計
- 高端美容／舒壓品牌視覺
- GitHub Pages 免費部署

---

## 📍 店家資訊

Miya 越式洗髮館
高雄市左營區華夏路557號

☎ 0900-439-213

Google Map：
https://maps.app.goo.gl/hSzXBpwmcEfWkdjK6

---

## 🚀 Deployment

This website is deployed using GitHub Pages.

Live Site:
https://teamtechtaiwan-design.github.io/Miya-hair-saloon-Kaohsiung/

---

## 💡 Marketing Strategy

此網站設計重點：

- 讓客人在 5 秒內理解服務價值
- 強化「放鬆感」而不是只講洗髮
- 大幅降低預約猶豫
- 強化 Google Map SEO
- 提升 LINE 詢問率與回訪率

---

## 🖤 Brand Message

今天，讓頭皮先替你放假。

在 Miya，
放鬆不是奢侈，
而是你應該擁有的日常。

-->

</body>
</html>
