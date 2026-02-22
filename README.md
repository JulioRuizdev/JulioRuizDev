<div align="center">

<!-- Animated Header Banner -->
<div align="center" >
  <svg width="800" height="200" viewBox="0 0 800 200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Background gradient -->
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d1117;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#0a1628;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#0d1117;stop-opacity:1" />
    </linearGradient>

    <!-- Glitch clip paths -->
    <clipPath id="clip1">
      <rect x="0" y="0" width="800" height="200"/>
    </clipPath>
    <clipPath id="clip-top">
      <rect x="0" y="55" width="800" height="30"/>
    </clipPath>
    <clipPath id="clip-mid">
      <rect x="0" y="90" width="800" height="20"/>
    </clipPath>
    <clipPath id="clip-bot">
      <rect x="0" y="115" width="800" height="25"/>
    </clipPath>

    <!-- Glow filter -->
    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="4" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Cyan glow -->
    <filter id="glowCyan">
      <feGaussianBlur stdDeviation="6" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Scan line pattern -->
    <pattern id="scanlines" x="0" y="0" width="800" height="4" patternUnits="userSpaceOnUse">
      <rect x="0" y="0" width="800" height="2" fill="rgba(0,0,0,0.15)"/>
    </pattern>
  </defs>

  <!-- Background -->
  <rect width="800" height="200" fill="url(#bgGrad)" rx="12"/>

  <!-- Grid lines horizontal -->
  <g opacity="0.07" stroke="#58a6ff" stroke-width="0.5">
    <line x1="0" y1="40" x2="800" y2="40"/>
    <line x1="0" y1="80" x2="800" y2="80"/>
    <line x1="0" y1="120" x2="800" y2="120"/>
    <line x1="0" y1="160" x2="800" y2="160"/>
  </g>
  <!-- Grid lines vertical -->
  <g opacity="0.07" stroke="#58a6ff" stroke-width="0.5">
    <line x1="100" y1="0" x2="100" y2="200"/>
    <line x1="200" y1="0" x2="200" y2="200"/>
    <line x1="300" y1="0" x2="300" y2="200"/>
    <line x1="400" y1="0" x2="400" y2="200"/>
    <line x1="500" y1="0" x2="500" y2="200"/>
    <line x1="600" y1="0" x2="600" y2="200"/>
    <line x1="700" y1="0" x2="700" y2="200"/>
  </g>

  <!-- Wave bottom decoration -->
  <path d="M0,180 Q100,165 200,175 Q300,185 400,170 Q500,155 600,168 Q700,181 800,165 L800,200 L0,200 Z"
    fill="#58a6ff" opacity="0.06">
    <animate attributeName="d"
      values="
        M0,180 Q100,165 200,175 Q300,185 400,170 Q500,155 600,168 Q700,181 800,165 L800,200 L0,200 Z;
        M0,175 Q100,185 200,168 Q300,155 400,178 Q500,188 600,162 Q700,172 800,178 L800,200 L0,200 Z;
        M0,180 Q100,165 200,175 Q300,185 400,170 Q500,155 600,168 Q700,181 800,165 L800,200 L0,200 Z"
      dur="6s" repeatCount="indefinite"/>
  </path>

  <path d="M0,185 Q150,172 300,182 Q450,192 600,175 Q700,165 800,178 L800,200 L0,200 Z"
    fill="#1f6feb" opacity="0.08">
    <animate attributeName="d"
      values="
        M0,185 Q150,172 300,182 Q450,192 600,175 Q700,165 800,178 L800,200 L0,200 Z;
        M0,178 Q150,190 300,172 Q450,162 600,183 Q700,193 800,170 L800,200 L0,200 Z;
        M0,185 Q150,172 300,182 Q450,192 600,175 Q700,165 800,178 L800,200 L0,200 Z"
      dur="8s" repeatCount="indefinite"/>
  </path>

  <!-- Corner accents -->
  <g stroke="#58a6ff" stroke-width="2" fill="none" opacity="0.6">
    <path d="M10,30 L10,12 L30,12"/>
    <path d="M770,12 L790,12 L790,30"/>
    <path d="M10,170 L10,188 L30,188"/>
    <path d="M770,188 L790,188 L790,170"/>
  </g>

  <!-- Floating particles -->
  <g fill="#58a6ff" opacity="0.5">
    <circle cx="60" cy="50" r="2">
      <animate attributeName="cy" values="50;40;50" dur="3s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.5;1;0.5" dur="3s" repeatCount="indefinite"/>
    </circle>
    <circle cx="740" cy="60" r="1.5">
      <animate attributeName="cy" values="60;48;60" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.4;0.9;0.4" dur="4s" repeatCount="indefinite"/>
    </circle>
    <circle cx="120" cy="150" r="1.5">
      <animate attributeName="cy" values="150;140;150" dur="5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.3;0.8;0.3" dur="5s" repeatCount="indefinite"/>
    </circle>
    <circle cx="680" cy="145" r="2">
      <animate attributeName="cy" values="145;135;145" dur="3.5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.5;1;0.5" dur="3.5s" repeatCount="indefinite"/>
    </circle>
    <circle cx="400" cy="25" r="1.5">
      <animate attributeName="cx" values="400;410;400" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.3;0.7;0.3" dur="4s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- ═══ MAIN TEXT: JULIO KRACK ═══ -->

  <!-- Shadow / echo layer (red glitch) -->
  <text x="400" y="115" text-anchor="middle"
    font-family="'Courier New', monospace" font-size="72" font-weight="900"
    fill="#ff4444" opacity="0" letter-spacing="8"
    clip-path="url(#clip-top)">
    JULIO KRACK
    <animate attributeName="x" values="400;406;400;397;400" dur="4s" repeatCount="indefinite" begin="1s"/>
    <animate attributeName="opacity" values="0;0;0.6;0;0;0;0.4;0;0" dur="4s" repeatCount="indefinite" begin="1s"/>
  </text>

  <!-- Shadow / echo layer (cyan glitch) -->
  <text x="400" y="115" text-anchor="middle"
    font-family="'Courier New', monospace" font-size="72" font-weight="900"
    fill="#00ffff" opacity="0" letter-spacing="8"
    clip-path="url(#clip-mid)">
    JULIO KRACK
    <animate attributeName="x" values="400;394;400;403;400" dur="4s" repeatCount="indefinite" begin="1s"/>
    <animate attributeName="opacity" values="0;0;0;0.5;0;0;0;0.3;0" dur="4s" repeatCount="indefinite" begin="1s"/>
  </text>

  <!-- Main text -->
  <text x="400" y="115" text-anchor="middle"
    font-family="'Courier New', monospace" font-size="72" font-weight="900"
    fill="#58a6ff" filter="url(#glow)" letter-spacing="8">
    JULIO KRACK
    <animate attributeName="x" values="400;400;402;400;398;400;400" dur="4s" repeatCount="indefinite" begin="1s"/>
    <animate attributeName="opacity" values="1;1;0.85;1;0.9;1;1" dur="4s" repeatCount="indefinite" begin="1s"/>
  </text>

  <!-- Subtitle -->
  <text x="400" y="148" text-anchor="middle"
    font-family="'Courier New', monospace" font-size="15" font-weight="400"
    fill="#8b949e" letter-spacing="5">
    ☁ CLOUD  &amp;  DEVOPS  ENGINEER  ☁
    <animate attributeName="opacity" values="0.7;1;0.7" dur="3s" repeatCount="indefinite"/>
  </text>

  <!-- Top label -->
  <text x="400" y="38" text-anchor="middle"
    font-family="'Courier New', monospace" font-size="11"
    fill="#1f6feb" letter-spacing="4" opacity="0.8">
    // JulioRuizdev · Lima, Perú 🇵🇪
  </text>

  <!-- Scan lines overlay -->
  <rect width="800" height="200" fill="url(#scanlines)" rx="12" opacity="0.4"/>

  <!-- Border glow -->
  <rect width="800" height="200" fill="none" stroke="#58a6ff" stroke-width="1" rx="12" opacity="0.3">
    <animate attributeName="opacity" values="0.3;0.6;0.3" dur="3s" repeatCount="indefinite"/>
  </rect>
</svg>
</div>

<!-- Typing animation -->
[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=600&lines=☁️+Cloud+%26+DevOps+Engineer;🚀+Automating+everything+I+can;🐳+Docker+%7C+Kubernetes+%7C+Terraform;🔧+CI%2FCD+%7C+IaC+%7C+Monitoring;📍+Lima%2C+Perú)](https://git.io/typing-svg)

</div>

---

## 👾 About Me

```yaml
name: Julio Ruiz (Julio Krack)
pronouns: he/him
location: Lima, Perú 🇵🇪
role: Cloud & DevOps Engineer
education: Systems Engineering Graduate
focus:
  - Cloud Infrastructure (AWS / GCP / Azure)
  - Container Orchestration (Kubernetes / Docker)
  - Infrastructure as Code (Terraform / Ansible)
  - CI/CD Pipelines (Jenkins / GitHub Actions / GitLab CI)
  - Monitoring & Observability (Prometheus / Grafana / ELK)
currently_learning: Platform Engineering & FinOps
motto: "Automate today, scale tomorrow 🚀"
```

---

## ☁️ Cloud & DevOps Stack

<div align="center">

**Cloud Providers**

![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Google Cloud](https://img.shields.io/badge/GCP-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white)

**Containers & Orchestration**

![Docker](https://img.shields.io/badge/Docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-%230F1689.svg?style=for-the-badge&logo=helm&logoColor=white)

**IaC & Config Management**

![Terraform](https://img.shields.io/badge/Terraform-%235835CC.svg?style=for-the-badge&logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-%231A1918.svg?style=for-the-badge&logo=ansible&logoColor=white)

**CI/CD**

![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-%232C5263.svg?style=for-the-badge&logo=jenkins&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab%20CI-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white)

**Monitoring & Observability**

![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=Prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-%23F46800.svg?style=for-the-badge&logo=grafana&logoColor=white)
![ElasticSearch](https://img.shields.io/badge/-ElasticSearch-005571?style=for-the-badge&logo=elasticsearch)

**Scripting & Languages**

![Bash](https://img.shields.io/badge/Bash-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![YAML](https://img.shields.io/badge/YAML-%23ffffff.svg?style=for-the-badge&logo=yaml&logoColor=151515)

**Version Control & Collaboration**

![Git](https://img.shields.io/badge/Git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

</div>

---

## 📊 GitHub Stats

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=JulioRuizdev&show_icons=true&theme=github_dark&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff&text_color=8b949e"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=JulioRuizdev&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=8b949e"/>

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=JulioRuizdev&theme=github-dark-blue&hide_border=true&background=0D1117&stroke=58A6FF&ring=58A6FF&fire=FF6B6B&currStreakLabel=58A6FF)](https://git.io/streak-stats)

</div>

---

## 🏗️ DevOps Philosophy

<div align="center">

```
┌─────────────────────────────────────────────────────┐
│                                                     │
│   Plan → Code → Build → Test → Release → Deploy    │
│     ↑                                      │        │
│     └──────────── Operate → Monitor ───────┘        │
│                                                     │
│          "Everything as Code. Always." 🚀           │
│                                                     │
└─────────────────────────────────────────────────────┘
```

</div>

---

## 📬 Connect with Me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/juliocesarruizcardenas)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:julio.ruiz.dev@gmail.com)
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?style=for-the-badge&logo=Instagram&logoColor=white)](https://instagram.com/julio.ops.27)
[![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/JulioRuizdev)

</div>

---

<div align="center">

<!-- Profile views counter -->
![Profile Views](https://komarev.com/ghpvc/?username=JulioRuizdev&color=58a6ff&style=for-the-badge&label=PROFILE+VIEWS)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:16213e,50:1a1a2e,100:0d1117&height=120&section=footer" width="100%"/>

</div>
