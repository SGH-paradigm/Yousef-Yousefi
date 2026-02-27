---
layout: default
title: 🏠 Home
nav_order: 1
permalink: /
---

<style>

/* ===== GLOBAL ===== */

body {
  font-family: "Segoe UI", Roboto, Arial, sans-serif;
  color: #1e2a3a;
}

/* ===== SGH TITLE HERO ===== */

.hero {
  background: linear-gradient(135deg, #020024, #090979, #00d4ff);
  padding: 70px 20px;
  text-align: center;
  border-radius: 15px;
  color: white;
  margin-bottom: 30px;
  box-shadow: 0px 12px 30px rgba(0,0,0,.35);
}

.herotitle {
  font-size: 58px;
  font-weight: 800;
  letter-spacing: 2px;
  text-shadow: 0px 4px 12px rgba(0,0,0,.6);
  margin-bottom: 10px;
}

.subtitle {
  font-size: 22px;
  opacity: .95;
  margin-bottom: 25px;
}

/* ===== TOP NAVIGATION ===== */

.topnav {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 18px;
  margin-bottom: 35px;
}

.tab {
  padding: 12px 20px;
  border-radius: 25px;
  background: #e6f0ff;
  font-weight: 600;
  text-decoration: none;
  color: #004e92;
  box-shadow: 0px 3px 8px rgba(0,0,0,.2);
  transition: .3s;
  border: 1px solid transparent;
}

.tab:hover {
  background: #004e92;
  color: white;
  transform: translateY(-3px);
  border-color: #00aaff;
}

/* ===== BUTTONS ===== */

.bigbtn {
  padding: 14px 24px;
  background: #00aaff;
  border-radius: 8px;
  color: white;
  text-decoration: none;
  font-weight: bold;
  margin: 6px;
  display: inline-block;
  transition: .3s;
  border: 1px solid transparent;
}

.bigbtn:hover {
  background: #0085cc;
  border-color: white;
}

/* ===== PROFILE SIDEBAR & MAIN CONTENT LAYOUT ===== */
.content-wrapper {
  display: flex;
  gap: 30px;
  margin-top: 20px;
}

/* Sidebar styles */
.profile-sidebar {
  flex: 0 0 280px; /* fixed width on large screens */
  background: #f0f7ff;
  border-radius: 14px;
  padding: 25px 20px;
  box-shadow: 0px 4px 12px rgba(0,0,0,.2);
  border-left: 6px solid #00aaff;
  align-self: start; /* prevent stretching */
}

.profile-image {
  text-align: center;
  margin-bottom: 20px;
}

.profile-image img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid #00aaff;
  box-shadow: 0px 4px 10px rgba(0,0,0,.2);
}

.profile-name {
  font-size: 1.8rem;
  font-weight: bold;
  color: #004e92;
  text-align: center;
  margin-bottom: 5px;
  font-style: italic;
}

.profile-title {
  font-size: 1.1rem;
  text-align: center;
  color: #1e2a3a;
  margin-bottom: 20px;
  border-bottom: 1px dashed #00aaff;
  padding-bottom: 15px;
}

.profile-bio {
  font-size: 1rem;
  line-height: 1.6;
  color: #1e2a3a;
}

.profile-bio p {
  margin-bottom: 15px;
}

/* Main content area */
.main-content {
  flex: 1; /* take remaining space */
  min-width: 0; /* prevent overflow */
}

/* Responsive: stack on mobile */
@media (max-width: 768px) {
  .content-wrapper {
    flex-direction: column;
  }
  .profile-sidebar {
    flex: auto;
    width: 100%;
  }
}

/* ===== GENERATION CARDS ===== */

.gen {
  padding: 28px;
  background: #f7f9fc;
  border-radius: 14px;
  box-shadow: 0px 4px 12px rgba(0,0,0,.2);
  transition: .3s;
  margin-bottom: 20px;
  border-left: 6px solid #00aaff;
}

.gen:hover {
  transform: translateX(10px);
  background: #e3f0ff;
  border-left-color: #004e92;
}

.gen h2, .gen h3 {
  margin-top: 0;
  color: #004e92;
}

.gen h3 a {
  color: #004e92;
  text-decoration: none;
  border-bottom: 2px solid transparent;
  transition: .3s;
}

.gen h3 a:hover {
  border-bottom-color: #00aaff;
}

.gen ul {
  margin-bottom: 0;
  padding-left: 20px;
  color: #1e2a3a;
}

.gen li {
  margin-bottom: 4px;
}

/* ===== ADDITIONAL SECTIONS ===== */

.pioneer, .news, .contact {
  margin-top: 40px;
  padding: 20px;
  background: #f0f7ff;
  border-radius: 12px;
  box-shadow: 0px 3px 10px rgba(0,0,0,.18);
  border-left: 6px solid #00aaff;
}

.pioneer h2, .news h2, .contact h2 {
  color: #004e92;
}

.pioneer a, .news a, .contact a {
  color: #004e92;
  font-weight: 600;
  text-decoration: none;
  border-bottom: 1px dotted #00aaff;
}

.pioneer a:hover, .news a:hover, .contact a:hover {
  color: #00aaff;
  border-bottom-style: solid;
}

blockquote {
  background: white;
  padding: 15px;
  border-radius: 8px;
  border-left: 4px solid #00aaff;
  margin: 0;
  color: #1e2a3a;
}

hr {
  border: none;
  height: 2px;
  background: linear-gradient(90deg, transparent, #00aaff, transparent);
  margin: 30px 0;
}

</style>

<!-- HERO SECTION -->
<div class="hero">
  <div class="herotitle">Science Generalization Hypothesis (SGH)</div>
  <div class="subtitle">Toward a Unified Ontology of Reality<br>Ontology • Mathematics • Physics • Consciousness</div>
  <a href="/preface/" class="bigbtn" target="_blank">Start Free Materials</a>
  <a href="/paradoxes/" class="bigbtn" target="_blank">Solved Paradoxes</a>
  <a href="/support/" class="bigbtn" target="_blank">Support Mission</a>
</div>

<!-- TOP NAVIGATION -->
<div class="topnav">
  <a class="tab" href="/table-of-content/" target="_blank">📚 Table of Contents</a>
  <a class="tab" href="/contact/" target="_blank">📬 Contact</a>
  <a class="tab" href="/support/" target="_blank">❤️ Support the Mission</a>
  <a class="tab" href="/feedback/" target="_blank">💡 Feedback</a>
  <a class="tab" href="/license/" target="_blank">⚖️ License</a>
</div>

<!-- PROFILE SIDEBAR + MAIN CONTENT -->
<div class="content-wrapper">
  <!-- LEFT SIDEBAR: Author profile -->
  <aside class="profile-sidebar">
    <div class="profile-image">
      <!-- Replace with your actual image path -->
      <img src="/assets/images/profile.jpg" alt="Yousef Yousefi">
    </div>
    <div class="profile-name">Yousef Yousefi</div>
    <div class="profile-title">Independent Researcher</div>
    <div class="profile-bio">
      <p>I am a theorist and lifelong explorer of the universe's deep structures, working at the intersection of philosophy, mathematics, and physics.</p>
      <p>My Science Generalization Hypothesis (SGH) offers a foundational ontological framework for the primordial structure of existence, unifying abstract and concrete reality.</p>
      <p>📍 Contact: <a href="mailto:yousefyousefi191@gmail.com">yousefyousefi191@gmail.com</a></p>
    </div>
  </aside>

  <!-- MAIN CONTENT: Research catalog -->
  <main class="main-content">
    <h1>📚 Complete Research Catalog</h1>
    <p>Click on any generation heading to access its overview page. Detailed contents are listed below each heading for reference.</p>

    <!-- GENERATION CARDS (DETAILED LISTS) -->
    <div class="gen">
      <h3><a href="/primary/" target="_blank">primery</a></h3>
      <ul>
        <li>preface</li>
        <li>introduction</li>
      </ul>
    </div>

    <!-- Pre-SGH genration -->
    <div class="gen">
      <h3><a href="/pre-sgh/" target="_blank">Pre-SGH genration</a></h3>
      <ul>
        <li>introduction</li>
        <li>Chapter 1: Constraint-Induced Concentration in High-Dimensional Function Spaces:<br>Geometric Regularities and Entropy Maximization</li>
        <li>Chapter 2: Empirical Clustering Patterns in Binary Partition Ratios of<br>Parametric Functions: A Large-Scale Computational Study</li>
        <li>Chapter 3: Attractor Networks via Constraint-Induced Concentration<br>in High-Dimensional Function Spaces</li>
        <li>Chapter 4: Quantum Partition Ratios: Born-Rule Observables<br>for Wavefunction Nodal Asymmetry, Eigenstate Geometry, and Experimental Signatures</li>
        <li>Chapter 5: Constraint-Induced Necessity:<br>A Philosophical Framework for Contextual Mathematical Structures</li>
        <li>Chapter 6: Partition Ratios Across Mathematical and Physical Systems:<br>A Comprehensive Review and Cross-Disciplinary Synthesis</li>
        <li>conclusion</li>
      </ul>
    </div>

    <div class="gen">
      <h3><a href="/first-gen/" target="_blank">first SGH genration</a></h3>
      <ul>
        <li>introduction</li>
        <li>Chapter 1: Foundations of SGH</li>
        <li>Chapter 2: The Creation Mechanism</li>
        <li>Chapter 3: Unified Classification</li>
        <li>Chapter 4: Mathematical Formalization</li>
        <li>Chapter 5: Physics Applications & Roadmap</li>
        <li>Chapter 6: Philosophical Implications</li>
        <li>Chapter 7: Research Roadmap</li>
        <li>solved paradox</li>
      </ul>
    </div>

    <div class="gen">
      <h3><a href="/second-gen/" target="_blank">Second genration</a></h3>
      <ul>
        <li>Sience Genralization Hypothese road map toward unification intoduction:<br>Toward Uinification</li>
        <li>SGH-Matematics Recounstrction : <br>A-1-1:</li>
        <li>SGH-Matematics Recounstrction :<br>A-1-2:</li>
        <li>SGH-Matematics Recounstrction :<br>A-2-1:</li>
        <li>SGH-Matematics Recounstrction :<br>A-2-2:</li>
        <li>SGH-Physics Recounstrction :<br>B-1-1:</li>
        <li>SGH-Physics Recounstrction :<br>B-1-2:</li>
        <li>SGH-Physics Recounstrction : : <br>B-2-1:</li>
        <li>SGH-Physics Recounstrction :<br>B-2-2:</li>
        <li>Conclusion</li>
        <li>solved paradox</li>
        <li>Resut 1</li>
        <li>Resut 2</li>
        <li>Resut 3</li>
        <li>Resut 4</li>
        <li>Resut 5</li>
        <li>Resut 6</li>
        <li>Resut 7</li>
        <li>Resut 8</li>
      </ul>
    </div>

    <div class="gen">
      <h3><a href="/third-gen/" target="_blank">Tird Genration</a></h3>
      <ul>
        <li>toward Genralization and Unification</li>
        <li>Triadic</li>
        <li>chapter 1 :A Foundational Ontological Framework for the Primordial Structure of Existence</li>
        <li>chapter 2: Chapter 2: Existence Creation<br>The Mechanism by Which Existence Comes to Be</li>
        <li>chapter 3: Science Generalization Hypothesis (SGH): A Unified Framework- clasification</li>
        <li>implication chapter 3</li>
        <li>felisiblity</li>
        <li>future work</li>
        <li>solved paradox</li>
        <li>result 1</li>
        <li>result 2</li>
        <li>result 3</li>
        <li>result 4</li>
        <li>result 5</li>
        <li>result 6</li>
        <li>result 7</li>
        <li>result 8</li>
        <li>result 9</li>
        <li>result 10</li>
        <li>result 11</li>
        <li>result 12</li>
        <li>result 13</li>
        <li>result 14</li>
        <li>result 15</li>
        <li>paradox</li>
        <li>paradox</li>
      </ul>
    </div>

    <div class="gen">
      <h3><a href="/fourth-gen/" target="_blank">forth genration</a></h3>
      <ul>
        <li>paradox</li>
        <li>Octactan SGH</li>
        <li>genralization</li>
        <li>paradox</li>
        <li>paradox</li>
        <li>paradox</li>
        <li>implication chapter 3</li>
        <li>implication chapter 3</li>
        <li>implication chapter 3</li>
        <li>implication chapter 3</li>
        <li>solved paradox</li>
        <li>unification</li>
        <li>future work</li>
        <li>toward galaxitizen</li>
      </ul>
    </div>
  </main>
</div>

<!-- PIONEER SECTION -->
<div class="pioneer">
  <h2>🚀 Pioneer & Speculative Frontiers</h2>
  <p>Based on the Science Generalization Hypothesis, I explore visionary possibilities that could reshape humanity’s future. These ideas are speculative today, but they illustrate the power of the framework:</p>
  <ul>
    <li><strong>Interstellar Travel:</strong> How manipulating the reality parameter χ might enable new propulsion methods and even access to other dimensions.</li>
    <li><strong>Medical Revolutions:</strong> Potential applications in cellular repair, reversing entropy, and understanding consciousness.</li>
    <li><strong>Next‑Gen Discovery Tools:</strong> Detectors sensitive to χ‑transitions and experiments to reveal hidden structures in the cosmos.</li>
    <li><strong>Toward “UFO” Technology:</strong> Engineering gravity and inertia by locally shifting χ – a path to revolutionary vehicles.</li>
  </ul>
  <p>👉 <a href="/pioneer/" target="_blank">Read More</a></p>
</div>

<!-- LATEST NEWS -->
<div class="news">
  <h2>📢 Latest News</h2>
  <blockquote>
    📜 My official papers are being simultaneously submitted to:<br>
    - <a href="https://arxiv.org" target="_blank">arXiv.org</a><br>
    - <a href="https://www.researchgate.net/profile/Yousef-Yousefi-7" target="_blank">ResearchGate</a><br>
    - <a href="https://sgh-paradigm.github.io/Yousef-Yousefi/" target="_blank">This Website</a>
  </blockquote>
  <p>Stay tuned for updates and new breakthroughs!</p>
</div>

<!-- GET IN TOUCH -->
<div class="contact">
  <h2>📬 Get in Touch</h2>
  <p>Feel free to reach out for discussions, collaborations, or questions.<br>
  You can find all contact options on the <a href="/contact/" target="_blank">Contact</a> page.</p>
</div>

<hr>

<p style="text-align:center;">⭐ <em>Knowledge grows by sharing and expanding ideas.</em> ⭐</p>
