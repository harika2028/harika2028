<svg width="1200" height="320" viewBox="0 0 1200 320" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#050414"/>
      <stop offset="45%" stop-color="#160a33"/>
      <stop offset="75%" stop-color="#2a0a4d"/>
      <stop offset="100%" stop-color="#3d0a4f"/>
    </linearGradient>
    <linearGradient id="blueGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00d4ff"/>
      <stop offset="100%" stop-color="#3a6bff"/>
    </linearGradient>
    <linearGradient id="pinkGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#ff2ecb"/>
      <stop offset="100%" stop-color="#a239ff"/>
    </linearGradient>
    <linearGradient id="emGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#3a6bff"/>
      <stop offset="50%" stop-color="#a239ff"/>
      <stop offset="100%" stop-color="#ff2ecb"/>
    </linearGradient>
    <radialGradient id="chipGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#c86bff" stop-opacity="0.55"/>
      <stop offset="100%" stop-color="#c86bff" stop-opacity="0"/>
    </radialGradient>
    <filter id="softBlur" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="3"/>
    </filter>
    <clipPath id="waveClip">
      <rect x="330" y="40" width="620" height="150"/>
    </clipPath>
  </defs>

  <!-- background -->
  <rect width="1200" height="320" fill="url(#bgGrad)"/>

  <!-- stars -->
  <g fill="#ffffff">
    <circle cx="60" cy="40" r="1.6"><animate attributeName="opacity" values="1;0.2;1" dur="2.6s" repeatCount="indefinite"/></circle>
    <circle cx="130" cy="90" r="1.2"><animate attributeName="opacity" values="0.3;1;0.3" dur="3.4s" repeatCount="indefinite"/></circle>
    <circle cx="1120" cy="50" r="1.6"><animate attributeName="opacity" values="1;0.2;1" dur="2.2s" repeatCount="indefinite"/></circle>
    <circle cx="1160" cy="120" r="1.2"><animate attributeName="opacity" values="0.2;1;0.2" dur="3s" repeatCount="indefinite"/></circle>
    <circle cx="1050" cy="230" r="1.4"><animate attributeName="opacity" values="1;0.3;1" dur="2.8s" repeatCount="indefinite"/></circle>
    <circle cx="980" cy="270" r="1.1"><animate attributeName="opacity" values="0.4;1;0.4" dur="3.6s" repeatCount="indefinite"/></circle>
    <circle cx="40" cy="230" r="1.3"><animate attributeName="opacity" values="0.3;1;0.3" dur="3.1s" repeatCount="indefinite"/></circle>
    <circle cx="220" cy="250" r="1.1"><animate attributeName="opacity" values="1;0.3;1" dur="2.4s" repeatCount="indefinite"/></circle>
    <circle cx="600" cy="30" r="1.2"><animate attributeName="opacity" values="0.3;1;0.3" dur="2.9s" repeatCount="indefinite"/></circle>
    <circle cx="720" cy="270" r="1.3"><animate attributeName="opacity" values="1;0.2;1" dur="3.3s" repeatCount="indefinite"/></circle>
  </g>

  <!-- distant ringed planet, bottom right -->
  <g transform="translate(1130,255)" opacity="0.85">
    <animateTransform attributeName="transform" type="translate" values="1130,255;1130,248;1130,255" dur="5s" repeatCount="indefinite"/>
    <circle r="14" fill="#7a4bff"/>
    <ellipse rx="26" ry="6" fill="none" stroke="#ff9dfb" stroke-width="2" opacity="0.8" transform="rotate(-18)"/>
  </g>

  <!-- satellite, top left, gentle bob + orbit dot -->
  <g transform="translate(95,58)">
    <animateTransform attributeName="transform" type="translate" values="95,58;95,46;95,58" dur="4.5s" repeatCount="indefinite"/>
    <g transform="rotate(-25)">
      <rect x="-9" y="-6" width="18" height="12" rx="2" fill="#dfe9ff" stroke="#8fd8ff" stroke-width="1"/>
      <rect x="-30" y="-3" width="18" height="18" fill="#3a6bff" opacity="0.85" stroke="#8fd8ff" stroke-width="1"/>
      <rect x="12" y="-3" width="18" height="18" fill="#3a6bff" opacity="0.85" stroke="#8fd8ff" stroke-width="1"/>
      <line x1="-9" y1="0" x2="-30" y2="6" stroke="#8fd8ff" stroke-width="1.5"/>
      <line x1="9" y1="0" x2="30" y2="6" stroke="#8fd8ff" stroke-width="1.5"/>
      <line x1="0" y1="-6" x2="0" y2="-16" stroke="#8fd8ff" stroke-width="1.5"/>
      <circle cx="0" cy="-18" r="1.6" fill="#ff2ecb"/>
    </g>
    <circle r="46" fill="none" stroke="#5b2bd6" stroke-width="0.8" opacity="0.5" stroke-dasharray="3 4"/>
    <circle r="3" fill="#ff2ecb">
      <animateMotion dur="6s" repeatCount="indefinite" path="M 46,0 A 46,46 0 1 1 45.99,0.1 Z"/>
    </circle>
  </g>
  <text x="95" y="120" text-anchor="middle" font-family="Segoe UI, Verdana, sans-serif" font-size="11" fill="#8fd8ff" opacity="0.85">SATELLITE</text>

  <!-- AI robot, left -->
  <g transform="translate(195,190)">
    <animateTransform attributeName="transform" type="translate" values="195,190;195,182;195,190" dur="3.6s" repeatCount="indefinite"/>
    <!-- antenna -->
    <line x1="0" y1="-64" x2="0" y2="-48" stroke="#8fd8ff" stroke-width="2"/>
    <circle cx="0" cy="-68" r="4" fill="#ff2ecb">
      <animate attributeName="opacity" values="1;0.35;1" dur="1.4s" repeatCount="indefinite"/>
    </circle>
    <!-- head -->
    <rect x="-30" y="-48" width="60" height="46" rx="16" fill="#151233" stroke="url(#blueGrad)" stroke-width="2.5"/>
    <!-- eyes -->
    <g fill="#8fd8ff">
      <ellipse cx="-13" cy="-26" rx="7" ry="9">
        <animate attributeName="ry" values="9;9;0.6;9;9" keyTimes="0;0.85;0.9;0.95;1" dur="4s" repeatCount="indefinite"/>
      </ellipse>
      <ellipse cx="13" cy="-26" rx="7" ry="9">
        <animate attributeName="ry" values="9;9;0.6;9;9" keyTimes="0;0.85;0.9;0.95;1" dur="4s" repeatCount="indefinite"/>
      </ellipse>
    </g>
    <!-- smile -->
    <path d="M -10,-8 Q 0,-1 10,-8" stroke="#8fd8ff" stroke-width="2" fill="none" stroke-linecap="round"/>
    <!-- body -->
    <rect x="-34" y="-2" width="68" height="52" rx="14" fill="#151233" stroke="url(#pinkGrad)" stroke-width="2.5"/>
    <rect x="-9" y="14" width="18" height="18" rx="4" fill="none" stroke="#ff9dfb" stroke-width="1.6"/>
    <circle cx="0" cy="23" r="3" fill="#ff2ecb">
      <animate attributeName="opacity" values="1;0.3;1" dur="1.8s" repeatCount="indefinite"/>
    </circle>
    <!-- arms -->
    <line x1="-34" y1="10" x2="-52" y2="-2" stroke="#8fd8ff" stroke-width="6" stroke-linecap="round"/>
    <line x1="34" y1="10" x2="52" y2="24" stroke="#8fd8ff" stroke-width="6" stroke-linecap="round"/>
    <circle cx="-52" cy="-2" r="6" fill="#3a6bff"/>
    <circle cx="52" cy="24" r="6" fill="#3a6bff"/>
  </g>
  <text x="195" y="278" text-anchor="middle" font-family="Segoe UI, Verdana, sans-serif" font-size="11" fill="#8fd8ff" opacity="0.85">AI ASSISTANT</text>

  <!-- VLSI chip, center -->
  <g transform="translate(400,150)">
    <circle r="90" fill="url(#chipGlow)">
      <animate attributeName="r" values="80;96;80" dur="3s" repeatCount="indefinite"/>
    </circle>
    <g transform="rotate(45)">
      <rect x="-48" y="-48" width="96" height="96" rx="8" fill="#120c2b" stroke="url(#emGrad)" stroke-width="3">
        <animate attributeName="stroke-opacity" values="0.6;1;0.6" dur="2.4s" repeatCount="indefinite"/>
      </rect>
      <!-- pins -->
      <g stroke="#c9a9ff" stroke-width="2">
        <line x1="-48" y1="-32" x2="-60" y2="-32"/><line x1="-48" y1="-12" x2="-60" y2="-12"/>
        <line x1="-48" y1="8" x2="-60" y2="8"/><line x1="-48" y1="28" x2="-60" y2="28"/>
        <line x1="48" y1="-32" x2="60" y2="-32"/><line x1="48" y1="-12" x2="60" y2="-12"/>
        <line x1="48" y1="8" x2="60" y2="8"/><line x1="48" y1="28" x2="60" y2="28"/>
        <line x1="-32" y1="-48" x2="-32" y2="-60"/><line x1="-12" y1="-48" x2="-12" y2="-60"/>
        <line x1="8" y1="-48" x2="8" y2="-60"/><line x1="28" y1="-48" x2="28" y2="-60"/>
        <line x1="-32" y1="48" x2="-32" y2="60"/><line x1="-12" y1="48" x2="-12" y2="60"/>
        <line x1="8" y1="48" x2="8" y2="60"/><line x1="28" y1="48" x2="28" y2="60"/>
      </g>
      <text x="0" y="7" text-anchor="middle" transform="rotate(-45)" font-family="Verdana, sans-serif" font-size="22" font-weight="bold" fill="#ff8dfb">VLSI</text>
    </g>
  </g>
  <text x="400" y="256" text-anchor="middle" font-family="Segoe UI, Verdana, sans-serif" font-size="11" fill="#c9a9ff" opacity="0.9">SMALL CHIPS, BIG IMPACT</text>

  <!-- EM waves flowing over the chip toward the tower -->
  <g clip-path="url(#waveClip)">
    <g>
      <animateTransform attributeName="transform" type="translate" values="0,0; -160,0" dur="3s" repeatCount="indefinite"/>
      <path d="M -160,150 Q -120,90 -80,150 T 0,150 T 80,150 T 160,150 T 240,150 T 320,150 T 400,150 T 480,150 T 560,150 T 640,150 T 720,150 T 800,150 T 880,150 T 960,150 T 1040,150"
            fill="none" stroke="url(#blueGrad)" stroke-width="3" opacity="0.9"/>
    </g>
    <g>
      <animateTransform attributeName="transform" type="translate" values="0,0; -160,0" dur="2.4s" repeatCount="indefinite"/>
      <path d="M -160,110 Q -120,150 -80,110 T 0,110 T 80,110 T 160,110 T 240,110 T 320,110 T 400,110 T 480,110 T 560,110 T 640,110 T 720,110 T 800,110 T 880,110 T 960,110 T 1040,110"
            fill="none" stroke="url(#pinkGrad)" stroke-width="3" opacity="0.9"/>
    </g>
  </g>
  <text x="470" y="72" font-family="Segoe UI, Verdana, sans-serif" font-size="12" font-weight="bold" fill="#8fd8ff">M WAVE</text>
  <text x="470" y="196" font-family="Segoe UI, Verdana, sans-serif" font-size="12" font-weight="bold" fill="#ff8dfb">E WAVE</text>

  <!-- merged EM wave heading to the tower -->
  <g clip-path="url(#waveClip)" transform="translate(0,0)">
    <g>
      <animateTransform attributeName="transform" type="translate" values="0,0; -220,0" dur="3.6s" repeatCount="indefinite"/>
      <path d="M 560,130 Q 615,80 670,130 T 780,130 T 890,130 T 1000,130 T 1110,130 T 1220,130"
            fill="none" stroke="url(#emGrad)" stroke-width="4" filter="url(#softBlur)" opacity="0.55"/>
      <path d="M 560,130 Q 615,80 670,130 T 780,130 T 890,130 T 1000,130 T 1110,130 T 1220,130"
            fill="none" stroke="url(#emGrad)" stroke-width="2.4" opacity="0.95"/>
    </g>
  </g>
  <text x="820" y="72" text-anchor="middle" font-family="Segoe UI, Verdana, sans-serif" font-size="13" font-weight="bold" fill="#ff8dfb">EM WAVE</text>

  <!-- communication tower, right -->
  <g transform="translate(1010,235)">
    <path d="M -22,0 L 0,-70 L 22,0 Z" fill="none" stroke="#c9a9ff" stroke-width="2.4"/>
    <line x1="-14" y1="-20" x2="14" y2="-20" stroke="#c9a9ff" stroke-width="1.6"/>
    <line x1="-8" y1="-42" x2="8" y2="-42" stroke="#c9a9ff" stroke-width="1.6"/>
    <line x1="0" y1="-70" x2="0" y2="-82" stroke="#c9a9ff" stroke-width="2"/>
    <circle cx="0" cy="-84" r="2.6" fill="#ff2ecb"/>
    <g stroke="#ff8dfb" fill="none" stroke-width="1.6">
      <circle cx="0" cy="-84" r="10" opacity="0"><animate attributeName="r" values="6;36" dur="2.6s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.8;0" dur="2.6s" repeatCount="indefinite"/></circle>
      <circle cx="0" cy="-84" r="10" opacity="0"><animate attributeName="r" values="6;36" begin="0.9s" dur="2.6s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.8;0" begin="0.9s" dur="2.6s" repeatCount="indefinite"/></circle>
      <circle cx="0" cy="-84" r="10" opacity="0"><animate attributeName="r" values="6;36" begin="1.8s" dur="2.6s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.8;0" begin="1.8s" dur="2.6s" repeatCount="indefinite"/></circle>
    </g>
  </g>
  <text x="1010" y="256" text-anchor="middle" font-family="Segoe UI, Verdana, sans-serif" font-size="11" fill="#c9a9ff" opacity="0.9">COMMUNICATION</text>

  <!-- circuit trace at the base -->
  <g stroke="#5b2bd6" stroke-width="1.4" fill="none" opacity="0.6">
    <path d="M 0,300 L 120,300 L 150,285 L 300,285 L 330,300 L 560,300 L 590,315 L 900,315 L 930,300 L 1200,300"/>
  </g>
  <g fill="#ff8dfb">
    <circle cx="150" cy="285" r="2.2"/>
    <circle cx="330" cy="300" r="2.2"/>
    <circle cx="590" cy="315" r="2.2"/>
    <circle cx="930" cy="300" r="2.2"/>
  </g>
</svg>

<div align="center">

<img src="assets/hero-banner.svg" width="100%" alt="Niha - ECE, VLSI, AI banner"/>

<br/>

<a href="https://harika2028.github.io/niha-portfolio/">
  <img src="https://readme-typing-svg.demolab.com?font=Segoe+UI&weight=600&size=26&duration=2800&pause=900&color=D690FF&center=true&vCenter=true&multiline=true&repeat=true&width=760&height=90&lines=Hi%2C+I'm+Niha+%F0%9F%91%8B;Electronics+%26+Communication+Engineer;Building+at+the+edge+of+Chips%2C+AI+%26+IoT" alt="Typing SVG" />
</a>

<br/>

[![Portfolio](https://img.shields.io/badge/Portfolio-View_Site-6a11cb?style=for-the-badge&logo=googlechrome&logoColor=white)](https://harika2028.github.io/niha-portfolio/)
[![Resume](https://img.shields.io/badge/Resume-Download-ff4ecb?style=for-the-badge&logo=readdotcv&logoColor=white)](https://harika2028.github.io/niha-portfolio/Niharesume.pdf)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-3a6bff?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/)
[![Email](https://img.shields.io/badge/Email-Message_Me-a239ff?style=for-the-badge&logo=gmail&logoColor=white)](mailto:yarasuneharika@gmail.com)

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2447,50:7b2ff7,100:ff4ecb&height=3&section=header"/>

### 🎓 About Me

<img align="right" width="270" src="https://harika2028.github.io/niha-portfolio/profile.jpeg" />

- 🔭 Electronics & Communication Engineering graduate (**Bapatla Women's Engineering College**, 2022 – 2026, CGPA **8.5**)
- 🔬 Core interest: **VLSI, CMOS & Low Power Design** — transistor-level circuit design and physical design concepts
- 🤖 Exploring the intersection of **VLSI, Embedded Systems, IoT and AI**
- 🧪 I learn best by building — circuit simulation, hardware prototyping and research-driven projects
- 📡 Fascinated by how signals, silicon and software come together to build real systems
- 💬 Ask me about **VLSI design styles (CMOS/GDI/FinFET), HDL simulation, or IoT-based embedded systems**
- 📫 Reach me at **yarasuneharika@gmail.com**

<br clear="right"/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2447,50:7b2ff7,100:ff4ecb&height=3&section=header"/>

### 🛠️ Technical Toolkit

<table align="center">
<tr>
<td valign="top" width="50%">

**💻 Programming**
<br/>
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**🔬 VLSI & Digital Design**
<br/>
![CMOS](https://img.shields.io/badge/CMOS-7B2FF7?style=flat-square)
![PTL](https://img.shields.io/badge/PTL-7B2FF7?style=flat-square)
![GDI](https://img.shields.io/badge/GDI-A239FF?style=flat-square)
![FinFET](https://img.shields.io/badge/FinFET-A239FF?style=flat-square)
![Low Power Design](https://img.shields.io/badge/Low_Power_Design-C13CD9?style=flat-square)

**🧩 HDL & Simulation**
<br/>
![Verilog](https://img.shields.io/badge/Verilog-FF4ECB?style=flat-square)
![VHDL](https://img.shields.io/badge/VHDL-FF4ECB?style=flat-square)
![Vivado](https://img.shields.io/badge/Vivado-D6249F?style=flat-square&logo=xilinx&logoColor=white)
![DSCH/Microwind](https://img.shields.io/badge/DSCH%20%2F%20Microwind-C13CD9?style=flat-square)
![Logisim](https://img.shields.io/badge/Logisim-D6249F?style=flat-square)

</td>
<td valign="top" width="50%">

**🌐 IoT & Embedded**
<br/>
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=arduino&logoColor=white)
![ESP8266](https://img.shields.io/badge/ESP8266-3A6BFF?style=flat-square&logo=espressif&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-3A6BFF?style=flat-square&logo=espressif&logoColor=white)
![ThingSpeak](https://img.shields.io/badge/ThingSpeak-00D4FF?style=flat-square)

**📐 Electronics**
<br/>
![PCB Design](https://img.shields.io/badge/PCB_Design-3A6BFF?style=flat-square)
![Digital Electronics](https://img.shields.io/badge/Digital_Electronics-3A6BFF?style=flat-square)
![Circuit Design](https://img.shields.io/badge/Circuit_Design-00D4FF?style=flat-square)

**🤖 AI & Computer Vision**
<br/>
![Python](https://img.shields.io/badge/DeepFace-FF4ECB?style=flat-square)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-A239FF?style=flat-square)

**⚙️ Backend & Blockchain**
<br/>
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![REST APIs](https://img.shields.io/badge/REST_APIs-6A11CB?style=flat-square)
![Blockchain](https://img.shields.io/badge/Blockchain-C13CD9?style=flat-square)
![Qiskit](https://img.shields.io/badge/Qiskit-6929C4?style=flat-square&logo=qiskit&logoColor=white)

</td>
</tr>
</table>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2447,50:7b2ff7,100:ff4ecb&height=3&section=header"/>

### 🚀 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

**⚡ [Low Power Hybrid Parallel Prefix Adder](https://harika2028.github.io/niha-portfolio/Low-Power-Hybrid-Parallel-Prefix-Adder.pdf)**
<br/>Hybrid parallel prefix adder combining Han-Carlson & Ladner-Fischer architectures for low-power VLSI applications.
<br/>`CMOS` `GDI` `FSGDI` `DSCH` `Microwind`

</td>
<td width="50%" valign="top">

**🌱 [Touch Me Not — Crop Protection System](https://harika2028.github.io/niha-portfolio/Touch-Me-Not-Project-Report.pdf)**
<br/>IoT-based crop protection system using sensors, solar tracking and wireless monitoring. Selected for an MSME innovation opportunity.
<br/>`Arduino` `ESP8266` `IoT` `ThingSpeak`

</td>
</tr>
<tr>
<td width="50%" valign="top">

**🔐 [Digital Locker System](https://harika2028.github.io/niha-portfolio/Digital-Locker-System-Project-Report.pdf)**
<br/>Digital locker system designed & simulated using digital logic, multiplexing and HDL concepts.
<br/>`DSCH` `Verilog` `Vivado` `Digital Logic`

</td>
<td width="50%" valign="top">

**🧮 4-Bit ALU**
<br/>Arithmetic logic unit designed and simulated with functional verification.
<br/>`Verilog` `ALU` `Vivado`

</td>
</tr>
<tr>
<td colspan="2" valign="top">

**⛓️ [FaceChain](https://harika2028.github.io/niha-portfolio/FaceChain_Report_Article.pdf) — AI • Computer Vision • Blockchain**
<br/>Privacy-aware prototype combining AI-based face analysis, reverse image search and blockchain provenance into a unified digital media verification pipeline.
<br/>`Python` `DeepFace` `OpenCV` `FAISS` `FastAPI` `SHA-256` `Blockchain`
<br/>[📄 Report](https://harika2028.github.io/niha-portfolio/FaceChain_Report_Article.pdf) · [💻 GitHub](https://github.com/harika2028)

</td>
</tr>
</table>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2447,50:7b2ff7,100:ff4ecb&height=3&section=header"/>

### 📊 GitHub Stats

<div align="center">
<img height="165" src="https://github-readme-stats.vercel.app/api?username=harika2028&show_icons=true&hide_border=true&bg_color=0d1117&title_color=ff4ecb&icon_color=7b2ff7&text_color=c9d1d9&ring_color=3a6bff" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=harika2028&layout=compact&hide_border=true&bg_color=0d1117&title_color=ff4ecb&text_color=c9d1d9&langs_count=8" />
</div>

<div align="center">
<img src="https://github-readme-streak-stats.herokuapp.com/?user=harika2028&hide_border=true&background=0d1117&ring=7b2ff7&fire=ff4ecb&currStreakLabel=c9d1d9&sideLabels=c9d1d9&dates=6e7681" />
</div>

<div align="center">
<img src="https://github-profile-trophy.vercel.app/?username=harika2028&theme=algolia&no-frame=true&column=7&margin-w=8&margin-h=8" />
</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2447,50:7b2ff7,100:ff4ecb&height=3&section=header"/>

### 🏆 Achievements & Certifications

- 🥇 **MSME Hackathon Project Selection** — Touch Me Not Crop Protection System selected for an MSME-focused innovation opportunity
- 🔬 **VLSI Project & Research Work** — Low-power hybrid parallel prefix adder analyzed across multiple logic styles with transistor-level simulation
- ⛓️ **FaceChain Technical Project** — AI face analysis + vector similarity search + blockchain provenance prototype
- 🏫 **Technical Workshops & Project Expo** — Active participant in electronics & emerging-tech exhibitions
- 🎓 **NPTEL & Coursera Certifications** — Continuous learning in core and emerging technical domains
- 🔧 **IoT & Electronics Workshop** — Hands-on exposure to hardware-oriented systems

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2447,50:7b2ff7,100:ff4ecb&height=3&section=header"/>

<div align="center">

### 📡 Let's Connect

I'm always interested in learning, collaborating and exploring opportunities in **VLSI, electronics, semiconductor technology and emerging technologies**.

[![Portfolio](https://img.shields.io/badge/-Portfolio-0f2447?style=for-the-badge&logo=googlechrome&logoColor=8fd8ff)](https://harika2028.github.io/niha-portfolio/)
[![Email](https://img.shields.io/badge/-Email-0f2447?style=for-the-badge&logo=gmail&logoColor=ff8dfb)](mailto:yarasuneharika@gmail.com)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0f2447?style=for-the-badge&logo=linkedin&logoColor=3a6bff)](https://www.linkedin.com/)
[![GitHub](https://img.shields.io/badge/-GitHub-0f2447?style=for-the-badge&logo=github&logoColor=c9d1d9)](https://github.com/harika2028)

<br/>

![Profile Views](https://komarev.com/ghpvc/?username=harika2028&color=a239ff&style=flat-square&label=Profile+Views)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:ff4ecb,50:7b2ff7,100:0f2447&height=100&section=footer"/>

</div>
