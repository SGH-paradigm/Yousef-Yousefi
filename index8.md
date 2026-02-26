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

/* HEADER CLEAN */
.site-header {
  background: transparent !important;
  box-shadow: none !important;
}

/* FIXED GLOWING TOP NAV */
.cosmic-top-nav {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000;
  display: flex;
  justify-content: center;
  gap: 25px;
  padding: 16px 20px;
  background: rgba(2, 6, 23, 0.95);
  backdrop-filter: blur(15px);
  border-bottom: 1px solid rgba(56,189,248,0.4);
}
.cosmic-tab {
  padding: 12px 26px;
  border-radius: 9999px;
  text-decoration: none;
  font-weight: 700;
  color: #7dd3fc;
  border: 1px solid rgba(125,211,252,0.5);
  transition: all 0.35s;
  font-size: 15.5px;
}
.cosmic-tab:hover {
  background: #0284c7;
  color: white;
  transform: translateY(-4px);
  box-shadow: 0 0 25px #38bdf8;
}

/* HERO - MAXIMUM SHINE & ATTRACTION */
.hero {
  text-align: center;
  padding: 160px 20px 120px;
  margin: 80px auto 70px;
  max-width: 1100px;
  border-radius: 28px;
  background: linear-gradient(145deg, #000428, #004e92);
  box-shadow: 
    0 0 90px rgba(56,189,248,0.7),
    inset 0 0 90px rgba(56,189,248,0.25);
  position: relative;
  overflow: hidden;
}
.hero::before {
  content: "";
  position: absolute;
  top: -150%;
  left: -150%;
  width: 400%;
  height: 400%;
  background: radial-gradient(circle, rgba(103,232,249,0.35) 0%, transparent 65%);
  animation: slowPulse 26s infinite ease-in-out;
}

/* ULTRA NEON TITLE - SUPER SHINING & ATTRACTIVE */
.herotitle {
  font-size: 96px;
  font-weight: 900;
  letter-spacing: 8px;
  color: #67e8f9;
  text-shadow: 
    0 0 15px #67e8f9,
    0 0 35px #38bdf8,
    0 0 70px #0284c7,
    0 0 110px #0369a1,
    0 0 160px #1e40af,
    0 0 220px #0e7490;
  line-height: 1.05;
  margin-bottom: 22px;
  animation: neonFlicker 3.5s infinite alternate;
}

/* SUBTITLE */
.subtitle {
  font-size: 29px;
  opacity: 0.97;
  margin-bottom: 45px;
  text-shadow: 0 0 20px rgba(103,232,249,0.7);
}

/* BIG BUTTONS */
.bigbtn {
  padding: 18px 40px;
  margin: 12px;
  border-radius: 9999px;
  background: linear-gradient(90deg, #0284c7, #22d3ee);
  color: white;
  text-decoration: none;
  font-weight: 700;
  font-size: 17px;
  display: inline-block;
  box-shadow: 0 12px 35px rgba(56,189,248,0.6);
  transition: all 0.4s;
}
.bigbtn:hover {
  transform: translateY(-8px) scale(1.06);
  box-shadow: 0 25px 50px rgba(56,189,248,0.8);
}

/* ANIMATIONS */
@keyframes neonFlicker {
  0%   { text-shadow: 0 0 15px #67e8f9, 0 0 35px #38bdf8, 0 0 70px #0284c7; }
  50%  { text-shadow: 0 0 25px #67e8f9, 0 0 55px #38bdf8, 0 0 100px #0284c7, 0 0 140px #0369a1; }
  100% { text-shadow: 0 0 15px #67e8f9, 0 0 35px #38bdf8, 0 0 70px #0284c7; }
}
@keyframes slowPulse {
  0%,100% { opacity: 0.65; transform: scale(0.92); }
  50%     { opacity: 1; transform: scale(1.08); }
}

/* YOUR ORIGINAL ROADMAP STYLES (kept exactly) */
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
</style>

<!-- FIXED ULTRA GLOWING TOP NAV -->
<div class="cosmic-top-nav">
  <a class="cosmic-tab" href="/table-of-content/">📖 Table of Contents</a>
  <a class="cosmic-tab" href="/contact/">📬 Contact</a>
  <a class="cosmic-tab" href="/support/">❤️ Support the Mission</a>
  <a class="cosmic-tab" href="/feedback/">💡 Feedback</a>
  <a class="cosmic-tab" href="/license/">⚖️ License</a>
</div>

<!-- HERO - NOW EXTREMELY SHINING & ATTRACTIVE -->
<div class="hero">
  <div class="herotitle">
    SCIENCE GENERALIZATION<br>HYPOTHESIS (SGH)
  </div>
  <div class="subtitle">
    A Foundational Ontological Framework for the Primordial Structure of Existence
  </div>
  <a href="/preface/" class="bigbtn">Start Free Materials</a>
  <a href="/paradoxes/" class="bigbtn">Solved Paradoxes</a>
  <a href="/support/" class="bigbtn">Support the Mission</a>
</div>

# 🌌 SGH Research Roadmap
<div class="roadmap">
  <div class="gen">
    ## PRIMARY — FREE ENTRY
    <a href="/preface/">Enter →</a>
  </div>
  <div class="arrow">↓</div>
  <div class="gen">
    ## FIRST GENERATION
    <a href="/first-gen/">Explore →</a>
  </div>
  <div class="arrow">↓</div>
  <div class="gen">
    ## SECOND GENERATION
    <a href="/second-gen/">Explore →</a>
  </div>
  <div class="arrow">↓</div>
  <div class="gen">
    ## THIRD GENERATION
    <a href="/third-gen/">Explore →</a>
  </div>
  <div class="arrow">↓</div>
  <div class="gen">
    ## FOURTH GENERATION
    <a href="/fourth-gen/">Explore →</a>
  </div>
  <div class="arrow">↓</div>
  <div class="gen">
    ## ULTIMATE
    <a href="/ultimate/">Explore →</a>
  </div>
</div>

---

⭐ Knowledge expands through structured discovery.
