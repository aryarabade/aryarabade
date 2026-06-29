<div align="center">

<svg width="860" height="520" viewBox="0 0 860 520" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d1117"/>
      <stop offset="50%" style="stop-color:#161b22"/>
      <stop offset="100%" style="stop-color:#0d1117"/>
    </linearGradient>
    <linearGradient id="ringGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#7c3aed"/>
      <stop offset="50%" style="stop-color:#a78bfa"/>
      <stop offset="100%" style="stop-color:#38bdf8"/>
    </linearGradient>
    <linearGradient id="textGrad" x1="0%" y1="0%" x2="200%" y2="0%">
      <stop offset="0%" style="stop-color:#a78bfa"/>
      <stop offset="50%" style="stop-color:#38bdf8"/>
      <stop offset="100%" style="stop-color:#a78bfa"/>
      <animateTransform attributeName="gradientTransform" type="translate" from="-100% 0" to="100% 0" dur="3s" repeatCount="indefinite"/>
    </linearGradient>
    <linearGradient id="barGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#7c3aed"/>
      <stop offset="100%" style="stop-color:#38bdf8"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <clipPath id="avatarClip"><circle cx="430" cy="90" r="44"/></clipPath>
  </defs>

  <!-- Background -->
  <rect width="860" height="520" fill="url(#bgGrad)" rx="16"/>

  <!-- Particle dots -->
  <circle cx="80" cy="60" r="1.5" fill="#a78bfa" opacity="0.5"><animate attributeName="opacity" values="0.5;1;0.5" dur="2.1s" repeatCount="indefinite"/></circle>
  <circle cx="150" cy="120" r="1" fill="#38bdf8" opacity="0.4"><animate attributeName="opacity" values="0.4;0.9;0.4" dur="3.2s" repeatCount="indefinite"/></circle>
  <circle cx="60" cy="200" r="1.5" fill="#a78bfa" opacity="0.3"><animate attributeName="opacity" values="0.3;0.8;0.3" dur="2.7s" repeatCount="indefinite"/></circle>
  <circle cx="780" cy="80" r="1" fill="#38bdf8" opacity="0.5"><animate attributeName="opacity" values="0.5;1;0.5" dur="1.9s" repeatCount="indefinite"/></circle>
  <circle cx="810" cy="160" r="1.5" fill="#a78bfa" opacity="0.4"><animate attributeName="opacity" values="0.4;0.8;0.4" dur="2.5s" repeatCount="indefinite"/></circle>
  <circle cx="760" cy="240" r="1" fill="#38bdf8" opacity="0.3"><animate attributeName="opacity" values="0.3;0.7;0.3" dur="3.5s" repeatCount="indefinite"/></circle>
  <circle cx="200" cy="40" r="1" fill="#7c3aed" opacity="0.4"><animate attributeName="opacity" values="0.4;0.9;0.4" dur="2.3s" repeatCount="indefinite"/></circle>
  <circle cx="660" cy="50" r="1.5" fill="#a78bfa" opacity="0.3"><animate attributeName="opacity" values="0.3;0.8;0.3" dur="3.1s" repeatCount="indefinite"/></circle>
  <circle cx="120" cy="300" r="1" fill="#38bdf8" opacity="0.4"><animate attributeName="opacity" values="0.4;0.9;0.4" dur="2.8s" repeatCount="indefinite"/></circle>
  <circle cx="740" cy="320" r="1.5" fill="#7c3aed" opacity="0.3"><animate attributeName="opacity" values="0.3;0.7;0.3" dur="4s" repeatCount="indefinite"/></circle>

  <!-- Avatar spinning ring -->
  <circle cx="430" cy="90" r="48" fill="none" stroke="url(#ringGrad)" stroke-width="3" stroke-dasharray="12 6">
    <animateTransform attributeName="transform" type="rotate" from="0 430 90" to="360 430 90" dur="8s" repeatCount="indefinite"/>
  </circle>
  <!-- Avatar inner circle -->
  <circle cx="430" cy="90" r="44" fill="#161b22"/>
  <text x="430" y="100" text-anchor="middle" font-family="Inter, sans-serif" font-size="22" font-weight="700" fill="#a78bfa">AR</text>

  <!-- Name with shimmer -->
  <text x="430" y="165" text-anchor="middle" font-family="Inter, sans-serif" font-size="30" font-weight="800" fill="url(#textGrad)" filter="url(#glow)">Arya Rabade</text>

  <!-- Sub info -->
  <text x="430" y="190" text-anchor="middle" font-family="'Courier New', monospace" font-size="12" fill="#8b949e">B.Tech CSE · Kolhapur · CGPA 8.0</text>

  <!-- Typing text line -->
  <text x="430" y="215" text-anchor="middle" font-family="'Courier New', monospace" font-size="12" fill="#a78bfa">Full Stack MERN Developer 🚀</text>

  <!-- Badges row -->
  <!-- Badge 1: MERN Stack -->
  <rect x="176" y="232" width="108" height="24" rx="12" fill="#2d1b69" stroke="#7c3aed" stroke-width="1"/>
  <text x="230" y="248" text-anchor="middle" font-family="'Courier New', monospace" font-size="10" font-weight="600" fill="#c4b5fd">🚀 MERN Stack</text>
  <!-- Badge 2: Java -->
  <rect x="294" y="232" width="118" height="24" rx="12" fill="#2d1500" stroke="#f97316" stroke-width="1"/>
  <text x="353" y="248" text-anchor="middle" font-family="'Courier New', monospace" font-size="10" font-weight="600" fill="#fdba74">☕ Java Enthusiast</text>
  <!-- Badge 3: DSA -->
  <rect x="422" y="232" width="108" height="24" rx="12" fill="#0c2d4d" stroke="#0ea5e9" stroke-width="1"/>
  <text x="476" y="248" text-anchor="middle" font-family="'Courier New', monospace" font-size="10" font-weight="600" fill="#7dd3fc">🧠 DSA Learner</text>
  <!-- Badge 4: Always Building -->
  <rect x="540" y="232" width="130" height="24" rx="12" fill="#0d2d1a" stroke="#10b981" stroke-width="1"/>
  <text x="605" y="248" text-anchor="middle" font-family="'Courier New', monospace" font-size="10" font-weight="600" fill="#6ee7b7">🌱 Always Building</text>

  <!-- Wave divider -->
  <path d="M0,270 C200,290 400,255 600,272 C750,283 820,262 860,270 L860,285 L0,285 Z" fill="#161b22"/>

  <!-- GITHUB STATS section bg -->
  <rect x="0" y="285" width="860" height="175" fill="#161b22"/>

  <!-- Section title -->
  <text x="50" y="310" font-family="'Courier New', monospace" font-size="11" font-weight="700" fill="#7c3aed" letter-spacing="2">// GITHUB STATS</text>
  <line x1="190" y1="307" x2="810" y2="307" stroke="#7c3aed" stroke-width="0.5" opacity="0.3"/>

  <!-- Stat cards -->
  <!-- Card 1: CGPA -->
  <rect x="50" y="320" width="235" height="70" rx="10" fill="#0d1117" stroke="#30363d" stroke-width="1"/>
  <text x="167" y="351" text-anchor="middle" font-family="Inter, sans-serif" font-size="26" font-weight="800" fill="url(#textGrad)">8.0</text>
  <text x="167" y="370" text-anchor="middle" font-family="Inter, sans-serif" font-size="11" fill="#8b949e">CGPA</text>

  <!-- Card 2: Projects -->
  <rect x="312" y="320" width="236" height="70" rx="10" fill="#0d1117" stroke="#30363d" stroke-width="1"/>
  <text x="430" y="351" text-anchor="middle" font-family="Inter, sans-serif" font-size="26" font-weight="800" fill="url(#textGrad)">3+</text>
  <text x="430" y="370" text-anchor="middle" font-family="Inter, sans-serif" font-size="11" fill="#8b949e">Projects</text>

  <!-- Card 3: Technologies -->
  <rect x="575" y="320" width="235" height="70" rx="10" fill="#0d1117" stroke="#30363d" stroke-width="1"/>
  <text x="692" y="351" text-anchor="middle" font-family="Inter, sans-serif" font-size="26" font-weight="800" fill="url(#textGrad)">5+</text>
  <text x="692" y="370" text-anchor="middle" font-family="Inter, sans-serif" font-size="11" fill="#8b949e">Technologies</text>

  <!-- Contribution activity bar -->
  <rect x="50" y="402" width="760" height="52" rx="8" fill="#0d1117" stroke="#30363d" stroke-width="1"/>
  <text x="65" y="420" font-family="'Courier New', monospace" font-size="9" fill="#8b949e">contribution activity</text>

  <!-- Activity bars (30 bars) -->
  <rect x="65"  y="448" width="14" height="6"  rx="2" fill="#7c3aed" opacity="0.7"><animate attributeName="height" values="6;12;6" dur="2s" begin="0s" repeatCount="indefinite"/><animate attributeName="y" values="448;442;448" dur="2s" begin="0s" repeatCount="indefinite"/></rect>
  <rect x="84"  y="440" width="14" height="14" rx="2" fill="#a78bfa" opacity="0.7"><animate attributeName="height" values="14;8;14" dur="2.2s" begin="0.1s" repeatCount="indefinite"/><animate attributeName="y" values="440;446;440" dur="2.2s" begin="0.1s" repeatCount="indefinite"/></rect>
  <rect x="103" y="435" width="14" height="19" rx="2" fill="#38bdf8" opacity="0.7"><animate attributeName="height" values="19;24;19" dur="1.8s" begin="0.2s" repeatCount="indefinite"/><animate attributeName="y" values="435;430;435" dur="1.8s" begin="0.2s" repeatCount="indefinite"/></rect>
  <rect x="122" y="428" width="14" height="26" rx="2" fill="#818cf8" opacity="0.7"><animate attributeName="height" values="26;20;26" dur="2.4s" begin="0.3s" repeatCount="indefinite"/><animate attributeName="y" values="428;434;428" dur="2.4s" begin="0.3s" repeatCount="indefinite"/></rect>
  <rect x="141" y="422" width="14" height="32" rx="2" fill="#7c3aed" opacity="0.7"><animate attributeName="height" values="32;26;32" dur="2s" begin="0.4s" repeatCount="indefinite"/><animate attributeName="y" values="422;428;422" dur="2s" begin="0.4s" repeatCount="indefinite"/></rect>
  <rect x="160" y="430" width="14" height="24" rx="2" fill="#a78bfa" opacity="0.7"><animate attributeName="height" values="24;30;24" dur="1.9s" begin="0.5s" repeatCount="indefinite"/><animate attributeName="y" values="430;424;430" dur="1.9s" begin="0.5s" repeatCount="indefinite"/></rect>
  <rect x="179" y="425" width="14" height="29" rx="2" fill="#38bdf8" opacity="0.7"><animate attributeName="height" values="29;22;29" dur="2.3s" begin="0.6s" repeatCount="indefinite"/><animate attributeName="y" values="425;432;425" dur="2.3s" begin="0.6s" repeatCount="indefinite"/></rect>
  <rect x="198" y="419" width="14" height="35" rx="2" fill="#818cf8" opacity="0.7"><animate attributeName="height" values="35;28;35" dur="2.1s" begin="0.7s" repeatCount="indefinite"/><animate attributeName="y" values="419;426;419" dur="2.1s" begin="0.7s" repeatCount="indefinite"/></rect>
  <rect x="217" y="427" width="14" height="27" rx="2" fill="#7c3aed" opacity="0.7"><animate attributeName="height" values="27;33;27" dur="1.7s" begin="0.8s" repeatCount="indefinite"/><animate attributeName="y" values="427;421;427" dur="1.7s" begin="0.8s" repeatCount="indefinite"/></rect>
  <rect x="236" y="424" width="14" height="30" rx="2" fill="#a78bfa" opacity="0.7"><animate attributeName="height" values="30;24;30" dur="2.5s" begin="0.9s" repeatCount="indefinite"/><animate attributeName="y" values="424;430;424" dur="2.5s" begin="0.9s" repeatCount="indefinite"/></rect>
  <rect x="255" y="432" width="14" height="22" rx="2" fill="#38bdf8" opacity="0.7"><animate attributeName="height" values="22;28;22" dur="2s" begin="1s" repeatCount="indefinite"/><animate attributeName="y" values="432;426;432" dur="2s" begin="1s" repeatCount="indefinite"/></rect>
  <rect x="274" y="418" width="14" height="36" rx="2" fill="#818cf8" opacity="0.7"><animate attributeName="height" values="36;29;36" dur="2.2s" begin="1.1s" repeatCount="indefinite"/><animate attributeName="y" values="418;425;418" dur="2.2s" begin="1.1s" repeatCount="indefinite"/></rect>
  <rect x="293" y="435" width="14" height="19" rx="2" fill="#7c3aed" opacity="0.7"><animate attributeName="height" values="19;25;19" dur="1.8s" begin="1.2s" repeatCount="indefinite"/><animate attributeName="y" values="435;429;435" dur="1.8s" begin="1.2s" repeatCount="indefinite"/></rect>
  <rect x="312" y="415" width="14" height="39" rx="2" fill="#a78bfa" opacity="0.7"><animate attributeName="height" values="39;32;39" dur="2.4s" begin="1.3s" repeatCount="indefinite"/><animate attributeName="y" values="415;422;415" dur="2.4s" begin="1.3s" repeatCount="indefinite"/></rect>
  <rect x="331" y="426" width="14" height="28" rx="2" fill="#38bdf8" opacity="0.7"><animate attributeName="height" values="28;22;28" dur="2s" begin="1.4s" repeatCount="indefinite"/><animate attributeName="y" values="426;432;426" dur="2s" begin="1.4s" repeatCount="indefinite"/></rect>
  <rect x="350" y="431" width="14" height="23" rx="2" fill="#818cf8" opacity="0.7"><animate attributeName="height" values="23;30;23" dur="1.9s" begin="1.5s" repeatCount="indefinite"/><animate attributeName="y" values="431;424;431" dur="1.9s" begin="1.5s" repeatCount="indefinite"/></rect>
  <rect x="369" y="421" width="14" height="33" rx="2" fill="#7c3aed" opacity="0.7"><animate attributeName="height" values="33;26;33" dur="2.3s" begin="1.6s" repeatCount="indefinite"/><animate attributeName="y" values="421;428;421" dur="2.3s" begin="1.6s" repeatCount="indefinite"/></rect>
  <rect x="388" y="429" width="14" height="25" rx="2" fill="#a78bfa" opacity="0.7"><animate attributeName="height" values="25;31;25" dur="2.1s" begin="1.7s" repeatCount="indefinite"/><animate attributeName="y" values="429;423;429" dur="2.1s" begin="1.7s" repeatCount="indefinite"/></rect>
  <rect x="407" y="435" width="14" height="19" rx="2" fill="#38bdf8" opacity="0.7"><animate attributeName="height" values="19;14;19" dur="1.7s" begin="1.8s" repeatCount="indefinite"/><animate attributeName="y" values="435;440;435" dur="1.7s" begin="1.8s" repeatCount="indefinite"/></rect>
  <rect x="426" y="440" width="14" height="14" rx="2" fill="#818cf8" opacity="0.7"><animate attributeName="height" values="14;20;14" dur="2.5s" begin="1.9s" repeatCount="indefinite"/><animate attributeName="y" values="440;434;440" dur="2.5s" begin="1.9s" repeatCount="indefinite"/></rect>
  <rect x="445" y="424" width="14" height="30" rx="2" fill="#7c3aed" opacity="0.7"><animate attributeName="height" values="30;24;30" dur="2s" begin="2s" repeatCount="indefinite"/><animate attributeName="y" values="424;430;424" dur="2s" begin="2s" repeatCount="indefinite"/></rect>
  <rect x="464" y="416" width="14" height="38" rx="2" fill="#a78bfa" opacity="0.7"><animate attributeName="height" values="38;31;38" dur="2.2s" begin="2.1s" repeatCount="indefinite"/><animate attributeName="y" values="416;423;416" dur="2.2s" begin="2.1s" repeatCount="indefinite"/></rect>
  <rect x="483" y="427" width="14" height="27" rx="2" fill="#38bdf8" opacity="0.7"><animate attributeName="height" values="27;33;27" dur="1.8s" begin="2.2s" repeatCount="indefinite"/><animate attributeName="y" values="427;421;427" dur="1.8s" begin="2.2s" repeatCount="indefinite"/></rect>
  <rect x="502" y="421" width="14" height="33" rx="2" fill="#818cf8" opacity="0.7"><animate attributeName="height" values="33;27;33" dur="2.4s" begin="2.3s" repeatCount="indefinite"/><animate attributeName="y" values="421;427;421" dur="2.4s" begin="2.3s" repeatCount="indefinite"/></rect>
  <rect x="521" y="429" width="14" height="25" rx="2" fill="#7c3aed" opacity="0.7"><animate attributeName="height" values="25;19;25" dur="2s" begin="2.4s" repeatCount="indefinite"/><animate attributeName="y" values="429;435;429" dur="2s" begin="2.4s" repeatCount="indefinite"/></rect>
  <rect x="540" y="435" width="14" height="19" rx="2" fill="#a78bfa" opacity="0.7"><animate attributeName="height" values="19;25;19" dur="1.9s" begin="2.5s" repeatCount="indefinite"/><animate attributeName="y" values="435;429;435" dur="1.9s" begin="2.5s" repeatCount="indefinite"/></rect>
  <rect x="559" y="423" width="14" height="31" rx="2" fill="#38bdf8" opacity="0.7"><animate attributeName="height" values="31;25;31" dur="2.3s" begin="2.6s" repeatCount="indefinite"/><animate attributeName="y" values="423;429;423" dur="2.3s" begin="2.6s" repeatCount="indefinite"/></rect>
  <rect x="578" y="418" width="14" height="36" rx="2" fill="#818cf8" opacity="0.7"><animate attributeName="height" values="36;30;36" dur="2.1s" begin="2.7s" repeatCount="indefinite"/><animate attributeName="y" values="418;424;418" dur="2.1s" begin="2.7s" repeatCount="indefinite"/></rect>
  <rect x="597" y="427" width="14" height="27" rx="2" fill="#7c3aed" opacity="0.7"><animate attributeName="height" values="27;33;27" dur="1.7s" begin="2.8s" repeatCount="indefinite"/><animate attributeName="y" values="427;421;427" dur="1.7s" begin="2.8s" repeatCount="indefinite"/></rect>
  <rect x="616" y="415" width="14" height="39" rx="2" fill="#a78bfa" opacity="0.7"><animate attributeName="height" values="39;33;39" dur="2.5s" begin="2.9s" repeatCount="indefinite"/><animate attributeName="y" values="415;421;415" dur="2.5s" begin="2.9s" repeatCount="indefinite"/></rect>

  <!-- Wave bottom -->
  <path d="M0,460 C180,445 400,470 600,455 C750,445 820,465 860,460 L860,520 L0,520 Z" fill="#0d1117"/>

</svg>

---

### 🛠️ Tech Stack

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=flat-square&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-404D59?style=flat-square&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=flat-square&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=flat-square&logo=mysql&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![DSA](https://img.shields.io/badge/DSA-red?style=flat-square&logo=leetcode&logoColor=white)

---

### 📊 Proficiency

```
MERN Stack       ████████████████████░░░░  82%
Java & OOP       ███████████████████░░░░░  78%
DSA / Algorithms █████████████████░░░░░░░  70%
Database         ██████████████████░░░░░░  75%
```

---

### 🚀 Featured Projects

| Project | Description | Tech | Impact |
|---------|-------------|------|--------|
| 💊 **Medicare Store Portal** | Medicine inventory system with live stock updates, smart alerts & pharmacy analytics | Express.js · MongoDB · MSSQL | Prevents expired medicine waste |
| ✅ **Smart Habit Tracker** | Habit-building app with streaks, reminders, and visual progress analytics | React · Node.js · MongoDB | Drives goal consistency |
| 💰 **AI Finance Tracker** | AI-powered dashboard that auto-categorizes spending and delivers smart budgeting insights | MERN · OpenAI · MongoDB | Data-driven money management |

---

### ⚡ LeetCode — @arya1624

![LeetCode Stats](https://leetcard.jacoblin.cool/arya1624?theme=dark&font=Fira%20Code&ext=heatmap)

---

### 🤝 Let's Connect

[![Email](https://img.shields.io/badge/Email-aryarabade2006@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:aryarabade2006@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-arya--rabade-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/arya-rabade)
[![LeetCode](https://img.shields.io/badge/LeetCode-arya1624-FFA116?style=for-the-badge&logo=leetcode&logoColor=white)](https://leetcode.com/u/arya1624/)

> *"Coding isn't just about writing lines of code — it's about learning a better way to solve problems."*
> — Arya Rabade

![](https://komarev.com/ghpvc/?username=aryarabade&color=7c3aed&style=flat-square&label=Profile+Views)

</div>

