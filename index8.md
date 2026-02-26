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

/* HEADER & TOP NAV */
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

/* HERO */
.hero {
  text-align: center; padding: 160px 20px 120px; margin: 80px auto 70px;
  max-width: 1100px; border-radius: 28px;
  background: linear-gradient(145deg, #000428, #004e92);
  box-shadow: 0 0 90px rgba(56,189,248,0.7), inset 0 0 90px rgba(56,189,248,0.25);
  position: relative; overflow: hidden;
}
.hero::before {
  content: ""; position: absolute; top: -150%; left: -150%; width: 400%; height: 400%;
  background: radial-gradient(circle, rgba(103,232,249,0.35) 0%, transparent 65%);
  animation: slowPulse 26s infinite ease-in-out;
}
.herotitle {
  font-size: 96px; font-weight: 900; letter-spacing: 8px; color: #67e8f9;
  text-shadow: 0 0 15px #67e8f9, 0 0 35px #38bdf8, 0 0 70px #0284c7,
               0 0 110px #0369a1, 0 0 160px #1e40af, 0 0 220px #0e7490;
  line-height: 1.05; margin-bottom: 22px; animation: neonFlicker 3.5s infinite alternate;
}
.subtitle { font-size: 29px; opacity: 0.97; margin-bottom: 45px; text-shadow: 0 0 20px rgba(103,232,249,0.7); }
.bigbtn {
  padding: 18px 40px; margin: 12px; border-radius: 9999px;
  background: linear-gradient(90deg, #0284c7, #22d3ee); color: white;
  text-decoration: none; font-weight: 700; font-size: 17px; display: inline-block;
  box-shadow: 0 12px 35px rgba(56,189,248,0.6); transition: all 0.4s;
}
.bigbtn:hover { transform: translateY(-8px) scale(1.06); box-shadow: 0 25px 50px rgba(56,189,248,0.8); }

/* ANIMATIONS */
@keyframes neonFlicker { 0% {text-shadow:0 0 15px #67e8f9,0 0 35px #38bdf8,0 0 70px #0284c7;} 50% {text-shadow:0 0 25px #67e8f9,0 0 55px #38bdf8,0 0 100px #0284c7,0 0 140px #0369a1;} 100% {text-shadow:0 0 15px #67e8f9,0 0 35px #38bdf8,0 0 70px #0284c7;} }
@keyframes slowPulse { 0%,100% {opacity:0.65;transform:scale(0.92);} 50% {opacity:1;transform:scale(1.08);} }

/* TWO-COLUMN LAYOUT - SIDEBAR LEFT (30%) + MAIN RIGHT (70%) */
.container {
  display: flex;
  max-width: 1280px;
  margin: 40px auto;
  gap: 40px;
  padding: 0 20px;
}
.sidebar {
  width: 30%;
  background: rgba(255,255,255,0.06);
  border: 1px solid rgba(125,211,252,0.3);
  border-radius: 16px;
  padding: 28px;
  height: fit-content;
  box-shadow: 0 0 30px rgba(56,189,248,0.25);
  position: sticky;
  top: 100px;
}
.main-content {
  width: 70%;
}

/* REFINED SIDEBAR - BEAUTIFUL & CENTERED */
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
.sidebar p { text-align: center; line-height: 1.5; }
.sidebar a { color: #7dd3fc; text-decoration: none; }
.sidebar a:hover { color: #38bdf8; }

/* ROADMAP - YOUR ORIGINAL CLEAN STRUCTURE */
.roadmap {
  display: flex;
  flex-direction: column;
  gap: 26px;
}
.gen {
  padding: 30px;
  border-radius: 15px;
  background: rgba(255,255,255,.05);
  border: 1px solid rgba(125,211,252,.25);
  box-shadow: 0 0 18px rgba(56,189,248,.2);
  transition: .35s;
}
.gen:hover {
  transform: translateX(12px);
  box-shadow: 0 0 30px rgba(56,189,248,.45);
}
.arrow {
  text-align: center;
  font-size: 30px;
}

/* MOBILE - SIDEBAR GOES ON TOP */
@media (max-width: 992px) {
  .container { flex-direction: column; }
  .sidebar, .main-content { width: 100%; }
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
  <!-- LEFT SIDEBAR - AUTHOR INFORMATION -->
  <div class="sidebar">
    <h3>ABOUT THE AUTHOR</h3>
    
    <img src="https://via.placeholder.com/140" alt="Yousef Yousefi" class="author-photo">
    
    <p><strong>Yousef Yousefi</strong><br>
    Independent Researcher<br>
    Creator of the Science Generalization Hypothesis (SGH)</p>
    
    <p>After more than a decade of independent research in metaphysics, mathematics, and modern physics, I developed SGH as the first complete primordial ontological framework that begins logically prior to spacetime and physical law.</p>
    
    <hr style="border-color:rgba(125,211,252,0.3);margin:20px 0;">
    
    <strong>Contact & Links</strong><br>
    📧 <a href="mailto:yousefyousefi191@gmail.com">yousefyousefi191@gmail.com</a><br><br>
    🔬 <a href="https://www.researchgate.net/profile/Yousef-Yousefi-7" target="_blank">ResearchGate</a><br>
    📄 <a href="https://arxiv.org" target="_blank">arXiv Submissions</a><br>
    🌐 This Website
    
    <hr style="border-color:rgba(125,211,252,0.3);margin:20px 0;">
    
    <p style="font-size:14px;opacity:0.85;text-align:center;">
      © 2026 Yousef Yousefi — All rights reserved
    </p>
  </div>

  <!-- MAIN CONTENT - YOUR ROADMAP (70%) -->
  <div class="main-content">
    # 🌌 SGH Research Generations & Pricing

    <div class="roadmap">
      <div class="gen">
        <h3>PRIMARY — FREE</h3>
        <ul>
          <li><a href="/preface/">Preface</a></li>
          <li><a href="/introduction/">Introduction</a></li>
        </ul>
      </div>
      <div class="arrow">↓</div>

      <div class="gen">
        <h3>FIRST GENERATION — Foundations of SGH</h3>
        <p>Suggested bundle: $10 • Individual: $50 each</p>
        <ul>
          <li><a href="/first-gen/ch1/">Chapter 1: Foundations of SGH</a> — $50</li>
          <li><a href="/first-gen/ch2/">Chapter 2: The Creation Mechanism</a> — $50</li>
          <li><a href="/first-gen/ch3/">Chapter 3: Unified Classification</a> — $50</li>
          <li><a href="/first-gen/ch4/">Chapter 4: Mathematical Formalization</a> — $50</li>
          <li><a href="/first-gen/ch5/">Chapter 5: Physics Applications & Roadmap</a> — $50</li>
          <li><a href="/first-gen/ch6/">Chapter 6: Philosophical Implications</a> — $50</li>
          <li><a href="/first-gen/ch7/">Chapter 7: Research Roadmap</a> — $50</li>
          <li><a href="/paradoxes/first-gen/">Solved Paradox Collection</a> — $500</li>
        </ul>
      </div>
      <div class="arrow">↓</div>

      <div class="gen">
        <h3>SECOND GENERATION — Mathematical Reconstruction</h3>
        <p>Suggested bundle: $5 • Individual: $100 each</p>
        <ul>
          <li><a href="/second-gen/intro/">Science Generalization Hypothesis Roadmap Toward Unification</a> — $100</li>
          <li><a href="/second-gen/a-1-1/">A-1-1</a> — $100</li>
          <li><a href="/second-gen/a-1-2/">A-1-2</a> — $100</li>
          <li><a href="/second-gen/a-2-1/">A-2-1</a> — $100</li>
          <li><a href="/second-gen/a-2-2/">A-2-2</a> — $100</li>
          <li><a href="/second-gen/b-1-1/">B-1-1</a> — $100</li>
          <li><a href="/second-gen/b-1-2/">B-1-2</a> — $100</li>
          <li><a href="/second-gen/b-2-1/">B-2-1</a> — $100</li>
          <li><a href="/second-gen/b-2-2/">B-2-2</a> — $100</li>
          <li><a href="/second-gen/conclusion/">Conclusion</a> — $100</li>
          <li><a href="/paradoxes/second-gen/">Solved Paradox Collection</a> — $1000</li>
          <li>Results 1–8 — $100 each</li>
        </ul>
      </div>
      <div class="arrow">↓</div>

      <div class="gen">
        <h3>THIRD GENERATION — Triadic SGH</h3>
        <p>Suggested bundle: $50 • Individual: $200 each</p>
        <ul>
          <li><a href="/third-gen/toward-generalization/">Toward Generalization and Unification</a> — $200</li>
          <li><a href="/third-gen/triadic/">Triadic</a> — $200</li>
          <li><a href="/third-gen/ch1/">Chapter 1: A Foundational Ontological Framework</a> — $200</li>
          <li><a href="/third-gen/ch2/">Chapter 2: Existence Creation Mechanism</a> — $200</li>
          <li><a href="/third-gen/ch3/">Chapter 3: Unified Classification</a> — $200</li>
          <li><a href="/third-gen/implications/">Implications of Chapter 3</a> — $200</li>
          <li><a href="/third-gen/falsifiability/">Falsifiability</a> — $200</li>
          <li><a href="/third-gen/future-work/">Future Work</a> — $200</li>
          <li><a href="/paradoxes/third-gen/">Solved Paradox Collection</a> — $1000</li>
          <li>Results 1–15 — $200 each</li>
        </ul>
      </div>
      <div class="arrow">↓</div>

      <div class="gen">
        <h3>FOURTH GENERATION — Octactan SGH</h3>
        <p>Suggested bundle: $100 • Individual: $100 each</p>
        <ul>
          <li><a href="/fourth-gen/octactan/">Octactan SGH</a> — $100</li>
          <li><a href="/fourth-gen/generalization/">Generalization</a> — $100</li>
          <li><a href="/fourth-gen/unification/">Unification</a> — $100</li>
          <li><a href="/fourth-gen/future-work/">Future Work</a> — $100</li>
          <li><a href="/fourth-gen/toward-gaexitizen/">Toward Gaexitizen</a> — $100</li>
          <li>Paradox Collection — $2000</li>
        </ul>
      </div>
      <div class="arrow">↓</div>

      <div class="gen">
        <h3>ULTIMATE — Toward Gaexitizen</h3>
        <p>Suggested: $100</p>
        <ul>
          <li><a href="/ultimate/capstone/">Capstone synthesis of the entire framework</a></li>
        </ul>
      </div>
    </div>
  </div>
</div>

---

⭐ Knowledge expands through structured discovery.  
**All payments via cryptocurrency (USDT/BTC) – pay-what-you-want option available.**  
© 2026 Yousef Yousefi — All rights reserved
