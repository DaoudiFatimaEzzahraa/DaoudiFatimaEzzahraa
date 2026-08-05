<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1600 500" width="100%" height="100%">
  <defs>
    <!-- COLOR GRADIENTS -->
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#050714"/>
      <stop offset="40%" stop-color="#0B1020"/>
      <stop offset="80%" stop-color="#121826"/>
      <stop offset="100%" stop-color="#1a102f"/>
    </linearGradient>

    <linearGradient id="skyGridGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#00E5FF" stop-opacity="0.15"/>
      <stop offset="100%" stop-color="#6C63FF" stop-opacity="0.0"/>
    </linearGradient>

    <linearGradient id="buildingGrad1" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#151b2d"/>
      <stop offset="100%" stop-color="#090d18"/>
    </linearGradient>

    <linearGradient id="buildingGrad2" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#1e263e"/>
      <stop offset="100%" stop-color="#0d1220"/>
    </linearGradient>

    <linearGradient id="holoBeam" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#00E5FF" stop-opacity="0.4"/>
      <stop offset="50%" stop-color="#6C63FF" stop-opacity="0.2"/>
      <stop offset="100%" stop-color="#00E5FF" stop-opacity="0.0"/>
    </linearGradient>

    <linearGradient id="neonCyanGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00E5FF"/>
      <stop offset="100%" stop-color="#38BDF8"/>
    </linearGradient>

    <linearGradient id="neonPurpleGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#6C63FF"/>
      <stop offset="100%" stop-color="#8B5CF6"/>
    </linearGradient>

    <linearGradient id="neonPinkGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#FF007F"/>
      <stop offset="100%" stop-color="#B388FF"/>
    </linearGradient>

    <linearGradient id="screenGradAI" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#081426"/>
      <stop offset="100%" stop-color="#030811"/>
    </linearGradient>

    <linearGradient id="screenGradCode" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#120a24"/>
      <stop offset="100%" stop-color="#05020c"/>
    </linearGradient>

    <radialGradient id="fogGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#6C63FF" stop-opacity="0.25"/>
      <stop offset="60%" stop-color="#00E5FF" stop-opacity="0.1"/>
      <stop offset="100%" stop-color="#0B1020" stop-opacity="0"/>
    </radialGradient>

    <radialGradient id="centerHoloGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#00E5FF" stop-opacity="0.5"/>
      <stop offset="40%" stop-color="#6C63FF" stop-opacity="0.3"/>
      <stop offset="100%" stop-color="#0B1020" stop-opacity="0"/>
    </radialGradient>

    <!-- GLOW FILTERS -->
    <filter id="glowCyan" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <filter id="glowPurple" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <filter id="glowSoft" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="2" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- REUSABLE PIXEL ASSETS -->
    <!-- Pixel Rain Unit -->
    <g id="rainDrop">
      <rect x="0" y="0" width="2" height="12" fill="#00E5FF" opacity="0.6"/>
      <rect x="0" y="12" width="2" height="4" fill="#FFFFFF" opacity="0.8"/>
    </g>

    <!-- Pixel Star -->
    <g id="pixelStar">
      <rect x="2" y="0" width="2" height="6" fill="#FFFFFF"/>
      <rect x="0" y="2" width="6" height="2" fill="#FFFFFF"/>
    </g>

    <!-- Drone Symbol -->
    <g id="cyberDrone">
      <rect x="4" y="8" width="24" height="6" fill="#1e263e" rx="1"/>
      <rect x="10" y="6" width="12" height="10" fill="#00E5FF" opacity="0.8"/>
      <rect x="2" y="4" width="6" height="2" fill="#6C63FF"/>
      <rect x="24" y="4" width="6" height="2" fill="#6C63FF"/>
      <circle cx="5" cy="5" r="3" fill="#FF007F">
        <animate attributeName="opacity" values="0.2;1;0.2" dur="0.6s" repeatCount="indefinite"/>
      </circle>
      <circle cx="27" cy="5" r="3" fill="#00E5FF">
        <animate attributeName="opacity" values="1;0.2;1" dur="0.6s" repeatCount="indefinite"/>
      </circle>
      <!-- Downward Scan Light -->
      <polygon points="12,14 4,35 28,35" fill="url(#holoBeam)" opacity="0.5"/>
    </g>

    <!-- Logo Mark Emblem -->
    <g id="fedEmblem">
      <path d="M 0,16 L 16,0 L 48,0 L 64,16 L 64,48 L 48,64 L 16,64 L 0,48 Z" fill="#090d18" stroke="#00E5FF" stroke-width="3"/>
      <path d="M 12,20 L 28,20 L 28,28 L 20,28 L 20,36 L 28,36 L 28,44 L 12,44 Z" fill="#6C63FF"/>
      <path d="M 32,20 L 48,20 L 52,28 L 52,36 L 48,44 L 32,44 Z M 40,28 L 44,28 L 44,36 L 40,36 Z" fill="#00E5FF"/>
      <rect x="8" y="8" width="4" height="4" fill="#FF007F"/>
      <rect x="52" y="8" width="4" height="4" fill="#00E5FF"/>
      <rect x="52" y="52" width="4" height="4" fill="#6C63FF"/>
      <rect x="8" y="52" width="4" height="4" fill="#B388FF"/>
    </g>
  </defs>

  <!-- ================= 1. BACKGROUND SKY & ENVIRONMENT ================= -->
  <rect width="1600" height="500" fill="url(#bgGrad)"/>

  <!-- Perspective Grid Lines in Sky -->
  <g opacity="0.2">
    <line x1="0" y1="250" x2="1600" y2="250" stroke="#6C63FF" stroke-width="1"/>
    <line x1="0" y1="200" x2="1600" y2="200" stroke="#6C63FF" stroke-width="0.5"/>
    <line x1="0" y1="150" x2="1600" y2="150" stroke="#6C63FF" stroke-width="0.5"/>
    <!-- Perspective Rays -->
    <line x1="800" y1="250" x2="0" y2="0" stroke="#00E5FF" stroke-width="0.5"/>
    <line x1="800" y1="250" x2="300" y2="0" stroke="#00E5FF" stroke-width="0.5"/>
    <line x1="800" y1="250" x2="600" y2="0" stroke="#00E5FF" stroke-width="0.5"/>
    <line x1="800" y1="250" x2="1000" y2="0" stroke="#00E5FF" stroke-width="0.5"/>
    <line x1="800" y1="250" x2="1300" y2="0" stroke="#00E5FF" stroke-width="0.5"/>
    <line x1="800" y1="250" x2="1600" y2="0" stroke="#00E5FF" stroke-width="0.5"/>
  </g>

  <!-- TWINKLING STARS -->
  <g>
    <use xlink:href="#pixelStar" x="120" y="30" opacity="0.8">
      <animate attributeName="opacity" values="0.2;1;0.2" dur="2s" repeatCount="indefinite"/>
    </use>
    <use xlink:href="#pixelStar" x="340" y="70" opacity="0.4">
      <animate attributeName="opacity" values="0.1;0.9;0.1" dur="3.5s" repeatCount="indefinite"/>
    </use>
    <use xlink:href="#pixelStar" x="520" y="25" opacity="0.9">
      <animate attributeName="opacity" values="0.9;0.2;0.9" dur="1.8s" repeatCount="indefinite"/>
    </use>
    <use xlink:href="#pixelStar" x="750" y="45" opacity="0.6">
      <animate attributeName="opacity" values="0.3;1;0.3" dur="2.7s" repeatCount="indefinite"/>
    </use>
    <use xlink:href="#pixelStar" x="980" y="30" opacity="0.8">
      <animate attributeName="opacity" values="0.8;0.1;0.8" dur="2.2s" repeatCount="indefinite"/>
    </use>
    <use xlink:href="#pixelStar" x="1150" y="80" opacity="0.5">
      <animate attributeName="opacity" values="0.2;1;0.2" dur="3.1s" repeatCount="indefinite"/>
    </use>
    <use xlink:href="#pixelStar" x="1380" y="35" opacity="0.9">
      <animate attributeName="opacity" values="1;0.3;1" dur="1.5s" repeatCount="indefinite"/>
    </use>
    <use xlink:href="#pixelStar" x="1500" y="65" opacity="0.7">
      <animate attributeName="opacity" values="0.1;0.8;0.1" dur="2.9s" repeatCount="indefinite"/>
    </use>
  </g>

  <!-- DRIFTING FOG LAYER 1 -->
  <rect x="-400" y="100" width="2400" height="200" fill="url(#fogGlow)">
    <animateTransform attributeName="transform" type="translate" values="-100 0; 100 0; -100 0" dur="20s" repeatCount="indefinite"/>
  </rect>

  <!-- ================= 2. CYBERPUNK CITY SKYLINE ================= -->
  <!-- Far Background Buildings Layer -->
  <g fill="url(#buildingGrad1)">
    <!-- Building Silhouettes Left -->
    <rect x="0" y="180" width="90" height="220"/>
    <rect x="70" y="140" width="60" height="260"/>
    <rect x="150" y="200" width="110" height="200"/>
    <rect x="280" y="110" width="85" height="290"/>
    <rect x="380" y="160" width="100" height="240"/>
    <!-- Center Gap for Hologram -->
    <rect x="1120" y="150" width="90" height="250"/>
    <rect x="1230" y="100" width="110" height="300"/>
    <rect x="1360" y="170" width="80" height="230"/>
    <rect x="1460" y="130" width="140" height="270"/>
  </g>

  <!-- Distant Building Windows (Animated Flickers) -->
  <g fill="#00E5FF" opacity="0.4">
    <!-- Building Left 1 -->
    <rect x="80" y="160" width="4" height="6"/>
    <rect x="90" y="160" width="4" height="6"/>
    <rect x="80" y="180" width="4" height="6" fill="#FF007F">
      <animate attributeName="opacity" values="0.1;1;0.1" dur="3s" repeatCount="indefinite"/>
    </rect>
    <rect x="100" y="210" width="4" height="6"/>
    <!-- Highrise 280px -->
    <rect x="295" y="130" width="6" height="4"/>
    <rect x="310" y="130" width="6" height="4"/>
    <rect x="325" y="130" width="6" height="4" fill="#6C63FF"/>
    <rect x="295" y="150" width="6" height="4"/>
    <rect x="325" y="150" width="6" height="4"/>
    <rect x="295" y="170" width="6" height="4" fill="#00E5FF">
      <animate attributeName="opacity" values="1;0.2;1" dur="1.8s" repeatCount="indefinite"/>
    </rect>
    <!-- Right Highrise 1230px -->
    <rect x="1250" y="120" width="6" height="6" fill="#FF007F"/>
    <rect x="1270" y="120" width="6" height="6"/>
    <rect x="1290" y="120" width="6" height="6"/>
    <rect x="1250" y="140" width="6" height="6"/>
    <rect x="1290" y="140" width="6" height="6" fill="#00E5FF">
      <animate attributeName="opacity" values="0.2;1;0.2" dur="2.4s" repeatCount="indefinite"/>
    </rect>
  </g>

  <!-- Foreground Mid-Layer Skyscraper Details -->
  <g fill="url(#buildingGrad2)">
    <rect x="30" y="210" width="110" height="190"/>
    <rect x="210" y="150" width="95" height="250"/>
    <rect x="450" y="190" width="130" height="210"/>
    <!-- Spire Left -->
    <polygon points="255,80 253,150 257,150"/>
    
    <!-- Right Side Foreground Buildings -->
    <rect x="1020" y="180" width="120" height="220"/>
    <rect x="1300" y="140" width="105" height="260"/>
    <!-- Spire Right -->
    <polygon points="1350,60 1348,140 1352,140"/>
  </g>

  <!-- Spire Beacon Lights -->
  <circle cx="255" cy="80" r="3" fill="#FF007F" filter="url(#glowSoft)">
    <animate attributeName="opacity" values="1;0.1;1" dur="1s" repeatCount="indefinite"/>
  </circle>
  <circle cx="1350" cy="60" r="3" fill="#00E5FF" filter="url(#glowSoft)">
    <animate attributeName="opacity" values="0.1;1;0.1" dur="1.2s" repeatCount="indefinite"/>
  </circle>

  <!-- NEON ADVERTISEMENTS & HOLOGRAM SIGNS ON BUILDINGS -->
  <!-- Left Building Neon Sign "SIIA / IA" -->
  <g transform="translate(50, 230)">
    <rect x="0" y="0" width="70" height="25" fill="#090d18" stroke="#6C63FF" stroke-width="2"/>
    <text x="12" y="17" fill="#00E5FF" font-family="'Courier New', monospace" font-weight="bold" font-size="13" filter="url(#glowCyan)">SIIA</text>
    <rect x="0" y="0" width="70" height="25" fill="none" stroke="#FF007F" stroke-width="1" opacity="0.6">
      <animate attributeName="opacity" values="0.2;0.9;0.2" dur="0.4s" repeatCount="indefinite"/>
    </rect>
  </g>

  <!-- Right Building Neon Sign "MARRAKECH" -->
  <g transform="translate(1040, 210)">
    <rect x="0" y="0" width="80" height="50" fill="#090d18" stroke="#FF007F" stroke-width="1.5"/>
    <text x="8" y="22" fill="#FF007F" font-family="'Courier New', monospace" font-weight="bold" font-size="11" filter="url(#glowSoft)">MAROC</text>
    <text x="8" y="38" fill="#00E5FF" font-family="'Courier New', monospace" font-weight="bold" font-size="10">2026</text>
  </g>

  <!-- ================= 3. ANIMATED FLYING DRONES ================= -->
  <!-- Drone 1: Left to Right across sky -->
  <use xlink:href="#cyberDrone" x="0" y="0">
    <animateMotion path="M -50,120 L 1650,90" dur="14s" repeatCount="indefinite"/>
  </use>

  <!-- Drone 2: Right to Left lower altitude -->
  <use xlink:href="#cyberDrone" x="0" y="0">
    <animateMotion path="M 1650,180 L -50,210" dur="18s" repeatCount="indefinite"/>
  </use>

  <!-- ================= 4. CENTER GIGANTIC HOLOGRAPHIC LOGO ================= -->
  <!-- Hologram Emitter Base Platform -->
  <g transform="translate(800, 290)">
    <!-- Base Cone Light -->
    <polygon points="-120,20 120,20 220,-180 -220,-180" fill="url(#holoBeam)"/>
    
    <!-- Emitter Hardware -->
    <ellipse cx="0" cy="20" rx="130" ry="18" fill="#121826" stroke="#00E5FF" stroke-width="2"/>
    <ellipse cx="0" cy="20" rx="90" ry="12" fill="#090d18" stroke="#6C63FF" stroke-width="2"/>
    <ellipse cx="0" cy="20" rx="40" ry="6" fill="#00E5FF" filter="url(#glowCyan)">
      <animate attributeName="opacity" values="0.5;1;0.5" dur="1.5s" repeatCount="indefinite"/>
    </ellipse>
  </g>

  <!-- Central Hologram Floating Emblem + Rings -->
  <g transform="translate(800, 160)">
    <!-- Glow Backdrop -->
    <circle cx="0" cy="0" r="140" fill="url(#centerHoloGlow)"/>

    <!-- Rotating Outer Energy Ring 1 -->
    <g filter="url(#glowCyan)">
      <ellipse cx="0" cy="0" rx="130" ry="35" fill="none" stroke="#00E5FF" stroke-width="2" stroke-dasharray="20 10 5 10">
        <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="10s" repeatCount="indefinite"/>
      </ellipse>
    </g>

    <!-- Rotating Middle Ring 2 (Opposite direction & tilted) -->
    <g filter="url(#glowPurple)">
      <ellipse cx="0" cy="0" rx="110" ry="45" fill="none" stroke="#8B5CF6" stroke-width="2.5" stroke-dasharray="40 15">
        <animateTransform attributeName="transform" type="rotate" from="360" to="0" dur="7s" repeatCount="indefinite"/>
      </ellipse>
    </g>

    <!-- Rotating Inner Ring 3 -->
    <g filter="url(#glowSoft)">
      <ellipse cx="0" cy="0" rx="85" ry="85" fill="none" stroke="#FF007F" stroke-width="1.5" stroke-dasharray="10 30">
        <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="15s" repeatCount="indefinite"/>
      </ellipse>
    </g>

    <!-- Floating Holographic Core Logo (Scales & Pulses) -->
    <g filter="url(#glowCyan)">
      <g transform="translate(-32, -32)">
        <use xlink:href="#fedEmblem"/>
      </g>
      <!-- Vertical Pulse Scale Animation -->
      <animateTransform attributeName="transform" type="scale" values="1; 1.08; 1" dur="2.5s" repeatCount="indefinite"/>
    </g>

    <!-- Rising Holographic Data Particles -->
    <circle cx="-40" cy="40" r="2" fill="#00E5FF">
      <animate attributeName="cy" values="60;-80" dur="2s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;1;0" dur="2s" repeatCount="indefinite"/>
    </circle>
    <circle cx="30" cy="50" r="3" fill="#FF007F">
      <animate attributeName="cy" values="70;-90" dur="2.6s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;1;0" dur="2.6s" repeatCount="indefinite"/>
    </circle>
    <circle cx="60" cy="20" r="1.5" fill="#6C63FF">
      <animate attributeName="cy" values="50;-70" dur="1.8s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;1;0" dur="1.8s" repeatCount="indefinite"/>
    </circle>
    <circle cx="-70" cy="30" r="2.5" fill="#00E5FF">
      <animate attributeName="cy" values="40;-100" dur="2.2s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;1;0" dur="2.2s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- ================= 5. FOREGROUND DEVELOPER SETUP ================= -->
  <!-- Desk Base Structure -->
  <g id="deskSetup">
    <!-- Desk Shadow & Glow -->
    <rect x="250" y="370" width="1100" height="130" fill="#090d18"/>
    <!-- RGB Strip Line under desk edge -->
    <rect x="250" y="370" width="1100" height="4" fill="#00E5FF" filter="url(#glowCyan)">
      <animate attributeName="fill" values="#00E5FF;#6C63FF;#FF007F;#00E5FF" dur="6s" repeatCount="indefinite"/>
    </rect>

    <!-- ================= MONITOR 1 (LEFT: AI TRAINING) ================= -->
    <g transform="translate(320, 240)">
      <!-- Stand -->
      <rect x="135" y="120" width="30" height="25" fill="#151b2d"/>
      <rect x="110" y="142" width="80" height="8" fill="#090d18" stroke="#6C63FF" stroke-width="1"/>
      <!-- Monitor Frame -->
      <rect x="0" y="0" width="300" height="125" rx="6" fill="#0d1220" stroke="#00E5FF" stroke-width="2" filter="url(#glowSoft)"/>
      <!-- Screen Inner -->
      <rect x="8" y="8" width="284" height="109" rx="3" fill="url(#screenGradAI)"/>

      <!-- UI Header -->
      <rect x="8" y="8" width="284" height="16" fill="#121826"/>
      <circle cx="20" cy="16" r="3" fill="#FF007F"/>
      <circle cx="30" cy="16" r="3" fill="#B388FF"/>
      <circle cx="40" cy="16" r="3" fill="#00E5FF"/>
      <text x="55" y="19" fill="#00E5FF" font-family="'Courier New', monospace" font-size="9" font-weight="bold">AI_CORE_TRAINER v2.4 -- EPOCH 128/200</text>

      <!-- Training Progress Bar -->
      <text x="18" y="40" fill="#FFFFFF" font-family="'Courier New', monospace" font-size="10">Training Neural Net...</text>
      <rect x="18" y="46" width="200" height="10" fill="#090d18" stroke="#6C63FF" stroke-width="1"/>
      <!-- Animated Bar Fill -->
      <rect x="20" y="48" width="140" height="6" fill="url(#neonCyanGrad)">
        <animate attributeName="width" values="10;196;196;10" dur="6s" repeatCount="indefinite"/>
      </rect>
      <text x="225" y="55" fill="#00E5FF" font-family="'Courier New', monospace" font-size="10" font-weight="bold">78%</text>

      <!-- Loss / Accuracy Animated Graph Lines -->
      <g transform="translate(18, 65)">
        <rect x="0" y="0" width="264" height="42" fill="#050811" stroke="#151b2d" stroke-width="1"/>
        <!-- Grid lines inside graph -->
        <line x1="0" y1="14" x2="264" y2="14" stroke="#121826" stroke-width="1"/>
        <line x1="0" y1="28" x2="264" y2="28" stroke="#121826" stroke-width="1"/>
        
        <!-- Accuracy Wave (Cyan) -->
        <path d="M 0,35 Q 40,30 80,18 T 160,12 T 264,5" fill="none" stroke="#00E5FF" stroke-width="2" filter="url(#glowSoft)"/>
        <!-- Loss Wave (Magenta) -->
        <path d="M 0,5 Q 40,12 80,25 T 160,32 T 264,38" fill="none" stroke="#FF007F" stroke-width="1.5"/>
      </g>

      <!-- Live Log Text -->
      <text x="18" y="113" fill="#6C63FF" font-family="'Courier New', monospace" font-size="8">Loss: 0.0024 | Acc: 99.1% | GenAI Model: Active</text>
    </g>

    <!-- ================= MONITOR 2 (RIGHT: PYTHON / PYTORCH CODE) ================= -->
    <g transform="translate(980, 240)">
      <!-- Stand -->
      <rect x="135" y="120" width="30" height="25" fill="#151b2d"/>
      <rect x="110" y="142" width="80" height="8" fill="#090d18" stroke="#6C63FF" stroke-width="1"/>
      <!-- Monitor Frame -->
      <rect x="0" y="0" width="300" height="125" rx="6" fill="#0d1220" stroke="#8B5CF6" stroke-width="2" filter="url(#glowSoft)"/>
      <!-- Screen Inner -->
      <rect x="8" y="8" width="284" height="109" rx="3" fill="url(#screenGradCode)"/>

      <!-- UI Header -->
      <rect x="8" y="8" width="284" height="16" fill="#120a24"/>
      <circle cx="20" cy="16" r="3" fill="#FF007F"/>
      <circle cx="30" cy="16" r="3" fill="#B388FF"/>
      <circle cx="40" cy="16" r="3" fill="#00E5FF"/>
      <text x="55" y="19" fill="#B388FF" font-family="'Courier New', monospace" font-size="9" font-weight="bold">main.py -- PyTorch / GenAI</text>

      <!-- Animated Code Lines -->
      <g font-family="'Courier New', monospace" font-size="9" font-weight="bold" transform="translate(16, 34)">
        <text x="0" y="0" fill="#FF007F">import <tspan fill="#FFFFFF">torch</tspan></text>
        <text x="0" y="12" fill="#FF007F">from <tspan fill="#FFFFFF">nn</tspan> import <tspan fill="#00E5FF">Transformer</tspan></text>
        
        <text x="0" y="28" fill="#6C63FF"># Building Intelligent Systems</text>
        <text x="0" y="40" fill="#00E5FF">model = <tspan fill="#FFFFFF">GenAI(tech=</tspan><tspan fill="#B388FF">'SaaS'</tspan><tspan fill="#FFFFFF">)</tspan></text>
        <text x="0" y="52" fill="#00E5FF">model.<tspan fill="#FFFFFF">optimize(target=</tspan><tspan fill="#B388FF">'Prod'</tspan><tspan fill="#FFFFFF">)</tspan></text>
        
        <text x="0" y="68" fill="#FF007F">if <tspan fill="#FFFFFF">model.accuracy &gt; </tspan><tspan fill="#B388FF">0.99</tspan>:</text>
        <text x="12" y="80" fill="#00E5FF">print<tspan fill="#FFFFFF">(</tspan><tspan fill="#B388FF">"Deploying to Marrakech!"</tspan><tspan fill="#FFFFFF">)</tspan></text>

        <!-- Blinking Typing Cursor -->
        <rect x="180" y="72" width="6" height="10" fill="#00E5FF">
          <animate attributeName="opacity" values="1;0;1" dur="0.8s" repeatCount="indefinite"/>
        </rect>
      </g>
    </g>

    <!-- ================= KEYBOARD & MOUSE ================= -->
    <g transform="translate(680, 365)">
      <!-- Keyboard Base -->
      <rect x="0" y="0" width="240" height="22" rx="3" fill="#121826" stroke="#6C63FF" stroke-width="1.5"/>
      <!-- Individual Animated RGB Key Rows -->
      <!-- Row 1 -->
      <g fill="#00E5FF">
        <rect x="8" y="3" width="12" height="4" rx="1"/>
        <rect x="23" y="3" width="12" height="4" rx="1"/>
        <rect x="38" y="3" width="12" height="4" rx="1"/>
        <rect x="53" y="3" width="12" height="4" rx="1"/>
        <rect x="68" y="3" width="12" height="4" rx="1"/>
        <rect x="83" y="3" width="12" height="4" rx="1" fill="#FF007F"/>
        <rect x="98" y="3" width="12" height="4" rx="1"/>
        <rect x="113" y="3" width="12" height="4" rx="1"/>
        <rect x="128" y="3" width="12" height="4" rx="1"/>
        <rect x="143" y="3" width="12" height="4" rx="1"/>
        <rect x="158" y="3" width="12" height="4" rx="1"/>
        <rect x="173" y="3" width="20" height="4" rx="1" fill="#6C63FF"/>
      </g>
      <!-- Row 2 -->
      <g fill="#6C63FF">
        <rect x="8" y="9" width="16" height="4" rx="1"/>
        <rect x="27" y="9" width="12" height="4" rx="1"/>
        <rect x="42" y="9" width="12" height="4" rx="1" fill="#00E5FF"/>
        <rect x="57" y="9" width="12" height="4" rx="1"/>
        <rect x="72" y="9" width="12" height="4" rx="1"/>
        <rect x="87" y="9" width="12" height="4" rx="1"/>
        <rect x="102" y="9" width="12" height="4" rx="1"/>
        <rect x="117" y="9" width="12" height="4" rx="1"/>
        <rect x="132" y="9" width="12" height="4" rx="1"/>
        <rect x="147" y="9" width="12" height="4" rx="1"/>
        <rect x="162" y="9" width="31" height="4" rx="1" fill="#FF007F"/>
      </g>
      <!-- Row 3 (Spacebar row) -->
      <g fill="#B388FF">
        <rect x="8" y="15" width="20" height="4" rx="1"/>
        <rect x="31" y="15" width="16" height="4" rx="1"/>
        <rect x="50" y="15" width="100" height="4" rx="1" fill="#00E5FF" filter="url(#glowCyan)">
          <animate attributeName="fill" values="#00E5FF;#FF007F;#6C63FF;#00E5FF" dur="4s" repeatCount="indefinite"/>
        </rect>
        <rect x="153" y="15" width="16" height="4" rx="1"/>
        <rect x="172" y="15" width="21" height="4" rx="1"/>
      </g>
    </g>

    <!-- Mouse -->
    <g transform="translate(945, 368)">
      <rect x="0" y="0" width="18" height="26" rx="8" fill="#121826" stroke="#00E5FF" stroke-width="1"/>
      <line x1="9" y1="3" x2="9" y2="9" stroke="#FF007F" stroke-width="1.5"/>
    </g>

    <!-- ================= COFFEE MUG & ANIMATED STEAM ================= -->
    <g transform="translate(620, 350)">
      <!-- Mug Body -->
      <rect x="0" y="10" width="22" height="24" rx="3" fill="#151b2d" stroke="#00E5FF" stroke-width="1.5"/>
      <!-- Handle -->
      <path d="M 22,14 C 28,14 28,24 22,28" fill="none" stroke="#00E5FF" stroke-width="1.5"/>
      <!-- Logo on Mug -->
      <rect x="6" y="18" width="10" height="8" fill="#6C63FF"/>

      <!-- Animated Steam Particle Trails -->
      <path d="M 6,8 Q 2,2 8,-6 T 4,-16" fill="none" stroke="#FFFFFF" stroke-width="1.5" stroke-linecap="round" opacity="0.5">
        <animate attributeName="d" values="M 6,8 Q 2,2 8,-6 T 4,-16; M 6,8 Q 10,2 4,-6 T 8,-16; M 6,8 Q 2,2 8,-6 T 4,-16" dur="3s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0.2;0.7;0.1" dur="3s" repeatCount="indefinite"/>
      </path>
      <path d="M 14,8 Q 18,0 12,-8 T 16,-20" fill="none" stroke="#00E5FF" stroke-width="1.5" stroke-linecap="round" opacity="0.4">
        <animate attributeName="d" values="M 14,8 Q 18,0 12,-8 T 16,-20; M 14,8 Q 10,0 16,-8 T 12,-20; M 14,8 Q 18,0 12,-8 T 16,-20" dur="2.5s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0.6;0.1;0.6" dur="2.5s" repeatCount="indefinite"/>
      </path>
    </g>

    <!-- ================= DESK PLANT (NEON BONSAI) ================= -->
    <g transform="translate(270, 320)">
      <!-- Pot -->
      <polygon points="10,45 35,45 40,25 5,25" fill="#121826" stroke="#6C63FF" stroke-width="1.5"/>
      <!-- Plant Stem & Leaves -->
      <path d="M 22,25 Q 15,15 20,0 Q 28,-10 22,-20" fill="none" stroke="#090d18" stroke-width="3"/>
      <!-- Pixel Leaves (Glow Neon) -->
      <circle cx="20" cy="0" r="6" fill="#00E5FF" opacity="0.8" filter="url(#glowSoft)"/>
      <circle cx="10" cy="10" r="5" fill="#6C63FF" opacity="0.8"/>
      <circle cx="30" cy="-5" r="7" fill="#00E5FF" opacity="0.9" filter="url(#glowCyan)"/>
      <circle cx="22" cy="-20" r="8" fill="#B388FF" opacity="0.8" filter="url(#glowSoft)"/>
    </g>

    <!-- ================= PIXEL CAT ON DESK ================= -->
    <g transform="translate(940, 335)">
      <!-- Cat Body -->
      <ellipse cx="20" cy="20" rx="14" ry="10" fill="#090d18" stroke="#121826" stroke-width="1"/>
      <!-- Cat Head -->
      <circle cx="10" cy="12" r="8" fill="#090d18"/>
      <!-- Ears -->
      <polygon points="4,6 8,0 10,6" fill="#6C63FF"/>
      <polygon points="12,6 14,0 17,6" fill="#6C63FF"/>
      <!-- Glowing Eyes -->
      <circle cx="7" cy="11" r="1.5" fill="#00E5FF">
        <animate attributeName="opacity" values="1;1;0;1" keyTimes="0;0.9;0.95;1" dur="4s" repeatCount="indefinite"/>
      </circle>
      <circle cx="12" cy="11" r="1.5" fill="#00E5FF">
        <animate attributeName="opacity" values="1;1;0;1" keyTimes="0;0.9;0.95;1" dur="4s" repeatCount="indefinite"/>
      </circle>
      <!-- Tail Animation -->
      <path d="M 32,22 Q 40,15 38,8" fill="none" stroke="#090d18" stroke-width="3" stroke-linecap="round">
        <animate attributeName="d" values="M 32,22 Q 40,15 38,8; M 32,22 Q 42,25 40,18; M 32,22 Q 40,15 38,8" dur="3s" repeatCount="indefinite"/>
      </path>
    </g>

    <!-- ================= MAIN FEMALE DEVELOPER CHARACTER ================= -->
    <g id="character" transform="translate(730, 260)">
      <!-- Slight Typing Motion Animation -->
      <animateTransform attributeName="transform" type="translate" values="730,260; 730,258.5; 730,260" dur="2s" repeatCount="indefinite"/>

      <!-- Hoodie Body (Back View) -->
      <path d="M 20,70 Q 70,50 120,70 L 130,140 L 10,140 Z" fill="#0d1220" stroke="#151b2d" stroke-width="2"/>
      
      <!-- Logo Emblem on Back of Hoodie -->
      <g transform="translate(53, 78) scale(0.5)" filter="url(#glowSoft)">
        <use xlink:href="#fedEmblem"/>
      </g>

      <!-- Hoodie Folds Details -->
      <path d="M 35,85 Q 50,110 45,140" fill="none" stroke="#151b2d" stroke-width="2"/>
      <path d="M 105,85 Q 90,110 95,140" fill="none" stroke="#151b2d" stroke-width="2"/>

      <!-- Shoulders & Arms extending to keyboard -->
      <path d="M 15,80 L -10,120 L 10,135 L 30,95" fill="#0d1220"/>
      <path d="M 125,80 L 150,120 L 130,135 L 110,95" fill="#0d1220"/>

      <!-- Head & Hair (Dark Pixel Style) -->
      <path d="M 45,25 Q 70,10 95,25 L 100,55 Q 70,65 40,55 Z" fill="#050714"/>
      <!-- Hair Highlights (Purple/Cyan Neon Refraction) -->
      <path d="M 42,30 Q 35,50 38,70" fill="none" stroke="#6C63FF" stroke-width="2"/>
      <path d="M 98,30 Q 105,50 102,70" fill="none" stroke="#00E5FF" stroke-width="2"/>

      <!-- RGB Headphones -->
      <g transform="translate(32, 20)">
        <!-- Band -->
        <path d="M 10,15 Q 38,-5 66,15" fill="none" stroke="#1c2541" stroke-width="5"/>
        <!-- Left Ear Cup + Glow LED -->
        <rect x="2" y="12" width="12" height="22" rx="4" fill="#090d18" stroke="#00E5FF" stroke-width="1.5"/>
        <rect x="5" y="16" width="6" height="14" rx="2" fill="#00E5FF" filter="url(#glowCyan)">
          <animate attributeName="fill" values="#00E5FF;#FF007F;#00E5FF" dur="3s" repeatCount="indefinite"/>
        </rect>
        <!-- Right Ear Cup + Glow LED -->
        <rect x="62" y="12" width="12" height="22" rx="4" fill="#090d18" stroke="#FF007F" stroke-width="1.5"/>
        <rect x="65" y="16" width="6" height="14" rx="2" fill="#FF007F" filter="url(#glowSoft)">
          <animate attributeName="fill" values="#FF007F;#6C63FF;#FF007F" dur="3s" repeatCount="indefinite"/>
        </rect>
      </g>
    </g>
  </g>

  <!-- ================= 6. TOP RIGHT HUD STATUS PANEL ================= -->
  <g id="statusPanel" transform="translate(1260, 25)">
    <!-- Cyberpunk Border Box -->
    <polygon points="0,0 300,0 315,15 315,140 15,140 0,125" fill="#090d18" fill-opacity="0.85" stroke="#00E5FF" stroke-width="1.5" filter="url(#glowSoft)"/>
    <!-- Top Corner Accent -->
    <polygon points="0,0 40,0 0,40" fill="#00E5FF" opacity="0.3"/>

    <!-- Header -->
    <text x="20" y="22" fill="#00E5FF" font-family="'Courier New', monospace" font-weight="bold" font-size="12" filter="url(#glowCyan)">// SYSTEM_STATUS</text>

    <!-- Status Items -->
    <!-- Item 1: AI Core -->
    <text x="20" y="45" fill="#FFFFFF" font-family="'Courier New', monospace" font-size="10" font-weight="bold">AI CORE:</text>
    <text x="90" y="45" fill="#00E5FF" font-family="'Courier New', monospace" font-size="10" font-weight="bold">ONLINE</text>
    <circle cx="145" cy="42" r="4" fill="#00E5FF" filter="url(#glowCyan)">
      <animate attributeName="opacity" values="1;0.2;1" dur="1s" repeatCount="indefinite"/>
    </circle>

    <!-- Item 2: Creativity Bar -->
    <text x="20" y="68" fill="#FFFFFF" font-family="'Courier New', monospace" font-size="10" font-weight="bold">CREATIVITY:</text>
    <rect x="100" y="60" width="190" height="10" fill="#121826" stroke="#6C63FF" stroke-width="1"/>
    <rect x="102" y="62" width="186" height="6" fill="url(#neonPurpleGrad)"/>

    <!-- Item 3: Coffee Bar -->
    <text x="20" y="91" fill="#FFFFFF" font-family="'Courier New', monospace" font-size="10" font-weight="bold">COFFEE:</text>
    <rect x="100" y="83" width="190" height="10" fill="#121826" stroke="#FF007F" stroke-width="1"/>
    <rect x="102" y="85" width="140" height="6" fill="url(#neonPinkGrad)">
      <animate attributeName="width" values="140;186;100;140" dur="12s" repeatCount="indefinite"/>
    </rect>

    <!-- Item 4: Bug Counter -->
    <text x="20" y="115" fill="#FFFFFF" font-family="'Courier New', monospace" font-size="10" font-weight="bold">BUGS DETECTED:</text>
    <text x="130" y="115" fill="#FF007F" font-family="'Courier New', monospace" font-size="12" font-weight="bold" filter="url(#glowSoft)">0</text>
    
    <!-- Decorative Tech Dots -->
    <rect x="290" y="120" width="4" height="4" fill="#00E5FF"/>
    <rect x="298" y="120" width="4" height="4" fill="#6C63FF"/>
    <rect x="306" y="120" width="4" height="4" fill="#FF007F"/>
  </g>

  <!-- ================= 7. MAIN TYPOGRAPHY & HEADERS ================= -->
  <!-- Top Center Title "FED" -->
  <g transform="translate(800, 55)" text-anchor="middle">
    <!-- Main Glowing Text -->
    <text x="0" y="0" fill="#FFFFFF" font-family="'Courier New', monospace" font-weight="900" font-size="42" letter-spacing="8" filter="url(#glowCyan)">FED</text>
    <text x="0" y="0" fill="#00E5FF" font-family="'Courier New', monospace" font-weight="900" font-size="42" letter-spacing="8">FED</text>
    
    <!-- Subtitle -->
    <text x="0" y="24" fill="#B388FF" font-family="'Courier New', monospace" font-weight="bold" font-size="14" letter-spacing="3" filter="url(#glowSoft)">BUILDING INTELLIGENT SYSTEMS</text>

    <!-- Badges Row -->
    <g transform="translate(0, 36)">
      <!-- Badge 1: AI/ML/DL -->
      <rect x="-160" y="0" width="95" height="18" rx="4" fill="#090d18" stroke="#00E5FF" stroke-width="1"/>
      <text x="-112" y="13" fill="#00E5FF" font-family="'Courier New', monospace" font-size="9" font-weight="bold">AI / ML / DL</text>

      <!-- Badge 2: GenAI x SaaS -->
      <rect x="-50" y="0" width="100" height="18" rx="4" fill="#090d18" stroke="#6C63FF" stroke-width="1"/>
      <text x="0" y="13" fill="#B388FF" font-family="'Courier New', monospace" font-size="9" font-weight="bold">GenAI × SaaS</text>

      <!-- Badge 3: Marrakech -->
      <rect x="65" y="0" width="95" height="18" rx="4" fill="#090d18" stroke="#FF007F" stroke-width="1"/>
      <text x="112" y="13" fill="#FF007F" font-family="'Courier New', monospace" font-size="9" font-weight="bold">Marrakech 🇲🇦</text>
    </g>
  </g>

  <!-- ================= 8. DENSE ANIMATED PIXEL RAIN OVERLAY ================= -->
  <g opacity="0.7">
    <!-- Stream 1 -->
    <use xlink:href="#rainDrop" x="50" y="0">
      <animateTransform attributeName="transform" type="translate" values="0,-100; -80,600" dur="1.2s" repeatCount="indefinite"/>
    </use>
    <!-- Stream 2 -->
    <use xlink:href="#rainDrop" x="180" y="0">
      <animateTransform attributeName="transform" type="translate" values="0,-100; -80,600" dur="0.9s" begin="0.3s" repeatCount="indefinite"/>
    </use>
    <!-- Stream 3 -->
    <use xlink:href="#rainDrop" x="320" y="0">
      <animateTransform attributeName="transform" type="translate" values="0,-100; -80,600" dur="1.4s" begin="0.7s" repeatCount="indefinite"/>
    </use>
    <!-- Stream 4 -->
    <use xlink:href="#rainDrop" x="480" y="0">
      <animateTransform attributeName="transform" type="translate" values="0,-100; -80,600" dur="1.1s" begin="0.2s" repeatCount="indefinite"/>
    </use>
    <!-- Stream 5 -->
    <use xlink:href="#rainDrop" x="640" y="0">
      <animateTransform attributeName="transform" type="translate" values="0,-100; -80,600" dur="1.0s" begin="0.5s" repeatCount="indefinite"/>
    </use>
    <!-- Stream 6 -->
    <use xlink:href="#rainDrop" x="820" y="0">
      <animateTransform attributeName="transform" type="translate" values="0,-100; -80,600" dur="1.3s" begin="0.1s" repeatCount="indefinite"/>
    </use>
    <!-- Stream 7 -->
    <use xlink:href="#rainDrop" x="960" y="0">
      <animateTransform attributeName="transform" type="translate" values="0,-100; -80,600" dur="0.95s" begin="0.6s" repeatCount="indefinite"/>
    </use>
    <!-- Stream 8 -->
    <use xlink:href="#rainDrop" x="1120" y="0">
      <animateTransform attributeName="transform" type="translate" values="0,-100; -80,600" dur="1.25s" begin="0.4s" repeatCount="indefinite"/>
    </use>
    <!-- Stream 9 -->
    <use xlink:href="#rainDrop" x="1280" y="0">
      <animateTransform attributeName="transform" type="translate" values="0,-100; -80,600" dur="1.05s" begin="0.8s" repeatCount="indefinite"/>
    </use>
    <!-- Stream 10 -->
    <use xlink:href="#rainDrop" x="1440" y="0">
      <animateTransform attributeName="transform" type="translate" values="0,-100; -80,600" dur="1.15s" begin="0.15s" repeatCount="indefinite"/>
    </use>
    <!-- Stream 11 -->
    <use xlink:href="#rainDrop" x="1560" y="0">
      <animateTransform attributeName="transform" type="translate" values="0,-100; -80,600" dur="1.35s" begin="0.45s" repeatCount="indefinite"/>
    </use>
  </g>

  <!-- ================= 9. FOREGROUND SCANLINE & VIGNETTE EFFECT ================= -->
  <!-- Subtle CRT Vignette Overlay -->
  <rect width="1600" height="500" fill="none" stroke="#00E5FF" stroke-width="2" opacity="0.3"/>
</svg>
