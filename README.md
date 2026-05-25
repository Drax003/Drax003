[README (2).md](https://github.com/user-attachments/files/28228351/README.2.md)[Uploading README (2).md<!-- HEADER -->
<div align="center">

<!-- ANIME FIGURE ANIMATION -->
<svg width="220" height="280" viewBox="0 0 220 280" xmlns="http://www.w3.org/2000/svg" style="filter: drop-shadow(0 0 18px #00FF88cc);">
  <defs>
    <radialGradient id="glowGrad" cx="50%" cy="50%" r="50%">
      <stop offset="0%" style="stop-color:#00FF88;stop-opacity:0.3"/>
      <stop offset="100%" style="stop-color:#00FF88;stop-opacity:0"/>
    </radialGradient>
    <linearGradient id="bodyGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#1a1a2e"/>
      <stop offset="100%" style="stop-color:#16213e"/>
    </linearGradient>
    <linearGradient id="hairGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#0f3460"/>
      <stop offset="100%" style="stop-color:#533483"/>
    </linearGradient>
    <linearGradient id="codeGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00FF88"/>
      <stop offset="100%" style="stop-color:#00ccff"/>
    </linearGradient>
    <filter id="blur2">
      <feGaussianBlur stdDeviation="2"/>
    </filter>
    <!-- Scanline pattern for hoodie -->
    <pattern id="scanlines" width="4" height="4" patternUnits="userSpaceOnUse">
      <line x1="0" y1="0" x2="4" y2="4" stroke="#00FF8822" stroke-width="0.5"/>
    </pattern>
  </defs>
  <style>
    .float { animation: float 3s ease-in-out infinite; }
    .blink { animation: blink 4s step-end infinite; }
    .type-cursor { animation: blink-cursor 0.8s step-end infinite; }
    .aura { animation: aura-pulse 2.5s ease-in-out infinite; }
    .hair-strand { animation: hair-wave 2s ease-in-out infinite; }
    .hair-strand2 { animation: hair-wave 2s ease-in-out infinite 0.3s; }
    .code-text { animation: code-scroll 6s linear infinite; }
    .circuit { animation: circuit-glow 2s ease-in-out infinite alternate; }
    @keyframes float {
      0%, 100% { transform: translateY(0px); }
      50% { transform: translateY(-10px); }
    }
    @keyframes blink {
      0%, 90%, 100% { opacity: 1; }
      95% { opacity: 0; }
    }
    @keyframes blink-cursor {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }
    @keyframes aura-pulse {
      0%, 100% { opacity: 0.4; r: 55; }
      50% { opacity: 0.8; r: 65; }
    }
    @keyframes hair-wave {
      0%, 100% { transform: rotate(0deg); transform-origin: top center; }
      50% { transform: rotate(3deg); transform-origin: top center; }
    }
    @keyframes code-scroll {
      0% { transform: translateY(0); opacity: 1; }
      80% { opacity: 1; }
      100% { transform: translateY(-60px); opacity: 0; }
    }
    @keyframes circuit-glow {
      0% { stroke: #00FF88; opacity: 0.4; }
      100% { stroke: #00ccff; opacity: 1; }
    }
  </style>

  <!-- Aura glow background -->
  <circle class="aura" cx="110" cy="150" r="55" fill="url(#glowGrad)" filter="url(#blur2)"/>

  <!-- FLOATING FIGURE GROUP -->
  <g class="float">

    <!-- === BODY (Hoodie) === -->
    <!-- Hoodie main body -->
    <path d="M70 175 Q65 200 62 240 L158 240 Q155 200 150 175 Q130 168 110 168 Q90 168 70 175Z"
          fill="url(#bodyGrad)" stroke="#00FF88" stroke-width="1.2"/>
    <!-- Hoodie scanline texture -->
    <path d="M70 175 Q65 200 62 240 L158 240 Q155 200 150 175 Q130 168 110 168 Q90 168 70 175Z"
          fill="url(#scanlines)" opacity="0.6"/>
    <!-- Hoodie center seam -->
    <line x1="110" y1="175" x2="110" y2="240" stroke="#00FF88" stroke-width="0.8" opacity="0.5"/>
    <!-- Hoodie pocket -->
    <path d="M90 210 Q90 225 110 225 Q130 225 130 210 Q130 205 110 205 Q90 205 90 210Z"
          fill="#0f1923" stroke="#00FF8866" stroke-width="1"/>
    <!-- Hoodie hood behind head -->
    <path d="M78 178 Q60 155 65 130 Q75 110 95 110 L110 108 L125 110 Q145 110 155 130 Q160 155 142 178"
          fill="#0d1527" stroke="#00FF8844" stroke-width="1"/>

    <!-- === ARMS === -->
    <!-- Left arm -->
    <path d="M70 178 Q50 195 48 220 Q55 222 60 222 Q65 200 78 188Z"
          fill="url(#bodyGrad)" stroke="#00FF88" stroke-width="1"/>
    <!-- Left hand -->
    <ellipse cx="50" cy="224" rx="8" ry="6" fill="#f5c9a0"/>
    <!-- Right arm (holding laptop / gesture) -->
    <path d="M150 178 Q165 195 168 215 Q161 218 156 217 Q152 198 142 188Z"
          fill="url(#bodyGrad)" stroke="#00FF88" stroke-width="1"/>
    <!-- Right hand -->
    <ellipse cx="166" cy="219" rx="8" ry="6" fill="#f5c9a0"/>

    <!-- === NECK === -->
    <rect x="102" y="158" width="16" height="14" rx="5" fill="#f5c9a0"/>

    <!-- === HEAD === -->
    <ellipse cx="110" cy="130" rx="38" ry="40" fill="#f5c9a0" stroke="#e8b88a" stroke-width="1"/>

    <!-- === HAIR === -->
    <!-- Main hair blob -->
    <path d="M75 118 Q72 90 85 75 Q98 60 110 62 Q122 60 135 75 Q148 90 145 118 Q138 108 130 105 Q120 102 110 103 Q100 102 90 105 Q82 108 75 118Z"
          fill="url(#hairGrad)"/>
    <!-- Side hair strands left -->
    <path class="hair-strand" d="M75 118 Q65 125 63 140 Q68 142 73 138 Q74 128 78 122Z" fill="url(#hairGrad)"/>
    <path class="hair-strand2" d="M77 130 Q66 140 67 155 Q72 157 76 153 Q76 142 80 135Z" fill="#0f3460" opacity="0.8"/>
    <!-- Side hair strands right -->
    <path class="hair-strand" d="M145 118 Q155 125 157 140 Q152 142 147 138 Q146 128 142 122Z" fill="url(#hairGrad)"/>
    <path class="hair-strand2" d="M143 130 Q154 140 153 155 Q148 157 144 153 Q144 142 140 135Z" fill="#0f3460" opacity="0.8"/>
    <!-- Hair ahoge (antenna strand) -->
    <path d="M110 62 Q113 45 118 38 Q114 36 110 40 Q106 36 102 38 Q107 45 110 62Z" fill="url(#hairGrad)"/>

    <!-- === FACE FEATURES === -->
    <!-- Eyes -->
    <g class="blink">
      <!-- Left eye -->
      <ellipse cx="96" cy="128" rx="7" ry="8" fill="white"/>
      <ellipse cx="96" cy="129" rx="5" ry="6" fill="#1a0a4e"/>
      <ellipse cx="96" cy="129" rx="3" ry="3.5" fill="#5533ff"/>
      <ellipse cx="94" cy="127" rx="1.5" ry="1.5" fill="white"/>
      <!-- Right eye -->
      <ellipse cx="124" cy="128" rx="7" ry="8" fill="white"/>
      <ellipse cx="124" cy="129" rx="5" ry="6" fill="#1a0a4e"/>
      <ellipse cx="124" cy="129" rx="3" ry="3.5" fill="#5533ff"/>
      <ellipse cx="122" cy="127" rx="1.5" ry="1.5" fill="white"/>
    </g>
    <!-- Eyebrows -->
    <path d="M88 118 Q96 115 104 118" fill="none" stroke="#4a3728" stroke-width="2" stroke-linecap="round"/>
    <path d="M116 118 Q124 115 132 118" fill="none" stroke="#4a3728" stroke-width="2" stroke-linecap="round"/>
    <!-- Nose -->
    <path d="M109 137 Q110 142 112 137" fill="none" stroke="#e0a882" stroke-width="1.2" stroke-linecap="round"/>
    <!-- Mouth (small smile) -->
    <path d="M103 148 Q110 154 117 148" fill="none" stroke="#c8856a" stroke-width="1.8" stroke-linecap="round"/>
    <!-- Blush marks -->
    <ellipse cx="88" cy="142" rx="7" ry="4" fill="#ffb3b3" opacity="0.4"/>
    <ellipse cx="132" cy="142" rx="7" ry="4" fill="#ffb3b3" opacity="0.4"/>

    <!-- === FLOATING CODE SCREEN (beside figure) === -->
    <g transform="translate(160, 100)">
      <!-- Screen glow -->
      <rect x="-2" y="-2" width="54" height="64" rx="5" fill="#00FF88" opacity="0.1" filter="url(#blur2)"/>
      <!-- Screen body -->
      <rect x="0" y="0" width="50" height="60" rx="4" fill="#0d1117" stroke="#00FF88" stroke-width="1.2"/>
      <!-- Screen scanline -->
      <rect x="0" y="0" width="50" height="60" rx="4" fill="url(#scanlines)" opacity="0.4"/>
      <!-- Code lines with scroll animation -->
      <clipPath id="screenClip"><rect x="0" y="0" width="50" height="60" rx="4"/></clipPath>
      <g clip-path="url(#screenClip)">
        <g class="code-text">
          <text x="4" y="14" font-family="monospace" font-size="5.5" fill="#00FF88">const dev = {</text>
          <text x="4" y="22" font-family="monospace" font-size="5.5" fill="#00ccff">  name: "you",</text>
          <text x="4" y="30" font-family="monospace" font-size="5.5" fill="#ff79c6">  skills: [</text>
          <text x="4" y="38" font-family="monospace" font-size="5.5" fill="#f1fa8c">    "hack",</text>
          <text x="4" y="46" font-family="monospace" font-size="5.5" fill="#f1fa8c">    "build",</text>
          <text x="4" y="54" font-family="monospace" font-size="5.5" fill="#00FF88">  ]</text>
          <text x="4" y="62" font-family="monospace" font-size="5.5" fill="#00FF88">}</text>
          <!-- Repeated for seamless loop -->
          <text x="4" y="76" font-family="monospace" font-size="5.5" fill="#00FF88">const dev = {</text>
          <text x="4" y="84" font-family="monospace" font-size="5.5" fill="#00ccff">  name: "you",</text>
          <text x="4" y="92" font-family="monospace" font-size="5.5" fill="#ff79c6">  skills: [</text>
          <text x="4" y="100" font-family="monospace" font-size="5.5" fill="#f1fa8c">    "hack",</text>
          <text x="4" y="108" font-family="monospace" font-size="5.5" fill="#f1fa8c">    "build",</text>
          <text x="4" y="116" font-family="monospace" font-size="5.5" fill="#00FF88">  ]</text>
          <text x="4" y="124" font-family="monospace" font-size="5.5" fill="#00FF88">}</text>
        </g>
      </g>
      <!-- Cursor blink -->
      <rect class="type-cursor" x="4" y="52" width="4" height="6" fill="#00FF88"/>
    </g>

    <!-- === CIRCUIT LINES (decorative) === -->
    <line class="circuit" x1="50" y1="224" x2="30" y2="240" stroke="#00FF88" stroke-width="1" stroke-dasharray="3,3"/>
    <circle cx="30" cy="240" r="2" fill="#00FF88" class="circuit"/>
    <line class="circuit" x1="166" y1="219" x2="190" y2="235" stroke="#00ccff" stroke-width="1" stroke-dasharray="3,3"/>
    <circle cx="190" cy="235" r="2" fill="#00ccff" class="circuit"/>

  </g><!-- end float group -->
</svg>

```
███████╗██╗   ██╗███████╗████████╗███████╗███╗   ███╗███████╗
██╔════╝╚██╗ ██╔╝██╔════╝╚══██╔══╝██╔════╝████╗ ████║██╔════╝
███████╗ ╚████╔╝ ███████╗   ██║   █████╗  ██╔████╔██║███████╗
╚════██║  ╚██╔╝  ╚════██║   ██║   ██╔══╝  ██║╚██╔╝██║╚════██║
███████║   ██║   ███████║   ██║   ███████╗██║ ╚═╝ ██║███████║
╚══════╝   ╚═╝   ╚══════╝   ╚═╝   ╚══════╝╚═╝     ╚═╝╚══════╝
```

### `[ hacker · builder · thinker · communicator ]`

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=500&color=00FF88&center=true&vCenter=true&width=600&lines=Breaking+things+to+build+them+better+%F0%9F%94%93;AI+%2B+Security+%3D+my+favourite+equation+%F0%9F%A4%96;Designing+systems+that+don't+fall+apart+%F0%9F%8F%97%EF%B8%8F;Full+stack%3F+More+like+full+snack+%F0%9F%8D%95;Communicating+ideas%2C+one+commit+at+a+time" alt="Typing SVG" />

</div>

---

<!-- ABOUT -->
## 👾 `whoami`

```bash
$ cat about.txt
```

```
Name     : [Your Name]
Location : 🌏 India
Status   : Turning coffee into secure, intelligent systems
Hobbies  : CTFs, building side projects, breaking stuff ethically
Superpower: Making complex things sound simple
```

> *"The best security is the one no one notices. The best code is the one everyone understands."*

---

<!-- SKILLS -->
## 🛠️ `ls ~/skills/`

<div align="center">

### 🔐 Cybersecurity
![Kali Linux](https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kali-linux&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2596CD?style=for-the-badge&logo=metasploit&logoColor=white)
![Burp Suite](https://img.shields.io/badge/Burp_Suite-FF6633?style=for-the-badge&logo=burp-suite&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP-000000?style=for-the-badge&logo=owasp&logoColor=white)

### 🤖 AI / Machine Learning
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)

### 🏗️ System Design & Architecture
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)

### 🌐 Full Stack
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)

</div>

---

<!-- STATS -->
## 📊 `./stats.sh`

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true&theme=chartreuse-dark&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_USERNAME&layout=compact&theme=chartreuse-dark&hide_border=true&bg_color=0d1117"/>

</div>

<div align="center">

![GitHub Streak](https://streak-stats.demolab.com?user=YOUR_USERNAME&theme=chartreuse-dark&hide_border=true&background=0D1117)

</div>

---

<!-- PROJECTS -->
## 🚀 `cat featured_projects.log`

| Project | Description | Stack |
|--------|-------------|-------|
| 🔐 **[Project Name]** | AI-powered threat detection system | `Python` `TensorFlow` `FastAPI` |
| 🌐 **[Project Name]** | Full stack app with end-to-end encryption | `React` `Node.js` `PostgreSQL` |
| 🤖 **[Project Name]** | LLM fine-tuned on security datasets | `PyTorch` `HuggingFace` `Docker` |
| 🏗️ **[Project Name]** | Distributed system with fault tolerance | `Go` `Redis` `Kubernetes` |

> 📌 *Replace the above with your real pinned projects!*

---

<!-- ACTIVITY -->
## 🐍 `watch -n 1 git log --oneline`

<div align="center">

![Snake animation](https://github.com/YOUR_USERNAME/YOUR_USERNAME/blob/output/github-contribution-grid-snake-dark.svg)

</div>

---

<!-- COMMUNICATION -->
## 🗣️ `ping me --anywhere`

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR_USERNAME)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/YOUR_USERNAME)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://yourwebsite.com)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:your@email.com)
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com/users/YOUR_ID)

</div>

---

<!-- FUN FOOTER -->
<div align="center">

```
while (alive) {
    eat();
    sleep();
    code();    // 🔥 this one loops the most
    hack();    // ethically, of course
    repeat();
}
```

![Visitor Count](https://komarev.com/ghpvc/?username=YOUR_USERNAME&color=00ff88&style=for-the-badge&label=VISITORS)

⭐ **If you like what you see, drop a star on something!** ⭐

</div>
…]()
