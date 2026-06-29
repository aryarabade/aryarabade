<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Arya Rabade — GitHub Profile</title>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;600&family=Inter:wght@300;400;500;600;700;900&display=swap" rel="stylesheet"/>
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { background: #0d1117; }

  .profile-wrap {
    font-family: 'Inter', sans-serif;
    background: #0d1117;
    color: #e6edf3;
    max-width: 900px;
    margin: 0 auto;
    border-radius: 16px;
    overflow: hidden;
  }

  /* ---- HERO ---- */
  .hero {
    position: relative;
    padding: 3rem 2rem 2rem;
    text-align: center;
    background: linear-gradient(160deg, #0d1117 0%, #161b22 50%, #0d1117 100%);
    overflow: hidden;
  }
  .hero-canvas { position: absolute; inset: 0; pointer-events: none; }

  .avatar-ring {
    width: 96px; height: 96px;
    border-radius: 50%;
    background: linear-gradient(135deg, #7c3aed, #a78bfa, #38bdf8);
    padding: 3px;
    margin: 0 auto 1rem;
    position: relative; z-index: 2;
    animation: spin-ring 8s linear infinite;
  }
  @keyframes spin-ring {
    from { filter: hue-rotate(0deg); }
    to   { filter: hue-rotate(360deg); }
  }
  .avatar-inner {
    width: 100%; height: 100%;
    border-radius: 50%;
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    display: flex; align-items: center; justify-content: center;
    font-size: 2.4rem; font-weight: 700; color: #a78bfa;
  }

  .hero h1 {
    font-size: 2rem; font-weight: 800;
    background: linear-gradient(90deg, #a78bfa, #38bdf8, #a78bfa);
    background-size: 200%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: shimmer 3s linear infinite;
    position: relative; z-index: 2; margin-bottom: .25rem;
  }
  @keyframes shimmer {
    from { background-position: 0% 50%; }
    to   { background-position: 200% 50%; }
  }

  .hero-sub {
    font-size: .9rem; color: #8b949e;
    font-family: 'Fira Code', monospace;
    position: relative; z-index: 2; margin-bottom: 1.2rem;
  }
  .typing-line {
    font-family: 'Fira Code', monospace;
    font-size: .85rem; color: #a78bfa;
    position: relative; z-index: 2;
  }
  .typing-cursor {
    display: inline-block; width: 2px; height: 1em;
    background: #a78bfa;
    animation: blink .7s step-end infinite;
    vertical-align: middle; margin-left: 2px;
  }
  @keyframes blink { 50% { opacity: 0; } }

  .badges-row {
    display: flex; flex-wrap: wrap; gap: 8px;
    justify-content: center;
    position: relative; z-index: 2; margin-top: 1rem;
  }
  .badge {
    font-size: .75rem; font-weight: 600; letter-spacing: .04em;
    padding: 4px 12px; border-radius: 20px;
    font-family: 'Fira Code', monospace;
  }
  .badge-purple { background: #2d1b69; color: #c4b5fd; border: 1px solid #7c3aed; }
  .badge-blue   { background: #0c2d4d; color: #7dd3fc; border: 1px solid #0ea5e9; }
  .badge-green  { background: #0d2d1a; color: #6ee7b7; border: 1px solid #10b981; }
  .badge-orange { background: #2d1500; color: #fdba74; border: 1px solid #f97316; }

  /* ---- WAVE ---- */
  .wave-svg { display: block; width: 100%; height: 60px; margin-top: -2px; }

  /* ---- SECTION ---- */
  .section { padding: 1.5rem 2rem; }
  .section-title {
    font-size: .7rem; font-weight: 700; letter-spacing: .12em;
    color: #7c3aed; text-transform: uppercase;
    font-family: 'Fira Code', monospace;
    display: flex; align-items: center; gap: 8px; margin-bottom: 1rem;
  }
  .section-title::after {
    content: ''; flex: 1; height: 1px;
    background: linear-gradient(to right, #7c3aed33, transparent);
  }

  /* ---- STATS ---- */
  .stats-row { display: grid; grid-template-columns: repeat(3, 1fr); gap: 12px; margin-bottom: 1.5rem; }
  .stat-card {
    background: #161b22; border: 1px solid #30363d;
    border-radius: 12px; padding: 1rem; text-align: center;
    transition: border-color .2s, transform .2s; cursor: default;
  }
  .stat-card:hover { border-color: #7c3aed; transform: translateY(-3px); }
  .stat-num {
    font-size: 1.6rem; font-weight: 800;
    background: linear-gradient(135deg, #a78bfa, #38bdf8);
    -webkit-background-clip: text; -webkit-text-fill-color: transparent;
  }
  .stat-label { font-size: .72rem; color: #8b949e; margin-top: 2px; }

  /* ---- TECH ---- */
  .tech-grid { display: flex; flex-wrap: wrap; gap: 8px; }
  .tech-chip {
    font-size: .75rem; font-weight: 600;
    padding: 5px 12px; border-radius: 6px;
    font-family: 'Fira Code', monospace; border: 1px solid;
    transition: transform .15s, box-shadow .15s;
  }
  .tech-chip:hover { transform: translateY(-2px); box-shadow: 0 4px 12px rgba(124,58,237,.3); }
  .tc-js   { background: #1a1500; color: #fbbf24; border-color: #78350f; }
  .tc-java { background: #1a0a00; color: #f97316; border-color: #7c2d12; }
  .tc-react{ background: #001a25; color: #38bdf8; border-color: #0c4a6e; }
  .tc-node { background: #001a0a; color: #4ade80; border-color: #14532d; }
  .tc-mongo{ background: #001a0a; color: #6ee7b7; border-color: #065f46; }
  .tc-cpp  { background: #00051a; color: #818cf8; border-color: #1e3a5f; }
  .tc-html { background: #1a0800; color: #fb923c; border-color: #7c2d12; }
  .tc-css  { background: #00051a; color: #60a5fa; border-color: #1e40af; }
  .tc-git  { background: #1a0000; color: #f87171; border-color: #7f1d1d; }
  .tc-ex   { background: #0a0a0a; color: #d1d5db; border-color: #374151; }
  .tc-mysql{ background: #00051a; color: #60a5fa; border-color: #1e40af; }
  .tc-dsa  { background: #1a0000; color: #f87171; border-color: #991b1b; }

  /* ---- SKILL BARS ---- */
  .skill-row { margin-bottom: .6rem; }
  .skill-info { display: flex; justify-content: space-between; margin-bottom: 3px; }
  .skill-name { font-size: .75rem; color: #c9d1d9; font-family: 'Fira Code', monospace; }
  .skill-pct  { font-size: .72rem; color: #7c3aed; }
  .skill-track { background: #21262d; border-radius: 4px; height: 6px; overflow: hidden; }
  .skill-fill {
    height: 100%; border-radius: 4px;
    background: linear-gradient(90deg, #7c3aed, #38bdf8);
    animation: fill-bar 1s ease-out both;
  }
  @keyframes fill-bar { from { width: 0 !important; } }

  /* ---- PROJECTS ---- */
  .projects-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
  .project-card {
    background: #161b22; border: 1px solid #30363d;
    border-radius: 12px; padding: 1.1rem;
    transition: border-color .2s, transform .2s;
    position: relative; overflow: hidden;
  }
  .project-card::before {
    content: ''; position: absolute; top: 0; left: 0; right: 0; height: 2px;
    background: linear-gradient(90deg, #7c3aed, #38bdf8);
    opacity: 0; transition: opacity .2s;
  }
  .project-card:hover { border-color: #7c3aed; transform: translateY(-3px); }
  .project-card:hover::before { opacity: 1; }
  .proj-title { font-size: .9rem; font-weight: 700; color: #e6edf3; margin-bottom: .3rem; }
  .proj-desc  { font-size: .75rem; color: #8b949e; line-height: 1.5; margin-bottom: .7rem; }
  .proj-tags  { display: flex; flex-wrap: wrap; gap: 4px; }
  .proj-tag {
    font-size: .65rem; padding: 2px 8px; border-radius: 4px;
    background: #2d1b69; color: #c4b5fd;
    font-family: 'Fira Code', monospace;
  }
  .proj-impact { font-size: .7rem; color: #4ade80; margin-top: .6rem; font-family: 'Fira Code', monospace; }

  /* ---- ACTIVITY BAR ---- */
  .activity-bar { display: flex; align-items: flex-end; gap: 3px; height: 48px; margin-top: .5rem; }
  .ab-col { flex: 1; border-radius: 2px; animation: grow-bar .6s ease-out both; }
  @keyframes grow-bar {
    from { transform: scaleY(0); transform-origin: bottom; }
    to   { transform: scaleY(1); transform-origin: bottom; }
  }

  /* ---- LEETCODE ---- */
  .lc-card { background: #161b22; border: 1px solid #30363d; border-radius: 12px; padding: 1.2rem; }
  .lc-header { display: flex; align-items: center; gap: 10px; margin-bottom: 1rem; }
  .lc-logo {
    font-size: 1.2rem; font-weight: 800;
    background: linear-gradient(135deg, #ffa116, #ffca2c);
    -webkit-background-clip: text; -webkit-text-fill-color: transparent;
    font-family: 'Fira Code', monospace;
  }
  .lc-user { font-size: .8rem; color: #8b949e; font-family: 'Fira Code', monospace; }
  .lc-stats { display: grid; grid-template-columns: repeat(3, 1fr); gap: 10px; }
  .lc-stat { text-align: center; padding: .6rem; border-radius: 8px; border: 1px solid #30363d; }
  .lc-stat-num { font-size: 1.3rem; font-weight: 800; }
  .lc-stat-label { font-size: .65rem; color: #8b949e; margin-top: 2px; }
  .lc-easy   { color: #4ade80; }
  .lc-medium { color: #fbbf24; }
  .lc-hard   { color: #f87171; }

  /* ---- CONTACT ---- */
  .contact-section {
    background: linear-gradient(135deg, #0d1117 0%, #1a0a2e 50%, #0d1117 100%);
    padding: 2rem; position: relative; overflow: hidden;
  }
  .contact-section::before {
    content: ''; position: absolute; inset: 0;
    background: radial-gradient(ellipse at 50% 0%, #7c3aed22 0%, transparent 70%);
    pointer-events: none;
  }
  .contact-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; }
  .contact-card {
    background: #161b22; border: 1px solid #30363d;
    border-radius: 12px; padding: 1rem;
    display: flex; align-items: center; gap: 12px;
    transition: border-color .2s, transform .2s, box-shadow .2s;
    cursor: pointer; text-decoration: none; color: inherit;
  }
  .contact-card:hover { transform: translateY(-3px); box-shadow: 0 8px 24px rgba(124,58,237,.2); }
  .cc-email:hover    { border-color: #ef4444; }
  .cc-linkedin:hover { border-color: #0ea5e9; }
  .cc-lc:hover       { border-color: #ffa116; }
  .cc-phone:hover    { border-color: #4ade80; }
  .cc-port:hover     { border-color: #a78bfa; }
  .cc-icon {
    width: 38px; height: 38px; border-radius: 10px;
    display: flex; align-items: center; justify-content: center;
    font-size: 1.1rem; flex-shrink: 0;
  }
  .icon-email    { background: #1a0000; }
  .icon-linkedin { background: #001020; }
  .icon-lc       { background: #1a0d00; }
  .icon-phone    { background: #001a0a; }
  .icon-port     { background: #140020; }
  .cc-text { flex: 1; }
  .cc-name { font-size: .8rem; font-weight: 600; color: #e6edf3; }
  .cc-val  { font-size: .72rem; color: #8b949e; font-family: 'Fira Code', monospace; margin-top: 1px; }
  .cc-arrow { font-size: .8rem; color: #30363d; transition: color .2s, transform .2s; }
  .contact-card:hover .cc-arrow { color: #a78bfa; transform: translateX(3px); }

  /* ---- QUOTE ---- */
  .quote-section { padding: 1.5rem 2rem; border-top: 1px solid #21262d; text-align: center; background: #0d1117; }
  .quote-text {
    font-family: 'Fira Code', monospace; font-size: .82rem;
    color: #8b949e; font-style: italic; position: relative; padding: 0 1.5rem;
  }
  .quote-text::before { content: '\201C'; position: absolute; left: 0; top: -4px; font-size: 1.5rem; color: #7c3aed; font-style: normal; }
  .quote-text::after  { content: '\201D'; position: absolute; right: 0; top: -4px; font-size: 1.5rem; color: #7c3aed; font-style: normal; }
  .footer-row { display: flex; justify-content: center; gap: 8px; flex-wrap: wrap; margin-top: 1rem; }
  .footer-badge { font-size: .7rem; padding: 3px 10px; border-radius: 12px; font-weight: 600; letter-spacing: .05em; }
</style>
</head>
<body>

<div class="profile-wrap">

  <!-- HERO -->
  <div class="hero">
    <canvas class="hero-canvas" id="heroCanvas"></canvas>
    <div class="avatar-ring">
      <div class="avatar-inner">AR</div>
    </div>
    <h1>Arya Rabade</h1>
    <div class="hero-sub">B.Tech CSE · Kolhapur · CGPA 8.0</div>
    <div class="typing-line" id="typingLine">Full Stack MERN Developer<span class="typing-cursor"></span></div>
    <div class="badges-row">
      <span class="badge badge-purple">🚀 MERN Stack</span>
      <span class="badge badge-orange">☕ Java Enthusiast</span>
      <span class="badge badge-blue">🧠 DSA Learner</span>
      <span class="badge badge-green">🌱 Always Building</span>
    </div>
  </div>

  <!-- WAVE 1 -->
  <svg class="wave-svg" viewBox="0 0 1440 60" preserveAspectRatio="none" style="background:#0d1117;">
    <path d="M0,30 C240,60 480,0 720,30 C960,60 1200,0 1440,30 L1440,60 L0,60 Z" fill="#161b22"/>
  </svg>

  <!-- GITHUB STATS -->
  <div class="section" style="background:#161b22;">
    <div class="section-title">// github stats</div>
    <div class="stats-row">
      <div class="stat-card"><div class="stat-num">8.0</div><div class="stat-label">CGPA</div></div>
      <div class="stat-card"><div class="stat-num">3+</div><div class="stat-label">Projects</div></div>
      <div class="stat-card"><div class="stat-num">5+</div><div class="stat-label">Technologies</div></div>
    </div>
    <div style="background:#0d1117;border:1px solid #30363d;border-radius:10px;padding:1rem;">
      <div style="font-size:.7rem;color:#8b949e;font-family:'Fira Code',monospace;margin-bottom:.5rem;">contribution activity</div>
      <div class="activity-bar" id="activityBar"></div>
    </div>
  </div>

  <!-- WAVE 2 -->
  <svg class="wave-svg" viewBox="0 0 1440 60" preserveAspectRatio="none" style="background:#161b22;">
    <path d="M0,20 C360,60 720,0 1080,30 C1260,50 1380,10 1440,20 L1440,60 L0,60 Z" fill="#0d1117"/>
  </svg>

  <!-- TECH STACK -->
  <div class="section">
    <div class="section-title">// tech stack</div>
    <div class="tech-grid" style="margin-bottom:1.2rem;">
      <span class="tech-chip tc-html">HTML5</span>
      <span class="tech-chip tc-css">CSS3</span>
      <span class="tech-chip tc-js">JavaScript</span>
      <span class="tech-chip tc-java">Java</span>
      <span class="tech-chip tc-react">React</span>
      <span class="tech-chip tc-node">Node.js</span>
      <span class="tech-chip tc-ex">Express.js</span>
      <span class="tech-chip tc-mongo">MongoDB</span>
      <span class="tech-chip tc-mysql">MySQL</span>
      <span class="tech-chip tc-cpp">C++</span>
      <span class="tech-chip tc-git">Git / GitHub</span>
      <span class="tech-chip tc-dsa">DSA</span>
    </div>
    <div class="section-title">// proficiency</div>
    <div class="skill-row"><div class="skill-info"><span class="skill-name">MERN Stack</span><span class="skill-pct">82%</span></div><div class="skill-track"><div class="skill-fill" style="width:82%"></div></div></div>
    <div class="skill-row"><div class="skill-info"><span class="skill-name">Java & OOP</span><span class="skill-pct">78%</span></div><div class="skill-track"><div class="skill-fill" style="width:78%"></div></div></div>
    <div class="skill-row"><div class="skill-info"><span class="skill-name">DSA / Algorithms</span><span class="skill-pct">70%</span></div><div class="skill-track"><div class="skill-fill" style="width:70%"></div></div></div>
    <div class="skill-row"><div class="skill-info"><span class="skill-name">Database (Mongo/SQL)</span><span class="skill-pct">75%</span></div><div class="skill-track"><div class="skill-fill" style="width:75%"></div></div></div>
  </div>

  <!-- WAVE 3 -->
  <svg class="wave-svg" viewBox="0 0 1440 60" preserveAspectRatio="none" style="background:#0d1117;">
    <path d="M0,40 C300,0 600,60 900,20 C1100,0 1300,50 1440,40 L1440,60 L0,60 Z" fill="#161b22"/>
  </svg>

  <!-- PROJECTS -->
  <div class="section" style="background:#161b22;">
    <div class="section-title">// featured projects</div>
    <div class="projects-grid">
      <div class="project-card">
        <div class="proj-title">💊 Medicare Store Portal</div>
        <div class="proj-desc">Medicine inventory system with live stock updates, smart alerts & pharmacy analytics.</div>
        <div class="proj-tags">
          <span class="proj-tag">Express.js</span>
          <span class="proj-tag">MongoDB</span>
          <span class="proj-tag">MSSQL</span>
        </div>
        <div class="proj-impact">→ Prevents expired medicine waste</div>
      </div>
      <div class="project-card">
        <div class="proj-title">✅ Smart Habit Tracker</div>
        <div class="proj-desc">Habit-building app with streaks, reminders, and visual progress analytics.</div>
        <div class="proj-tags">
          <span class="proj-tag">React</span>
          <span class="proj-tag">Node.js</span>
          <span class="proj-tag">MongoDB</span>
        </div>
        <div class="proj-impact">→ Drives goal consistency</div>
      </div>
      <div class="project-card" style="grid-column: 1 / -1;">
        <div class="proj-title">💰 AI Finance Tracker</div>
        <div class="proj-desc">AI-powered dashboard that auto-categorizes spending and delivers smart budgeting insights via MERN stack with OpenAI integration.</div>
        <div class="proj-tags">
          <span class="proj-tag">MERN</span>
          <span class="proj-tag">AI Powered</span>
          <span class="proj-tag">MongoDB</span>
          <span class="proj-tag">OpenAI</span>
        </div>
        <div class="proj-impact">→ Data-driven money management</div>
      </div>
    </div>
  </div>

  <!-- WAVE 4 -->
  <svg class="wave-svg" viewBox="0 0 1440 60" preserveAspectRatio="none" style="background:#161b22;">
    <path d="M0,10 C200,50 500,0 800,35 C1000,55 1200,10 1440,25 L1440,60 L0,60 Z" fill="#0d1117"/>
  </svg>

  <!-- LEETCODE -->
  <div class="section">
    <div class="section-title">// leetcode · arya1624</div>
    <div class="lc-card">
      <div class="lc-header">
        <div>
          <div class="lc-logo">LeetCode</div>
          <div class="lc-user">@arya1624 · Active Problem Solver</div>
        </div>
        <div style="margin-left:auto;font-size:1.4rem;animation:spin-ring 4s linear infinite;">🔥</div>
      </div>
      <div class="lc-stats">
        <div class="lc-stat" style="background:#001a0a;border-color:#14532d;">
          <div class="lc-stat-num lc-easy" id="lcEasy">0</div>
          <div class="lc-stat-label" style="color:#4ade80;">Easy</div>
        </div>
        <div class="lc-stat" style="background:#1a0d00;border-color:#78350f;">
          <div class="lc-stat-num lc-medium" id="lcMed">0</div>
          <div class="lc-stat-label" style="color:#fbbf24;">Medium</div>
        </div>
        <div class="lc-stat" style="background:#1a0000;border-color:#7f1d1d;">
          <div class="lc-stat-num lc-hard" id="lcHard">0</div>
          <div class="lc-stat-label" style="color:#f87171;">Hard</div>
        </div>
      </div>
      <div style="margin-top:.8rem;padding:.6rem;background:#0d1117;border-radius:8px;font-family:'Fira Code',monospace;font-size:.72rem;color:#8b949e;">
        <span style="color:#4ade80;">const</span> arya = { profile: <span style="color:#fbbf24;"><a href="https://leetcode.com/u/arya1624/" target="_blank" style="color:#fbbf24;text-decoration:none;">"leetcode.com/u/arya1624"</a></span>, focus: <span style="color:#a78bfa;">"DSA Mastery"</span> };
      </div>
    </div>
  </div>

  <!-- WAVE 5 -->
  <svg class="wave-svg" viewBox="0 0 1440 60" preserveAspectRatio="none" style="background:#0d1117;">
    <path d="M0,30 C180,0 360,60 720,25 C900,10 1200,55 1440,30 L1440,60 L0,60 Z" fill="#1a0a2e"/>
  </svg>

  <!-- CONTACT -->
  <div class="contact-section">
    <div class="section-title" style="color:#a78bfa;">// let's connect</div>
    <div style="font-size:.82rem;color:#8b949e;margin-bottom:1.2rem;font-family:'Fira Code',monospace;">
      Open to internships, collaborations &amp; cool projects ✨
    </div>
    <div class="contact-grid">
      <a class="contact-card cc-email" href="mailto:aryarabade2006@gmail.com">
        <div class="cc-icon icon-email">📧</div>
        <div class="cc-text">
          <div class="cc-name">Email</div>
          <div class="cc-val">aryarabade2006@gmail.com</div>
        </div>
        <div class="cc-arrow">→</div>
      </a>
      <a class="contact-card cc-linkedin" href="https://linkedin.com/in/arya-rabade" target="_blank">
        <div class="cc-icon icon-linkedin">💼</div>
        <div class="cc-text">
          <div class="cc-name">LinkedIn</div>
          <div class="cc-val">arya-rabade</div>
        </div>
        <div class="cc-arrow">→</div>
      </a>
      <a class="contact-card cc-lc" href="https://leetcode.com/u/arya1624/" target="_blank">
        <div class="cc-icon icon-lc">⚡</div>
        <div class="cc-text">
          <div class="cc-name">LeetCode</div>
          <div class="cc-val">@arya1624</div>
        </div>
        <div class="cc-arrow">→</div>
      </a>
      <a class="contact-card cc-phone" href="tel:+917841835474">
        <div class="cc-icon icon-phone">📱</div>
        <div class="cc-text">
          <div class="cc-name">Phone / WhatsApp</div>
          <div class="cc-val">+91 78418 35474</div>
        </div>
        <div class="cc-arrow">→</div>
      </a>
      <a class="contact-card cc-port" href="https://your-portfolio.com" target="_blank" style="grid-column: 1 / -1;">
        <div class="cc-icon icon-port">🌐</div>
        <div class="cc-text">
          <div class="cc-name">Portfolio</div>
          <div class="cc-val">your-portfolio.com</div>
        </div>
        <div class="cc-arrow">→</div>
      </a>
    </div>
  </div>

  <!-- QUOTE & FOOTER -->
  <div class="quote-section">
    <div class="quote-text">
      Coding isn't just about writing lines of code — it's about learning a better way to solve problems.
    </div>
    <div style="font-size:.72rem;color:#7c3aed;margin-top:.5rem;font-family:'Fira Code',monospace;">— Arya Rabade</div>
    <div class="footer-row">
      <span class="footer-badge" style="background:#1a0a2e;color:#c4b5fd;border:1px solid #7c3aed;">Curious</span>
      <span class="footer-badge" style="background:#001a0a;color:#6ee7b7;border:1px solid #10b981;">Driven</span>
      <span class="footer-badge" style="background:#001020;color:#7dd3fc;border:1px solid #0ea5e9;">Creative</span>
    </div>
    <div style="margin-top:1rem;font-size:.7rem;color:#30363d;font-family:'Fira Code',monospace;">
      ❤️ Thanks for visiting · Have a great day!
    </div>
  </div>

</div>

<script>
(function(){
  /* --- Typing animation --- */
  const lines = [
    'Full Stack MERN Developer 🚀',
    'Java Enthusiast ☕',
    'DSA Problem Solver 🧠',
    'B.Tech CSE @ Kolhapur 🎓',
    'Always Learning New Things 🌱'
  ];
  let li = 0, ci = 0, del = false;
  const el = document.getElementById('typingLine');
  function type(){
    const txt = lines[li];
    if(!del){
      ci++;
      el.innerHTML = txt.slice(0,ci) + '<span class="typing-cursor"></span>';
      if(ci === txt.length){ del = true; setTimeout(type, 1600); return; }
    } else {
      ci--;
      el.innerHTML = txt.slice(0,ci) + '<span class="typing-cursor"></span>';
      if(ci === 0){ del = false; li = (li+1) % lines.length; }
    }
    setTimeout(type, del ? 40 : 80);
  }
  type();

  /* --- Hero particle canvas --- */
  const canvas = document.getElementById('heroCanvas');
  const ctx = canvas.getContext('2d');
  function resize(){
    canvas.width  = canvas.offsetWidth;
    canvas.height = canvas.offsetHeight;
  }
  resize();
  window.addEventListener('resize', resize);

  const particles = Array.from({length: 40}, () => ({
    x:  Math.random() * canvas.width,
    y:  Math.random() * canvas.height,
    r:  Math.random() * 1.5 + 0.5,
    vx: (Math.random() - 0.5) * 0.4,
    vy: (Math.random() - 0.5) * 0.4,
    a:  Math.random() * 0.6 + 0.2
  }));

  function drawParticles(){
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    particles.forEach(p => {
      ctx.beginPath();
      ctx.arc(p.x, p.y, p.r, 0, Math.PI * 2);
      ctx.fillStyle = `rgba(167,139,250,${p.a})`;
      ctx.fill();
      p.x += p.vx; p.y += p.vy;
      if(p.x < 0 || p.x > canvas.width)  p.vx *= -1;
      if(p.y < 0 || p.y > canvas.height) p.vy *= -1;
    });
    requestAnimationFrame(drawParticles);
  }
  drawParticles();

  /* --- Activity bar --- */
  const bar = document.getElementById('activityBar');
  const heights = [20,35,45,60,80,55,70,90,65,75,50,85,40,95,70,55,80,60,45,30,75,90,65,80,55,40,70,85,60,95];
  const colors  = ['#7c3aed','#a78bfa','#38bdf8','#818cf8'];
  heights.forEach((h, i) => {
    const col = document.createElement('div');
    col.className = 'ab-col';
    col.style.height = h + '%';
    col.style.background = colors[i % colors.length];
    col.style.opacity = '.7';
    col.style.animationDelay = (i * 0.04) + 's';
    bar.appendChild(col);
  });

  /* --- LeetCode counter animation --- */
  function countUp(el, target, dur){
    let start = 0, step = target / dur * 16;
    function tick(){
      start += step;
      if(start >= target){ el.textContent = target; return; }
      el.textContent = Math.floor(start);
      requestAnimationFrame(tick);
    }
    tick();
  }
  setTimeout(() => {
    countUp(document.getElementById('lcEasy'), 85, 60);
    countUp(document.getElementById('lcMed'),  42, 60);
    countUp(document.getElementById('lcHard'),  8, 60);
  }, 400);
})();
</script>
</body>
</html>
