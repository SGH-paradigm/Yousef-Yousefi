---
layout: default
title: "Home"
nav_order: 1
description: "Welcome to the official website of Yousef Yousefi — Researcher & Theorist."
permalink: /
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;0,900;1,700&family=DM+Sans:wght@300;400;500;600&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">

<style>
/* ── Reset & Base ─────────────────────────────────────── */
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

:root {
  --bg:        #04060f;
  --surface:   #0b0f1e;
  --border:    rgba(255,255,255,0.08);

  --gold:      #e8b84b;
  --gold-dim:  rgba(232,184,75,0.12);

  --gen0-c:    #64b5f6;  --gen0-bg: rgba(100,181,246,0.09);
  --gen1-c:    #81c784;  --gen1-bg: rgba(129,199,132,0.09);
  --gen2-c:    #ce93d8;  --gen2-bg: rgba(206,147,216,0.09);
  --gen3-c:    #ff8a65;  --gen3-bg: rgba(255,138,101,0.09);
  --gen4-c:    #4dd0e1;  --gen4-bg: rgba(77,208,225,0.09);

  --text:      #e8eaf0;
  --muted:     #8892a4;
  --font-head: 'Playfair Display', Georgia, serif;
  --font-body: 'DM Sans', system-ui, sans-serif;
  --font-mono: 'JetBrains Mono', monospace;
  --radius:    12px;
  --shadow:    0 8px 40px rgba(0,0,0,0.6);
}

/* override Just the Docs white body */
body { background: var(--bg) !important; color: var(--text) !important; font-family: var(--font-body) !important; }
.main-content { max-width: 100% !important; padding: 0 !important; }
.main-content h1, .main-content h2, .main-content h3 { border: none !important; }

/* ── Page wrapper ─────────────────────────────────────── */
.yy-page {
  max-width: 1120px;
  margin: 0 auto;
  padding: 0 24px 80px;
  font-family: var(--font-body);
}

/* ── Hero ─────────────────────────────────────────────── */
.hero {
  position: relative;
  text-align: center;
  padding: 80px 24px 60px;
  overflow: hidden;
}
.hero::before {
  content: '';
  position: absolute; inset: 0;
  background: radial-gradient(ellipse 80% 60% at 50% 0%, rgba(232,184,75,0.14) 0%, transparent 70%),
              radial-gradient(ellipse 50% 40% at 20% 80%, rgba(100,181,246,0.10) 0%, transparent 60%);
  pointer-events: none;
}
.hero-eyebrow {
  font-family: var(--font-mono);
  font-size: 11px;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: var(--gold);
  margin-bottom: 20px;
  opacity: 0;
  animation: fadeUp .6s .1s forwards;
}
.hero h1 {
  font-family: var(--font-head);
  font-size: clamp(38px, 6vw, 72px);
  font-weight: 900;
  line-height: 1.08;
  color: #fff;
  margin-bottom: 16px;
  opacity: 0;
  animation: fadeUp .7s .2s forwards;
}
.hero h1 span { color: var(--gold); }
.hero-sub {
  font-size: 16px;
  color: var(--muted);
  max-width: 580px;
  margin: 0 auto 36px;
  line-height: 1.7;
  opacity: 0;
  animation: fadeUp .7s .35s forwards;
}
.hero-badges {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  justify-content: center;
  opacity: 0;
  animation: fadeUp .7s .5s forwards;
}
.badge {
  padding: 7px 18px;
  border-radius: 40px;
  font-size: 12px;
  font-weight: 600;
  letter-spacing: .5px;
  border: 1px solid;
}
.badge-gold { background: var(--gold-dim); color: var(--gold); border-color: rgba(232,184,75,.3); }
.badge-blue { background: var(--gen0-bg); color: var(--gen0-c); border-color: rgba(100,181,246,.3); }
.badge-green { background: var(--gen1-bg); color: var(--gen1-c); border-color: rgba(129,199,132,.3); }

/* ── Section titles ───────────────────────────────────── */
.section-title {
  font-family: var(--font-head);
  font-size: 28px;
  font-weight: 700;
  color: #fff;
  margin: 60px 0 6px;
  display: flex;
  align-items: center;
  gap: 14px;
}
.section-title::after {
  content: '';
  flex: 1;
  height: 1px;
  background: var(--border);
}
.section-sub {
  color: var(--muted);
  font-size: 14px;
  margin-bottom: 32px;
}

/* ── Program Overview cards ───────────────────────────── */
.overview-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 14px;
  margin-bottom: 48px;
}
.ov-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: var(--radius);
  padding: 22px 18px;
  text-align: center;
  transition: transform .2s, box-shadow .2s;
  position: relative;
  overflow: hidden;
}
.ov-card::before {
  content: '';
  position: absolute; top: 0; left: 0; right: 0;
  height: 3px;
  border-radius: var(--radius) var(--radius) 0 0;
}
.ov-card:hover { transform: translateY(-4px); box-shadow: var(--shadow); }
.ov-gen0::before { background: var(--gen0-c); }
.ov-gen1::before { background: var(--gen1-c); }
.ov-gen2::before { background: var(--gen2-c); }
.ov-gen3::before { background: var(--gen3-c); }
.ov-gen4::before { background: var(--gen4-c); }
.ov-gen5::before { background: var(--gold); }

.ov-icon { font-size: 26px; margin-bottom: 10px; }
.ov-label {
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  margin-bottom: 6px;
}
.ov-gen0 .ov-label { color: var(--gen0-c); }
.ov-gen1 .ov-label { color: var(--gen1-c); }
.ov-gen2 .ov-label { color: var(--gen2-c); }
.ov-gen3 .ov-label { color: var(--gen3-c); }
.ov-gen4 .ov-label { color: var(--gen4-c); }
.ov-gen5 .ov-label { color: var(--gold); }

.ov-name { font-size: 13px; color: var(--text); font-weight: 500; margin-bottom: 4px; }
.ov-count { font-family: var(--font-mono); font-size: 11px; color: var(--muted); }

/* ── Research Table ───────────────────────────────────── */
.table-wrap {
  border-radius: var(--radius);
  border: 1px solid var(--border);
  overflow: hidden;
  box-shadow: var(--shadow);
}

table.catalog {
  width: 100%;
  border-collapse: collapse;
  font-size: 14px;
}
table.catalog thead tr {
  background: rgba(255,255,255,0.04);
}
table.catalog thead th {
  padding: 14px 18px;
  text-align: left;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: var(--muted);
  border-bottom: 1px solid var(--border);
}
table.catalog thead th:last-child { text-align: right; }

table.catalog tbody tr {
  border-bottom: 1px solid var(--border);
  transition: background .15s;
}
table.catalog tbody tr:last-child { border-bottom: none; }
table.catalog tbody tr:hover { background: rgba(255,255,255,0.03); }

table.catalog td {
  padding: 13px 18px;
  vertical-align: middle;
  color: var(--text);
}
table.catalog td:last-child { text-align: right; }

/* Generation header rows */
.gen-row td {
  padding: 11px 18px 10px !important;
  font-size: 11px !important;
  font-weight: 700 !important;
  letter-spacing: 2px !important;
  text-transform: uppercase !important;
  border-bottom: 1px solid var(--border) !important;
}
.gen-row-0 { background: var(--gen0-bg) !important; }
.gen-row-0 td { color: var(--gen0-c) !important; }
.gen-row-1 { background: var(--gen1-bg) !important; }
.gen-row-1 td { color: var(--gen1-c) !important; }
.gen-row-2 { background: var(--gen2-bg) !important; }
.gen-row-2 td { color: var(--gen2-c) !important; }
.gen-row-3 { background: var(--gen3-bg) !important; }
.gen-row-3 td { color: var(--gen3-c) !important; }
.gen-row-4 { background: var(--gen4-bg) !important; }
.gen-row-4 td { color: var(--gen4-c) !important; }

/* item type tag */
.item-type {
  display: inline-block;
  font-size: 10px;
  font-weight: 600;
  padding: 2px 9px;
  border-radius: 20px;
  margin-right: 8px;
  vertical-align: middle;
  letter-spacing: .5px;
}
.type-chapter  { background: rgba(129,199,132,.15); color: #81c784; border: 1px solid rgba(129,199,132,.25); }
.type-result   { background: rgba(100,181,246,.15); color: #64b5f6; border: 1px solid rgba(100,181,246,.25); }
.type-paradox  { background: rgba(255,138,101,.15); color: #ff8a65; border: 1px solid rgba(255,138,101,.25); }
.type-intro    { background: rgba(232,184,75,.15);  color: #e8b84b; border: 1px solid rgba(232,184,75,.25); }
.type-math     { background: rgba(206,147,216,.15); color: #ce93d8; border: 1px solid rgba(206,147,216,.25); }
.type-special  { background: rgba(77,208,225,.15);  color: #4dd0e1; border: 1px solid rgba(77,208,225,.25); }

/* item title link */
.item-link {
  color: var(--text);
  text-decoration: none;
  font-weight: 500;
  transition: color .15s;
}
.item-link:hover { color: var(--gold); text-decoration: underline; }

/* price pill */
.price-pill {
  display: inline-block;
  font-family: var(--font-mono);
  font-size: 12px;
  font-weight: 600;
  padding: 4px 12px;
  border-radius: 20px;
  white-space: nowrap;
}
.price-free    { background: rgba(129,199,132,.15); color: #81c784; border: 1px solid rgba(129,199,132,.25); }
.price-low     { background: rgba(100,181,246,.15); color: #64b5f6; border: 1px solid rgba(100,181,246,.25); }
.price-mid     { background: rgba(206,147,216,.15); color: #ce93d8; border: 1px solid rgba(206,147,216,.25); }
.price-high    { background: rgba(255,138,101,.15); color: #ff8a65; border: 1px solid rgba(255,138,101,.25); }
.price-top     { background: rgba(232,184,75,.15);  color: #e8b84b; border: 1px solid rgba(232,184,75,.3);  }
.price-ultimate{ background: rgba(255,82,82,.15);   color: #ff5252; border: 1px solid rgba(255,82,82,.3);  }

/* ── Info panels row ─────────────────────────────────── */
.info-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 20px;
  margin-top: 40px;
}
@media (max-width: 640px) { .info-grid { grid-template-columns: 1fr; } }

.info-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: var(--radius);
  padding: 28px;
}
.info-card h3 {
  font-family: var(--font-head);
  font-size: 18px;
  font-weight: 700;
  color: #fff;
  margin-bottom: 14px;
  display: flex;
  align-items: center;
  gap: 10px;
}
.info-card p, .info-card li { font-size: 14px; color: var(--muted); line-height: 1.75; }
.info-card ul { list-style: none; padding: 0; }
.info-card li { padding: 5px 0; border-bottom: 1px solid var(--border); }
.info-card li:last-child { border: none; }
.info-card li::before { content: '→ '; color: var(--gold); font-weight: 700; }
.info-card a { color: var(--gold); text-decoration: none; }
.info-card a:hover { text-decoration: underline; }

.news-item {
  background: rgba(232,184,75,0.05);
  border-left: 3px solid var(--gold);
  border-radius: 0 8px 8px 0;
  padding: 12px 16px;
  margin-bottom: 12px;
  font-size: 14px;
  color: var(--muted);
  line-height: 1.7;
}

/* ── Pioneer section ─────────────────────────────────── */
.pioneer-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 16px;
  margin-top: 28px;
}
.pioneer-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: var(--radius);
  padding: 24px;
  transition: transform .2s, border-color .2s;
}
.pioneer-card:hover { transform: translateY(-3px); border-color: rgba(232,184,75,.3); }
.pioneer-card .p-icon { font-size: 28px; margin-bottom: 12px; }
.pioneer-card h4 { font-size: 15px; font-weight: 700; color: #fff; margin-bottom: 8px; }
.pioneer-card p { font-size: 13px; color: var(--muted); line-height: 1.65; }

/* ── Footer ──────────────────────────────────────────── */
.yy-footer {
  text-align: center;
  margin-top: 80px;
  padding: 40px 0 0;
  border-top: 1px solid var(--border);
}
.yy-footer p { font-size: 14px; color: var(--muted); line-height: 2; }
.yy-footer .gold { color: var(--gold); }

/* ── Animation ───────────────────────────────────────── */
@keyframes fadeUp {
  from { opacity:0; transform: translateY(18px); }
  to   { opacity:1; transform: translateY(0); }
}
.animate { opacity:0; animation: fadeUp .6s forwards; }

/* ── Scrollbar ───────────────────────────────────────── */
::-webkit-scrollbar { width: 6px; }
::-webkit-scrollbar-track { background: var(--bg); }
::-webkit-scrollbar-thumb { background: rgba(232,184,75,.3); border-radius: 3px; }

/* ── Mobile ───────────────────────────────────────────── */
@media (max-width: 700px) {
  .hero h1 { font-size: 34px; }
  table.catalog thead th:nth-child(2),
  table.catalog td:nth-child(2) { display: none; }
}
</style>

<div class="yy-page">

<!-- ══════════════════════════════════════════════════════ -->
<!--  HERO                                                  -->
<!-- ══════════════════════════════════════════════════════ -->
<div class="hero">
  <div class="hero-eyebrow">Science Generalization Hypothesis · SGH Research Program</div>
  <h1>Yousef <span>Yousefi</span></h1>
  <p class="hero-sub">
    Researcher &amp; theorist exploring the deep ontological foundations of physical reality.
    Decades of original work spanning five generations of the SGH framework — from primordial
    existence to unified physics.
  </p>
  <div class="hero-badges">
    <span class="badge badge-gold">★ Pay-What-You-Want</span>
    <span class="badge badge-blue">USDT · BTC Accepted</span>
    <span class="badge badge-green">5 Research Generations</span>
  </div>
</div>

<!-- ══════════════════════════════════════════════════════ -->
<!--  PROGRAM OVERVIEW                                      -->
<!-- ══════════════════════════════════════════════════════ -->
<div class="section-title">📐 Research Program Overview</div>
<p class="section-sub">The full SGH program spans five generations, each building on the last — from foundational ontology to ultimate unification.</p>

<div class="overview-grid">
  <div class="ov-card ov-gen0">
    <div class="ov-icon">📖</div>
    <div class="ov-label">Primary</div>
    <div class="ov-name">Preface &amp; Introduction</div>
    <div class="ov-count">2 documents · Free</div>
  </div>
  <div class="ov-card ov-gen1">
    <div class="ov-icon">🔬</div>
    <div class="ov-label">1st Generation</div>
    <div class="ov-name">Foundations of SGH</div>
    <div class="ov-count">10 papers · from $50</div>
  </div>
  <div class="ov-card ov-gen2">
    <div class="ov-icon">🧮</div>
    <div class="ov-label">2nd Generation</div>
    <div class="ov-name">Mathematical Reconstruction</div>
    <div class="ov-count">5 papers · from $100</div>
  </div>
  <div class="ov-card ov-gen3">
    <div class="ov-icon">🌐</div>
    <div class="ov-label">3rd Generation</div>
    <div class="ov-name">Triadic SGH</div>
    <div class="ov-count">50 papers · from $200</div>
  </div>
  <div class="ov-card ov-gen4">
    <div class="ov-icon">🔷</div>
    <div class="ov-label">4th Generation</div>
    <div class="ov-name">Octactan SGH</div>
    <div class="ov-count">100 papers · from $100</div>
  </div>
  <div class="ov-card ov-gen5">
    <div class="ov-icon">🌌</div>
    <div class="ov-label">Ultimate</div>
    <div class="ov-name">Toward Gaexitizen</div>
    <div class="ov-count">100 papers · from $100</div>
  </div>
</div>

<!-- ══════════════════════════════════════════════════════ -->
<!--  MAIN CATALOG TABLE                                    -->
<!-- ══════════════════════════════════════════════════════ -->
<div class="section-title">📚 Complete Research Catalog</div>
<p class="section-sub">All documents are available individually. Click any title to access. Prices are suggested — pay what you wish.</p>

<div class="table-wrap">
<table class="catalog">
  <thead>
    <tr>
      <th style="width:42%">Document</th>
      <th style="width:22%">Type</th>
      <th style="width:22%">Generation</th>
      <th style="width:14%">Price</th>
    </tr>
  </thead>
  <tbody>

    <!-- ── PRIMARY ── -->
    <tr class="gen-row gen-row-0">
      <td colspan="4">📖 &nbsp; PRIMARY  —  Open Access</td>
    </tr>
    <tr>
      <td><a class="item-link" href="/preface/" target="_blank">Preface</a></td>
      <td><span class="item-type type-intro">Intro</span></td>
      <td style="color:var(--gen0-c); font-size:12px; font-weight:600;">Primary</td>
      <td><span class="price-pill price-free">FREE</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/introduction/" target="_blank">Introduction</a></td>
      <td><span class="item-type type-intro">Intro</span></td>
      <td style="color:var(--gen0-c); font-size:12px; font-weight:600;">Primary</td>
      <td><span class="price-pill price-free">FREE</span></td>
    </tr>

    <!-- ── 1ST GENERATION ── -->
    <tr class="gen-row gen-row-1">
      <td colspan="4">🔬 &nbsp; FIRST GENERATION  —  Foundations of SGH</td>
    </tr>
    <tr>
      <td><a class="item-link" href="/first-gen/ch1/" target="_blank">Chapter 1: Foundations of SGH</a></td>
      <td><span class="item-type type-chapter">Chapter</span></td>
      <td style="color:var(--gen1-c); font-size:12px; font-weight:600;">1st Generation</td>
      <td><span class="price-pill price-low">$50</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/first-gen/ch2/" target="_blank">Chapter 2: The Creation Mechanism</a></td>
      <td><span class="item-type type-chapter">Chapter</span></td>
      <td style="color:var(--gen1-c); font-size:12px; font-weight:600;">1st Generation</td>
      <td><span class="price-pill price-low">$50</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/first-gen/ch3/" target="_blank">Chapter 3: Unified Classification</a></td>
      <td><span class="item-type type-chapter">Chapter</span></td>
      <td style="color:var(--gen1-c); font-size:12px; font-weight:600;">1st Generation</td>
      <td><span class="price-pill price-low">$50</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/first-gen/ch4/" target="_blank">Chapter 4: Mathematical Formalization</a></td>
      <td><span class="item-type type-chapter">Chapter</span></td>
      <td style="color:var(--gen1-c); font-size:12px; font-weight:600;">1st Generation</td>
      <td><span class="price-pill price-low">$50</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/first-gen/ch5/" target="_blank">Chapter 5: Physics Applications &amp; Roadmap</a></td>
      <td><span class="item-type type-chapter">Chapter</span></td>
      <td style="color:var(--gen1-c); font-size:12px; font-weight:600;">1st Generation</td>
      <td><span class="price-pill price-low">$50</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/first-gen/ch6/" target="_blank">Chapter 6: Philosophical Implications</a></td>
      <td><span class="item-type type-chapter">Chapter</span></td>
      <td style="color:var(--gen1-c); font-size:12px; font-weight:600;">1st Generation</td>
      <td><span class="price-pill price-low">$50</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/first-gen/ch7/" target="_blank">Chapter 7: Research Roadmap</a></td>
      <td><span class="item-type type-chapter">Chapter</span></td>
      <td style="color:var(--gen1-c); font-size:12px; font-weight:600;">1st Generation</td>
      <td><span class="price-pill price-low">$50</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/first-gen/solved-paradox/" target="_blank">⚡ Solved Paradox Collection</a></td>
      <td><span class="item-type type-paradox">Paradox</span></td>
      <td style="color:var(--gen1-c); font-size:12px; font-weight:600;">1st Generation</td>
      <td><span class="price-pill price-high">$500</span></td>
    </tr>

    <!-- ── 2ND GENERATION ── -->
    <tr class="gen-row gen-row-2">
      <td colspan="4">🧮 &nbsp; SECOND GENERATION  —  Mathematical Reconstruction</td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/toward-unification/" target="_blank">SGH Road Map: Toward Unification — Introduction</a></td>
      <td><span class="item-type type-intro">Intro</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/a-1-1/" target="_blank">SGH Mathematics Reconstruction — A-1-1</a></td>
      <td><span class="item-type type-math">Math</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/a-1-2/" target="_blank">SGH Mathematics Reconstruction — A-1-2</a></td>
      <td><span class="item-type type-math">Math</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/a-2-1/" target="_blank">SGH Mathematics Reconstruction — A-2-1</a></td>
      <td><span class="item-type type-math">Math</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/a-2-2/" target="_blank">SGH Mathematics Reconstruction — A-2-2</a></td>
      <td><span class="item-type type-math">Math</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/b-1-1/" target="_blank">SGH Mathematics Reconstruction — B-1-1</a></td>
      <td><span class="item-type type-math">Math</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/b-1-2/" target="_blank">SGH Mathematics Reconstruction — B-1-2</a></td>
      <td><span class="item-type type-math">Math</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/b-2-1/" target="_blank">SGH Mathematics Reconstruction — B-2-1</a></td>
      <td><span class="item-type type-math">Math</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/b-2-2/" target="_blank">SGH Mathematics Reconstruction — B-2-2</a></td>
      <td><span class="item-type type-math">Math</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/conclusion/" target="_blank">Conclusion</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/solved-paradox/" target="_blank">⚡ Solved Paradox Collection</a></td>
      <td><span class="item-type type-paradox">Paradox</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-top">$1,000</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/result1/" target="_blank">Result 1</a></td>
      <td><span class="item-type type-result">Result</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/result2/" target="_blank">Result 2</a></td>
      <td><span class="item-type type-result">Result</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/result3/" target="_blank">Result 3</a></td>
      <td><span class="item-type type-result">Result</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/result4/" target="_blank">Result 4</a></td>
      <td><span class="item-type type-result">Result</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/result5/" target="_blank">Result 5</a></td>
      <td><span class="item-type type-result">Result</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/result6/" target="_blank">Result 6</a></td>
      <td><span class="item-type type-result">Result</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/result7/" target="_blank">Result 7</a></td>
      <td><span class="item-type type-result">Result</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/second-gen/result8/" target="_blank">Result 8</a></td>
      <td><span class="item-type type-result">Result</span></td>
      <td style="color:var(--gen2-c); font-size:12px; font-weight:600;">2nd Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>

    <!-- ── 3RD GENERATION ── -->
    <tr class="gen-row gen-row-3">
      <td colspan="4">🌐 &nbsp; THIRD GENERATION  —  Triadic SGH · Toward Generalization &amp; Unification</td>
    </tr>
    <tr>
      <td><a class="item-link" href="/third-gen/toward-generalization/" target="_blank">Toward Generalization and Unification</a></td>
      <td><span class="item-type type-intro">Intro</span></td>
      <td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td>
      <td><span class="price-pill price-high">$200</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/third-gen/triadic/" target="_blank">Triadic SGH Framework</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td>
      <td><span class="price-pill price-high">$200</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/third-gen/ch1/" target="_blank">Chapter 1: A Foundational Ontological Framework for the Primordial Structure of Existence</a></td>
      <td><span class="item-type type-chapter">Chapter</span></td>
      <td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td>
      <td><span class="price-pill price-high">$200</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/third-gen/ch2/" target="_blank">Chapter 2: Existence Creation — The Mechanism by Which Existence Comes to Be</a></td>
      <td><span class="item-type type-chapter">Chapter</span></td>
      <td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td>
      <td><span class="price-pill price-high">$200</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/third-gen/ch3/" target="_blank">Chapter 3: SGH — A Unified Framework &amp; Classification</a></td>
      <td><span class="item-type type-chapter">Chapter</span></td>
      <td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td>
      <td><span class="price-pill price-high">$200</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/third-gen/implication-ch3/" target="_blank">Implications of Chapter 3</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td>
      <td><span class="price-pill price-high">$200</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/third-gen/falsifiability/" target="_blank">Falsifiability &amp; Empirical Testability</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td>
      <td><span class="price-pill price-high">$200</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/third-gen/future-work/" target="_blank">Future Work &amp; Open Questions</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td>
      <td><span class="price-pill price-high">$200</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/third-gen/solved-paradox/" target="_blank">⚡ Solved Paradox Collection</a></td>
      <td><span class="item-type type-paradox">Paradox</span></td>
      <td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td>
      <td><span class="price-pill price-top">$1,000</span></td>
    </tr>
    <tr><td><a class="item-link" href="/third-gen/result1/" target="_blank">Result 1</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result2/" target="_blank">Result 2</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result3/" target="_blank">Result 3</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result4/" target="_blank">Result 4</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result5/" target="_blank">Result 5</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result6/" target="_blank">Result 6</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result7/" target="_blank">Result 7</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result8/" target="_blank">Result 8</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result9/" target="_blank">Result 9</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result10/" target="_blank">Result 10</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result11/" target="_blank">Result 11</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result12/" target="_blank">Result 12</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result13/" target="_blank">Result 13</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result14/" target="_blank">Result 14</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/result15/" target="_blank">Result 15</a></td><td><span class="item-type type-result">Result</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/paradox1/" target="_blank">Paradox I</a></td><td><span class="item-type type-paradox">Paradox</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>
    <tr><td><a class="item-link" href="/third-gen/paradox2/" target="_blank">Paradox II</a></td><td><span class="item-type type-paradox">Paradox</span></td><td style="color:var(--gen3-c); font-size:12px; font-weight:600;">3rd Generation</td><td><span class="price-pill price-high">$200</span></td></tr>

    <!-- ── 4TH GENERATION ── -->
    <tr class="gen-row gen-row-4">
      <td colspan="4">🔷 &nbsp; FOURTH GENERATION  —  Octactan SGH · Advanced Unification</td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/octactan/" target="_blank">Octactan SGH Framework</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/generalization/" target="_blank">Generalization</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/implication1/" target="_blank">Implication I</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/implication2/" target="_blank">Implication II</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/implication3/" target="_blank">Implication III</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/implication4/" target="_blank">Implication IV</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/paradox1/" target="_blank">Paradox I</a></td>
      <td><span class="item-type type-paradox">Paradox</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/paradox2/" target="_blank">Paradox II</a></td>
      <td><span class="item-type type-paradox">Paradox</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/paradox3/" target="_blank">Paradox III</a></td>
      <td><span class="item-type type-paradox">Paradox</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/paradox4/" target="_blank">Paradox IV</a></td>
      <td><span class="item-type type-paradox">Paradox</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/paradox5/" target="_blank">⚡ Grand Unified Paradox</a></td>
      <td><span class="item-type type-paradox">Paradox</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-ultimate">$2,000</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/unification/" target="_blank">Unification</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/future-work/" target="_blank">Future Work</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>
    <tr>
      <td><a class="item-link" href="/fourth-gen/toward-gaexitizen/" target="_blank">Toward Gaexitizen</a></td>
      <td><span class="item-type type-special">Special</span></td>
      <td style="color:var(--gen4-c); font-size:12px; font-weight:600;">4th Generation</td>
      <td><span class="price-pill price-mid">$100</span></td>
    </tr>

  </tbody>
</table>
</div>

<!-- ══════════════════════════════════════════════════════ -->
<!--  PIONEER SECTION                                       -->
<!-- ══════════════════════════════════════════════════════ -->
<div class="section-title">🚀 Pioneer &amp; Speculative Frontiers</div>
<p class="section-sub">Visionary possibilities that could reshape humanity's future — grounded in the SGH framework.</p>

<div class="pioneer-grid">
  <div class="pioneer-card">
    <div class="p-icon">🛸</div>
    <h4>Interstellar Travel</h4>
    <p>Manipulating the reality parameter χ may enable new propulsion methods and access to other dimensions.</p>
  </div>
  <div class="pioneer-card">
    <div class="p-icon">🧬</div>
    <h4>Medical Revolutions</h4>
    <p>Potential applications in cellular repair, reversing entropy, and understanding consciousness at its root.</p>
  </div>
  <div class="pioneer-card">
    <div class="p-icon">🔭</div>
    <h4>Next-Gen Discovery Tools</h4>
    <p>Detectors sensitive to χ-transitions and experiments to reveal hidden structures in the cosmos.</p>
  </div>
  <div class="pioneer-card">
    <div class="p-icon">⚙️</div>
    <h4>Engineering Gravity</h4>
    <p>Locally shifting χ to engineer gravity and inertia — a path toward revolutionary propulsion vehicles.</p>
  </div>
</div>
<p style="margin-top:18px; font-size:14px;">
  👉 <a href="/pioneer/" style="color:var(--gold); text-decoration:none; font-weight:600;">Read More about Pioneer Research →</a>
</p>

<!-- ══════════════════════════════════════════════════════ -->
<!--  INFO PANELS                                           -->
<!-- ══════════════════════════════════════════════════════ -->
<div class="info-grid">
  <div class="info-card">
    <h3>📢 Latest News</h3>
    <div class="news-item">
      📜 Official papers are being simultaneously submitted to academic repositories.
    </div>
    <ul>
      <li><a href="https://arxiv.org" target="_blank">arXiv.org</a></li>
      <li><a href="https://www.researchgate.net/profile/Yousef-Yousefi-7" target="_blank">ResearchGate</a></li>
      <li><a href="https://sgh-paradigm.github.io/Yousef-Yousefi/" target="_blank">This Website</a></li>
    </ul>
    <p style="margin-top:14px;">Stay tuned for updates and new breakthroughs!</p>
  </div>
  <div class="info-card">
    <h3>💳 How to Purchase</h3>
    <ul>
      <li>All prices are <strong style="color:var(--gold)">pay-what-you-want</strong> — pay less or more</li>
      <li>Payments via <strong style="color:var(--gold)">USDT or BTC</strong> cryptocurrency</li>
      <li>Each document available <strong style="color:var(--gold)">individually</strong></li>
      <li>Generation <strong style="color:var(--gold)">bundles</strong> available on request</li>
      <li>Contact via the <a href="/contact/">Contact page</a> for payment details</li>
    </ul>
  </div>
</div>

<!-- ══════════════════════════════════════════════════════ -->
<!--  FOOTER                                                -->
<!-- ══════════════════════════════════════════════════════ -->
<div class="yy-footer">
  <p>
    <span class="gold">✦</span> &nbsp;
    <strong style="color:#fff;">Yousef Yousefi</strong> — Science Generalization Hypothesis
    &nbsp; <span class="gold">✦</span>
  </p>
  <p>Knowledge grows by sharing and expanding ideas.</p>
  <p style="margin-top:8px;">
    <a href="/contact/" style="color:var(--gold); text-decoration:none; margin:0 14px;">Contact</a>
    <a href="/paradoxes/" style="color:var(--gold); text-decoration:none; margin:0 14px;">Paradoxes</a>
    <a href="/pioneer/" style="color:var(--gold); text-decoration:none; margin:0 14px;">Pioneer</a>
  </p>
</div>

</div><!-- .yy-page -->

<script>
// Staggered fade-in for table rows on scroll
const observer = new IntersectionObserver((entries) => {
  entries.forEach((e, i) => {
    if (e.isIntersecting) {
      setTimeout(() => {
        e.target.style.opacity = '1';
        e.target.style.transform = 'translateY(0)';
      }, i * 18);
      observer.unobserve(e.target);
    }
  });
}, { threshold: 0.05 });

document.querySelectorAll('.catalog tbody tr').forEach(row => {
  row.style.opacity = '0';
  row.style.transform = 'translateY(10px)';
  row.style.transition = 'opacity .35s ease, transform .35s ease';
  observer.observe(row);
});

// Overview cards stagger
document.querySelectorAll('.ov-card, .pioneer-card').forEach((card, i) => {
  card.style.opacity = '0';
  card.style.transform = 'translateY(16px)';
  card.style.transition = `opacity .4s ${i*0.07}s ease, transform .4s ${i*0.07}s ease`;
  setTimeout(() => {
    card.style.opacity = '1';
    card.style.transform = 'translateY(0)';
  }, 300 + i * 70);
});
</script>
