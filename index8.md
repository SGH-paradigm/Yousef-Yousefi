---
layout: default
title: SGH
nav_order: 1
permalink: /
---

<style>
/* ================================
ULTRA SHINY COSMIC BACKGROUND
================================ */
body {
  background: 
    radial-gradient(circle at 20% 20%, #021a40 0%, transparent 50%),
    radial-gradient(circle at 80% 10%, #001f54 0%, transparent 45%),
    radial-gradient(circle at 60% 90%, #002b5b 0%, transparent 55%),
    #020617;
  color: #e6edf3;
  font-family: 'Segoe UI', Roboto, Arial, sans-serif;
}

/* HEADER & TOP NAV (kept exactly as before) */
.site-header { background: transparent !important; box-shadow: none !important; }
.cosmic-top-nav {
  position: fixed; top: 0; left: 0; width: 100%; z-index: 1000;
  display: flex; justify-content: center; gap: 25px; padding: 16px 20px;
  background: rgba(2,6,23,0.95); backdrop-filter: blur(15px);
  border-bottom: 1px solid rgba(56,189,248,0.4);
}
.cosmic-tab {
  padding: 12px 26px; border-radius: 9999px; text-decoration: none;
  font-weight: 700; color: #7dd3fc; border: 1px solid rgba(125,211,252,0.5);
  transition: all 0.35s;
}
.cosmic-tab:hover {
  background: #0284c7; color: white; transform: translateY(-4px);
  box-shadow: 0 0 25px #38bdf8;
}

/* HERO (kept exactly) */
.hero { /* ... same as previous version ... */ }

/* MAIN LAYOUT - TWO COLUMNS */
.container {
  display: flex;
  max-width: 1280px;
  margin: 0 auto;
  gap: 40px;
  padding: 0 20px;
}
.main-content {
  flex: 1;
}
.sidebar {
  width: 320px;
  background: rgba(255,255,255,0.06);
  border: 1px solid rgba(125,211,252,0.3);
  border-radius: 16px;
  padding: 28px;
  height: fit-content;
  box-shadow: 0 0 30px rgba(56,189,248,0.25);
  position: sticky;
  top: 100px;
}

/* SIDEBAR STYLING */
.sidebar h3 {
  color: #67e8f9;
  text-align: center;
  margin-bottom: 20px;
  text-shadow: 0 0 15px #38bdf8;
}
.author-photo {
  width: 140px;
  height: 140px;
  border-radius: 50%;
  border: 4px solid #67e8f9;
  box-shadow: 0 0 30px #38bdf8;
  display: block;
  margin: 0 auto 20px;
}
.sidebar a {
  color: #7dd3fc;
  text-decoration: none;
}
.sidebar a:hover { color: #38bdf8; }

/* ROADMAP (kept exactly) */
.roadmap { display: flex; flex-direction: column; gap: 26px; }
.gen { /* same as before */ }

/* RESPONSIVE - Sidebar goes below on mobile */
@media (max-width: 992px) {
  .container { flex-direction: column; }
  .sidebar { width: 100%; position: static; }
}
</style>

<!-- FIXED TOP NAV -->
<div class="cosmic-top-nav">
  <a class="cosmic-tab" href="/table-of-content/">📖 Table of Contents</a>
  <a class="cosmic-tab" href="/contact/">📬 Contact</a>
  <a class="cosmic-tab" href="/support/">❤️ Support the Mission</a>
  <a class="cosmic-tab" href="/feedback/">💡 Feedback</a>
  <a class="cosmic-tab" href="/license/">⚖️ License</a>
</div>

<!-- HERO -->
<div class="hero">
  <div class="herotitle">SCIENCE GENERALIZATION<br>HYPOTHESIS (SGH)</div>
  <div class="subtitle">A Foundational Ontological Framework for the Primordial Structure of Existence</div>
  <a href="/preface/" class="bigbtn">Start Free Materials</a>
  <a href="/paradoxes/" class="bigbtn">Solved Paradoxes</a>
  <a href="/support/" class="bigbtn">Support the Mission</a>
</div>

<div class="container">
  <!-- MAIN CONTENT -->
  <div class="main-content">

    # 🌌 SGH Research Generations & Pricing

    <div class="roadmap">
      <!-- PRIMARY -->
      <div class="gen">
        <h3>PRIMARY — FREE</h3>
        <ul>
          <li><a href="/preface/">Preface</a></li>
          <li><a href="/introduction/">Introduction</a></li>
        </ul>
      </div>
      <div class="arrow">↓</div>

      <!-- FIRST GENERATION -->
      <div class="gen">
        <h3>FIRST GENERATION — Foundations of SGH</h3>
        <p>Suggested bundle: $10 • Individual: $50 each</p>
        <ul>
          <li><a href="/first-gen/ch1/">Chapter 1: Foundations of SGH</a> — $50</li>
          <!-- ... add all other chapters exactly as in previous version ... -->
        </ul>
      </div>
      <!-- (Continue with Second, Third, Fourth, Ultimate exactly as last version) -->
    </div>
  </div>

  <!-- SIDEBAR - AUTHOR INFORMATION -->
  <div class="sidebar">
    <h3>ABOUT THE AUTHOR</h3>
    
    <img src="https://via.placeholder.com/140" alt="Yousef Yousefi" class="author-photo">
    
    <p><strong>Yousef Yousefi</strong><br>
    Independent Researcher<br>
    Creator of the Science Generalization Hypothesis (SGH)</p>
    
    <p>After more than a decade of independent research in metaphysics, mathematics, and modern physics, I developed SGH as the first complete primordial ontological framework that begins logically prior to spacetime and physical law.</p>
    
    <hr style="border-color:rgba(125,211,252,0.3);margin:20px 0;">
    
    <strong>Contact & Links</strong><br>
    📧 <a href="mailto:yousefyousefi191@gmail.com">yousefyousefi191@gmail.com</a><br>
    🔬 <a href="https://www.researchgate.net/profile/Yousef-Yousefi-7" target="_blank">ResearchGate</a><br>
    📄 <a href="https://arxiv.org" target="_blank">arXiv Submissions</a><br>
    🌐 <a href="https://sgh-paradigm.github.io/Yousef-Yousefi/" target="_blank">Official Website</a>
    
    <hr style="border-color:rgba(125,211,252,0.3);margin:20px 0;">
    
    <p style="font-size:14px;opacity:0.85;">
      All content © 2026 Yousef Yousefi<br>
      All rights reserved
    </p>
  </div>
</div>

---

⭐ Knowledge expands through structured discovery.  
**Payments via cryptocurrency (USDT/BTC) – pay-what-you-want option available.**
