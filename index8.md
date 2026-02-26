---
layout: default
title: SGH
nav_order: 1
permalink: /
---

<style>
/* ================================
ULTRA COSMIC BACKGROUND + GLOBAL
================================ */
body {
  background: 
    radial-gradient(circle at 15% 25%, #0a2a6b 0%, transparent 45%),
    radial-gradient(circle at 85% 15%, #001f54 0%, transparent 50%),
    radial-gradient(circle at 50% 85%, #002b5b 0%, transparent 55%),
    #020617;
  color: #e6edf3;
  font-family: 'Segoe UI', Roboto, Arial, sans-serif;
}

/* HEADER - CLEAN & GLOWING */
.site-header {
  background: rgba(2,6,23,0.85) !important;
  backdrop-filter: blur(12px);
  border-bottom: 1px solid rgba(56,189,248,0.3) !important;
  box-shadow: 0 4px 30px rgba(56,189,248,0.25) !important;
}
.site-title {
  font-size: 28px !important;
  font-weight: 900 !important;
  letter-spacing: 2px;
  color: #7dd3fc !important;
  text-shadow: 0 0 15px #38bdf8;
}

/* TOP NAV - FIXED & GLOWING */
.cosmic-top-nav {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000;
  display: flex;
  justify-content: center;
  gap: 18px;
  padding: 14px 20px;
  background: rgba(2,6,23,0.92);
  backdrop-filter: blur(15px);
  border-bottom: 1px solid rgba(56,189,248,0.4);
}
.cosmic-tab {
  padding: 10px 22px;
  border-radius: 9999px;
  text-decoration: none;
  font-weight: 700;
  color: #7dd3fc;
  border: 1px solid rgba(125,211,252,0.5);
  transition: all 0.35s;
  font-size: 15px;
}
.cosmic-tab:hover {
  background: #0284c7;
  color: white;
  transform: translateY(-3px);
  box-shadow: 0 0 25px #38bdf8;
}

/* HERO - MAXIMUM SHINE */
.hero {
  text-align: center;
  padding: 140px 20px 110px;
  margin: 80px auto 80px;
  max-width: 1100px;
  border-radius: 24px;
  background: linear-gradient(145deg, #000428, #004e92);
  box-shadow: 
    0 0 80px rgba(56,189,248,0.6),
    inset 0 0 80px rgba(56,189,248,0.2);
  position: relative;
  overflow: hidden;
}
.hero::before {
  content: "";
  position: absolute;
  top: -100%;
  left: -100%;
  width: 300%;
  height: 300%;
  background: radial-gradient(circle, rgba(125,211,252,0.25) 0%, transparent 70%);
  animation: slowPulse 28s infinite ease-in-out;
}

/* ULTRA NEON TITLE - SUPER SHINING */
.herotitle {
  font-size: 92px;
  font-weight: 900;
  letter-spacing: 6px;
  color: #67e8f9;
  text-shadow: 
    0 0 10px #67e8f9,
    0 0 25px #38bdf8,
    0 0 50px #0284c7,
    0 0 90px #0369a1,
    0 0 130px #1e40af,
    0 0 180px #0e7490;
  line-height: 1.05;
  margin-bottom: 20px;
  animation: neonFlicker 4s infinite alternate;
}

/* SUBTITLE */
.subtitle {
  font-size: 28px;
  opacity: 0.98;
  margin-bottom: 40px;
  text-shadow: 0 0 15px rgba(103,232,249,0.6);
}

/* BUTTONS */
.bigbtn {
  padding: 18px 38px;
  margin: 12px;
  border-radius: 9999px;
  background: linear-gradient(90deg, #0284c7, #22d3ee);
  color: white;
  text-decoration: none;
  font-weight: 700;
  font-size: 17px;
  display: inline-block;
  box-shadow: 0 10px 30px rgba(56,189,248,0.5);
  transition: all 0.4s;
}
.bigbtn:hover {
  transform: translateY(-8px) scale(1.05);
  box-shadow: 0 20px 40px rgba(56,189,248,0.7);
}

/* ANIMATIONS */
@keyframes neonFlicker {
  0%   { text-shadow: 0 0 10px #67e8f9, 0 0 25px #38bdf8, 0 0 50px #0284c7; }
  50%  { text-shadow: 0 0 15px #67e8f9, 0 0 40px #38bdf8, 0 0 80px #0284c7, 0 0 120px #0369a1; }
  100% { text-shadow: 0 0 10px #67e8f9, 0 0 25px #38bdf8, 0 0 50px #0284c7; }
}
@keyframes slowPulse {
  0%,100% { opacity: 0.6; transform: scale(0.95); }
  50%     { opacity: 1; transform: scale(1.05); }
}

/* ROADMAP (unchanged but cleaner) */
.roadmap { ... } /* keep your previous roadmap styles or use the one from last version */
</style>

<!-- FIXED TOP NAV -->
<div class="cosmic-top-nav">
  <a class="cosmic-tab" href="/table-of-content/">📖 Table of Contents</a>
  <a class="cosmic-tab" href="/contact/">📬 Contact</a>
  <a class="cosmic-tab" href="/support/">❤️ Support</a>
  <a class="cosmic-tab" href="/feedback/">💡 Feedback</a>
  <a class="cosmic-tab" href="/license/">⚖️ License</a>
</div>

<!-- HERO - NOW EXTREMELY SHINING -->
<div class="hero">
  <div class="herotitle">
    SCIENCE GENERALIZATION<br>HYPOTHESIS (SGH)
  </div>
  <div class="subtitle">
    A Foundational Ontological Framework for the Primordial Structure of Existence
  </div>
  <a href="/preface/" class="bigbtn">Start Free Materials</a>
  <a href="/first-gen/" class="bigbtn">Buy First Generation</a>
  <a href="/paradoxes/" class="bigbtn">Solved Paradoxes</a>
</div>

<!-- REST OF YOUR CONTENT (roadmap, paradoxes, etc.) remains exactly as before -->
