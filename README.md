<svg viewBox="0 0 1180 610" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
  <defs>
    <!-- Background Gradients -->
    <linearGradient id="bgGradDark" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#030712" />
      <stop offset="50%" stop-color="#0F172A" />
      <stop offset="100%" stop-color="#030712" />
    </linearGradient>

    <radialGradient id="glowBlue" cx="20%" cy="20%" r="60%">
      <stop offset="0%" stop-color="#3B82F6" stop-opacity="0.15" />
      <stop offset="100%" stop-color="#030712" stop-opacity="0" />
    </radialGradient>

    <radialGradient id="glowPurple" cx="80%" cy="80%" r="50%">
      <stop offset="0%" stop-color="#8B5CF6" stop-opacity="0.15" />
      <stop offset="100%" stop-color="#030712" stop-opacity="0" />
    </radialGradient>

    <radialGradient id="glowEmerald" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#10B981" stop-opacity="0.1" />
      <stop offset="100%" stop-color="#030712" stop-opacity="0" />
    </radialGradient>

    <!-- ASCII Gradient -->
    <linearGradient id="asciiGradDark" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#06B6D4" />
      <stop offset="50%" stop-color="#8B5CF6" />
      <stop offset="100%" stop-color="#EC4899" />
      <animate attributeName="x1" values="0%;100%;0%" dur="8s" repeatCount="indefinite" />
      <animate attributeName="x2" values="100%;0%;100%" dur="8s" repeatCount="indefinite" />
    </linearGradient>

    <!-- Accent Gradients -->
    <linearGradient id="accentGradDark" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#7C3AED" />
      <stop offset="50%" stop-color="#22D3EE" />
      <stop offset="100%" stop-color="#10B981" />
    </linearGradient>

    <linearGradient id="pillGradDark" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="rgba(124, 58, 237, 0.2)" />
      <stop offset="100%" stop-color="rgba(34, 211, 238, 0.1)" />
    </linearGradient>

    <!-- Glass Panel Gradients -->
    <linearGradient id="panelGradDark" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="rgba(15, 23, 42, 0.8)" />
      <stop offset="100%" stop-color="rgba(15, 23, 42, 0.4)" />
    </linearGradient>

    <linearGradient id="borderGradDark" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="rgba(255, 255, 255, 0.12)" />
      <stop offset="50%" stop-color="rgba(255, 255, 255, 0.05)" />
      <stop offset="100%" stop-color="rgba(255, 255, 255, 0.12)" />
    </linearGradient>

    <!-- Glass Reflection -->
    <linearGradient id="reflectionGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="rgba(255, 255, 255, 0.1)" />
      <stop offset="40%" stop-color="rgba(255, 255, 255, 0)" />
    </linearGradient>

    <!-- Filters -->
    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="6" result="blur" />
      <feMerge>
        <feMergeNode in="blur" />
        <feMergeNode in="SourceGraphic" />
      </feMerge>
    </filter>

    <filter id="softGlow" x="-10%" y="-10%" width="120%" height="120%">
      <feGaussianBlur stdDeviation="3" result="blur" />
      <feMerge>
        <feMergeNode in="blur" />
        <feMergeNode in="SourceGraphic" />
      </feMerge>
    </filter>

    <filter id="noise">
      <feTurbulence type="fractalNoise" baseFrequency="0.65" numOctaves="3" stitchTiles="stitch" />
      <feColorMatrix type="matrix" values="1 0 0 0 0, 0 1 0 0 0, 0 0 1 0 0, 0 0 0 0.04 0" />
    </filter>

    <filter id="dropShadow">
      <feDropShadow dx="0" dy="10" stdDeviation="15" flood-color="#000000" flood-opacity="0.5" />
    </filter>

    <!-- Masks for Typing Effect -->
    <mask id="mask-word1">
      <rect x="520" y="150" width="0" height="30" fill="white">
        <animate attributeName="width" from="0" to="260" begin="1.5s" dur="1.5s" fill="freeze" />
        <animate attributeName="width" to="0" begin="4.5s" dur="0.5s" fill="freeze" />
      </rect>
    </mask>

    <mask id="mask-word2">
      <rect x="520" y="150" width="0" height="30" fill="white">
        <animate attributeName="width" from="0" to="280" begin="5s" dur="1.5s" fill="freeze" />
        <animate attributeName="width" to="0" begin="8s" dur="0.5s" fill="freeze" />
      </rect>
    </mask>

    <mask id="mask-word3">
      <rect x="520" y="150" width="0" height="30" fill="white">
        <animate attributeName="width" from="0" to="160" begin="8.5s" dur="1.5s" fill="freeze" />
        <animate attributeName="width" to="0" begin="11.5s" dur="0.5s" fill="freeze" />
      </rect>
    </mask>

    <mask id="mask-word4">
      <rect x="520" y="150" width="0" height="30" fill="white">
        <animate attributeName="width" from="0" to="200" begin="12s" dur="1.5s" fill="freeze" />
        <animate attributeName="width" to="0" begin="15s" dur="0.5s" fill="freeze" />
      </rect>
    </mask>

    <!-- Scanline Pattern -->
    <pattern id="scanlines" width="4" height="4" patternUnits="userSpaceOnUse">
      <rect width="4" height="2" fill="transparent" />
      <rect y="2" width="4" height="2" fill="rgba(0, 0, 0, 0.08)" />
    </pattern>
  </defs>

  <!-- Background Layer -->
  <rect width="1180" height="610" rx="24" fill="url(#bgGradDark)" />
  
  <!-- Floating Background Glows -->
  <circle cx="200" cy="150" r="150" fill="url(#glowBlue)" opacity="0.6">
    <animateTransform attributeName="transform" type="translate" values="0,0; 20,30; 0,0" dur="10s" repeatCount="indefinite" />
  </circle>
  <circle cx="1000" cy="450" r="200" fill="url(#glowPurple)" opacity="0.6">
    <animateTransform attributeName="transform" type="translate" values="0,0; -30,-20; 0,0" dur="12s" repeatCount="indefinite" />
  </circle>
  <circle cx="600" cy="300" r="180" fill="url(#glowEmerald)" opacity="0.4">
    <animateTransform attributeName="transform" type="translate" values="0,0; -10,20; 0,0" dur="8s" repeatCount="indefinite" />
  </circle>

  <!-- Floating Particles -->
  <g fill="#7C3AED" opacity="0.6">
    <circle cx="100" cy="200" r="2">
      <animate attributeName="cy" values="200;180;200" dur="4s" repeatCount="indefinite" />
      <animate attributeName="opacity" values="0.6;0.2;0.6" dur="4s" repeatCount="indefinite" />
    </circle>
    <circle cx="300" cy="500" r="1.5">
      <animate attributeName="cy" values="500;480;500" dur="5s" repeatCount="indefinite" />
      <animate attributeName="opacity" values="0.4;0.1;0.4" dur="5s" repeatCount="indefinite" />
    </circle>
    <circle cx="850" cy="150" r="2">
      <animate attributeName="cy" values="150;130;150" dur="3.5s" repeatCount="indefinite" />
      <animate attributeName="opacity" values="0.5;0.1;0.5" dur="3.5s" repeatCount="indefinite" />
    </circle>
    <circle cx="1100" cy="350" r="1.5">
      <animate attributeName="cy" values="350;330;350" dur="6s" repeatCount="indefinite" />
      <animate attributeName="opacity" values="0.7;0.3;0.7" dur="6s" repeatCount="indefinite" />
    </circle>
  </g>

  <!-- Left Panel (ASCII Portrait) -->
  <g transform="translate(40, 40)">
    <!-- Glass Panel -->
    <rect width="420" height="530" rx="16" fill="url(#panelGradDark)" stroke="url(#borderGradDark)" stroke-width="1" filter="url(#dropShadow)" />
    <path d="M0,0 L420,0 L0,530 Z" fill="url(#reflectionGrad)" opacity="0.6" rx="16" />
    
    <!-- Terminal Header Dots -->
    <circle cx="16" cy="20" r="6" fill="#EF4444" />
    <circle cx="38" cy="20" r="6" fill="#F59E0B" />
    <circle cx="60" cy="20" r="6" fill="#10B981" />

    <!-- ASCII Art Block -->
    <g font-family="'Courier New', Courier, monospace" font-size="14" fill="url(#asciiGradDark)">
      <text x="30" y="60">
        <tspan x="30" dy="0" opacity="0">              ,------------------------,<animate attributeName="opacity" from="0" to="1" begin="0.1s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">             /   _______________   ____/|<animate attributeName="opacity" from="0" to="1" begin="0.25s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">            /   /              /| /   / |<animate attributeName="opacity" from="0" to="1" begin="0.4s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">           (   (  O         O  ( |/   /  )<animate attributeName="opacity" from="0" to="1" begin="0.55s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">           |    \  _______  /  |/   /   |<animate attributeName="opacity" from="0" to="1" begin="0.7s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">           |     \ \     / /   /   /    |<animate attributeName="opacity" from="0" to="1" begin="0.85s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">           |      \ `. ,' /   /   /     |<animate attributeName="opacity" from="0" to="1" begin="1.0s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">           |       \ `-' /   /   /      |<animate attributeName="opacity" from="0" to="1" begin="1.15s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">           |        \___/   /   /       |<animate attributeName="opacity" from="0" to="1" begin="1.3s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">           |               /   /        |<animate attributeName="opacity" from="0" to="1" begin="1.45s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">           |    SAQLAIN   /   /         |<animate attributeName="opacity" from="0" to="1" begin="1.6s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">           |     CS      /   /          |<animate attributeName="opacity" from="0" to="1" begin="1.75s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">           |            /   /           |<animate attributeName="opacity" from="0" to="1" begin="1.9s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">           |___________/   /            |<animate attributeName="opacity" from="0" to="1" begin="2.05s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">           |_______________/            |<animate attributeName="opacity" from="0" to="1" begin="2.2s" dur="0.15s" fill="freeze" /></tspan>
        <tspan x="30" dy="18" opacity="0">            \__________________________\<animate attributeName="opacity" from="0" to="1" begin="2.35s" dur="0.15s" fill="freeze" /></tspan>
      </text>
      
      <!-- Blinking Cursor -->
      <rect x="280" y="358" width="8" height="16" fill="#22D3EE" opacity="1">
        <animate attributeName="opacity" values="1;0;1" dur="0.8s" repeatCount="indefinite" />
      </rect>
    </g>

    <!-- Float Animation for ASCII Block -->
    <animateTransform attributeName="transform" type="translate" values="0,0; 0,-8; 0,0; 0,8; 0,0" dur="6s" repeatCount="indefinite" />
  </g>

  <!-- Right Panel (Professional Terminal) -->
  <g transform="translate(490, 40)">
    <!-- Glass Panel -->
    <rect width="650" height="530" rx="16" fill="url(#panelGradDark)" stroke="url(#borderGradDark)" stroke-width="1" filter="url(#dropShadow)" />
    <path d="M0,0 L650,0 L0,530 Z" fill="url(#reflectionGrad)" opacity="0.6" rx="16" />

    <!-- Terminal Header Dots -->
    <circle cx="16" cy="20" r="6" fill="#EF4444" />
    <circle cx="38" cy="20" r="6" fill="#F59E0B" />
    <circle cx="60" cy="20" r="6" fill="#10B981" />

    <!-- Greeting Section -->
    <g font-family="system-ui, -apple-system, sans-serif">
      <text x="30" y="80" font-size="18" fill="#94A3B8" opacity="0">
        Hi 👋
        <animate attributeName="opacity" from="0" to="1" begin="0.5s" dur="0.5s" fill="freeze" />
      </text>
      
      <text x="30" y="120" font-size="32" font-weight="bold" fill="#F8FAFC" opacity="0">
        I'm MOHAMMED SAQLAIN
        <animate attributeName="opacity" from="0" to="1" begin="1.0s" dur="0.5s" fill="freeze" />
      </text>

      <!-- Animated Typing Text -->
      <!-- Word 1 -->
      <text x="30" y="170" font-size="20" font-weight="600" fill="url(#accentGradDark)" mask="url(#mask-word1)">Full Stack Developer</text>
      <!-- Word 2 -->
      <text x="30" y="170" font-size="20" font-weight="600" fill="url(#accentGradDark)" mask="url(#mask-word2)">Open Source Contributor</text>
      <!-- Word 3 -->
      <text x="30" y="170" font-size="20" font-weight="600" fill="url(#accentGradDark)" mask="url(#mask-word3)">UI Engineer</text>
      <!-- Word 4 -->
      <text x="30" y="170" font-size="20" font-weight="600" fill="url(#accentGradDark)" mask="url(#mask-word4)">AI Enthusiast</text>

      <!-- Typing Cursor -->
      <rect x="295" y="152" width="3" height="22" fill="#F8FAFC" opacity="1">
        <animate attributeName="opacity" values="1;0;1" dur="0.8s" repeatCount="indefinite" />
        <!-- Move cursor with words -->
        <animate attributeName="x" values="295;555;295;575;295;455;295;495" dur="13.5s" repeatCount="indefinite" />
      </rect>
      
      <rect x="295" y="152" width="3" height="22" fill="#F8FAFC" opacity="0">
        <animate attributeName="opacity" values="0;0;1;0;0;1;0;0;1;0;0;1;0" dur="13.5s" repeatCount="indefinite" />
      </rect>

      <!-- Details Section -->
      <g font-size="16" fill="#94A3B8" font-weight="normal">
        <!-- Location -->
        <text x="30" y="230" opacity="0">
          📍 Location: INDIA
          <animate attributeName="opacity" from="0" to="1" begin="2.5s" dur="0.5s" fill="freeze" />
        </text>
        <!-- Education -->
        <text x="30" y="260" opacity="0">
          🎓 Education: BTech CSE
          <animate attributeName="opacity" from="0" to="1" begin="3.0s" dur="0.5s" fill="freeze" />
        </text>
        <!-- Focus -->
        <text x="30" y="290" opacity="0">
          🚀 Current Focus: enterprise level development
          <animate attributeName="opacity" from="0" to="1" begin="3.5s" dur="0.5s" fill="freeze" />
        </text>
        <!-- Portfolio -->
        <text x="30" y="320" opacity="0">
          🌐 Portfolio: soon
          <animate attributeName="opacity" from="0" to="1" begin="4.0s" dur="0.5s" fill="freeze" />
        </text>
        <!-- Email -->
        <text x="30" y="350" opacity="0">
          ✉️ Email: mohammed.saqlain.cs@gmail.com
          <animate attributeName="opacity" from="0" to="1" begin="4.5s" dur="0.5s" fill="freeze" />
        </text>
      </g>

      <!-- Skills Section -->
      <g opacity="0">
        <animate attributeName="opacity" from="0" to="1" begin="5.5s" dur="0.5s" fill="freeze" />
        <text x="30" y="400" font-size="18" font-weight="bold" fill="#F8FAFC">⚡ Skills</text>
        
        <!-- Row 1 -->
        <g transform="translate(30, 420)">
          <!-- React -->
          <g>
            <animateTransform attributeName="transform" type="scale" from="1,1" to="1.1,1.1" begin="mouseover" dur="0.2s" fill="freeze" additive="sum"/>
            <animateTransform attributeName="transform" type="scale" from="1.1,1.1" to="1,1" begin="mouseout" dur="0.2s" fill="freeze" additive="sum"/>
            <rect width="85" height="30" rx="8" fill="url(#pillGradDark)" stroke="rgba(124, 58, 237, 0.5)" stroke-width="1" />
            <rect width="85" height="30" rx="8" fill="url(#accentGradDark)" opacity="0" filter="url(#glow)">
              <animate attributeName="opacity" to="0.5" begin="mouseover" dur="0.2s" fill="freeze" />
              <animate attributeName="opacity" to="0" begin="mouseout" dur="0.2s" fill="freeze" />
            </rect>
            <text x="42.5" y="20" font-size="12" fill="#E2E8F0" text-anchor="middle" font-family="system-ui">React</text>
          </g>
          <!-- Spring Boot -->
          <g transform="translate(105, 0)">
            <animateTransform attributeName="transform" type="scale" from="1,1" to="1.1,1.1" begin="mouseover" dur="0.2s" fill="freeze" additive="sum"/>
            <animateTransform attributeName="transform" type="scale" from="1.1,1.1" to="1,1" begin="mouseout" dur="0.2s" fill="freeze" additive="sum"/>
            <rect width="105" height="30" rx="8" fill="url(#pillGradDark)" stroke="rgba(124, 58, 237, 0.5)" stroke-width="1" />
            <rect width="105" height="30" rx="8" fill="url(#accentGradDark)" opacity="0" filter="url(#glow)">
              <animate attributeName="opacity" to="0.5" begin="mouseover" dur="0.2s" fill="freeze" />
              <animate attributeName="opacity" to="0" begin="mouseout" dur="0.2s" fill="freeze" />
            </rect>
            <text x="52.5" y="20" font-size="12" fill="#E2E8F0" text-anchor="middle" font-family="system-ui">Spring Boot</text>
          </g>
          <!-- Node.js -->
          <g transform="translate(230, 0)">
            <animateTransform attributeName="transform" type="scale" from="1,1" to="1.1,1.1" begin="mouseover" dur="0.2s" fill="freeze" additive="sum"/>
            <animateTransform attributeName="transform" type="scale" from="1.1,1.1" to="1,1" begin="mouseout" dur="0.2s" fill="freeze" additive="sum"/>
            <rect width="85" height="30" rx="8" fill="url(#pillGradDark)" stroke="rgba(124, 58, 237, 0.5)" stroke-width="1" />
            <rect width="85" height="30" rx="8" fill="url(#accentGradDark)" opacity="0" filter="url(#glow)">
              <animate attributeName="opacity" to="0.5" begin="mouseover" dur="0.2s" fill="freeze" />
              <animate attributeName="opacity" to="0" begin="mouseout" dur="0.2s" fill="freeze" />
            </rect>
            <text x="42.5" y="20" font-size="12" fill="#E2E8F0" text-anchor="middle" font-family="system-ui">Node.js</text>
          </g>
          <!-- TypeScript -->
          <g transform="translate(335, 0)">
            <animateTransform attributeName="transform" type="scale" from="1,1" to="1.1,1.1" begin="mouseover" dur="0.2s" fill="freeze" additive="sum"/>
            <animateTransform attributeName="transform" type="scale" from="1.1,1.1" to="1,1" begin="mouseout" dur="0.2s" fill="freeze" additive="sum"/>
            <rect width="95" height="30" rx="8" fill="url(#pillGradDark)" stroke="rgba(124, 58, 237, 0.5)" stroke-width="1" />
            <rect width="95" height="30" rx="8" fill="url(#accentGradDark)" opacity="0" filter="url(#glow)">
              <animate attributeName="opacity" to="0.5" begin="mouseover" dur="0.2s" fill="freeze" />
              <animate attributeName="opacity" to="0" begin="mouseout" dur="0.2s" fill="freeze" />
            </rect>
            <text x="47.5" y="20" font-size="12" fill="#E2E8F0" text-anchor="middle" font-family="system-ui">TypeScript</text>
          </g>
        </g>

        <!-- Row 2 -->
        <g transform="translate(30, 460)">
          <g>
            <animateTransform attributeName="transform" type="scale" from="1,1" to="1.1,1.1" begin="mouseover" dur="0.2s" fill="freeze" additive="sum"/>
            <animateTransform attributeName="transform" type="scale" from="1.1,1.1" to="1,1" begin="mouseout" dur="0.2s" fill="freeze" additive="sum"/>
            <rect width="85" height="30" rx="8" fill="url(#pillGradDark)" stroke="rgba(124, 58, 237, 0.5)" stroke-width="1" />
            <rect width="85" height="30" rx="8" fill="url(#accentGradDark)" opacity="0" filter="url(#glow)">
              <animate attributeName="opacity" to="0.5" begin="mouseover" dur="0.2s" fill="freeze" />
              <animate attributeName="opacity" to="0" begin="mouseout" dur="0.2s" fill="freeze" />
            </rect>
            <text x="42.5" y="20" font-size="12" fill="#E2E8F0" text-anchor="middle" font-family="system-ui">Tailwind</text>
          </g>
          <g transform="translate(105, 0)">
            <animateTransform attributeName="transform" type="scale" from="1,1" to="1.1,1.1" begin="mouseover" dur="0.2s" fill="freeze" additive="sum"/>
            <animateTransform attributeName="transform" type="scale" from="1.1,1.1" to="1,1" begin="mouseout" dur="0.2s" fill="freeze" additive="sum"/>
            <rect width="75" height="30" rx="8" fill="url(#pillGradDark)" stroke="rgba(124, 58, 237, 0.5)" stroke-width="1" />
            <rect width="75" height="30" rx="8" fill="url(#accentGradDark)" opacity="0" filter="url(#glow)">
              <animate attributeName="opacity" to="0.5" begin="mouseover" dur="0.2s" fill="freeze" />
              <animate attributeName="opacity" to="0" begin="mouseout" dur="0.2s" fill="freeze" />
            </rect>
            <text x="37.5" y="20" font-size="12" fill="#E2E8F0" text-anchor="middle" font-family="system-ui">Python</text>
          </g>
          <g transform="translate(200, 0)">
            <animateTransform attributeName="transform" type="scale" from="1,1" to="1.1,1.1" begin="mouseover" dur="0.2s" fill="freeze" additive="sum"/>
            <animateTransform attributeName="transform" type="scale" from="1.1,1.1" to="1,1" begin="mouseout" dur="0.2s" fill="freeze" additive="sum"/>
            <rect width="80" height="30" rx="8" fill="url(#pillGradDark)" stroke="rgba(124, 58, 237, 0.5)" stroke-width="1" />
            <rect width="80" height="30" rx="8" fill="url(#accentGradDark)" opacity="0" filter="url(#glow)">
              <animate attributeName="opacity" to="0.5" begin="mouseover" dur="0.2s" fill="freeze" />
              <animate attributeName="opacity" to="0" begin="mouseout" dur="0.2s" fill="freeze" />
            </rect>
            <text x="40" y="20" font-size="12" fill="#E2E8F0" text-anchor="middle" font-family="system-ui">Docker</text>
          </g>
          <g transform="translate(300, 0)">
            <animateTransform attributeName="transform" type="scale" from="1,1" to="1.1,1.1" begin="mouseover" dur="0.2s" fill="freeze" additive="sum"/>
            <animateTransform attributeName="transform" type="scale" from="1.1,1.1" to="1,1" begin="mouseout" dur="0.2s" fill="freeze" additive="sum"/>
            <rect width="95" height="30" rx="8" fill="url(#pillGradDark)" stroke="rgba(124, 58, 237, 0.5)" stroke-width="1" />
            <rect width="95" height="30" rx="8" fill="url(#accentGradDark)" opacity="0" filter="url(#glow)">
              <animate attributeName="opacity" to="0.5" begin="mouseover" dur="0.2s" fill="freeze" />
              <animate attributeName="opacity" to="0" begin="mouseout" dur="0.2s" fill="freeze" />
            </rect>
            <text x="47.5" y="20" font-size="12" fill="#E2E8F0" text-anchor="middle" font-family="system-ui">MongoDB</text>
          </g>
        </g>

        <!-- Row 3 -->
        <g transform="translate(30, 500)">
          <g>
            <animateTransform attributeName="transform" type="scale" from="1,1" to="1.1,1.1" begin="mouseover" dur="0.2s" fill="freeze" additive="sum"/>
            <animateTransform attributeName="transform" type="scale" from="1.1,1.1" to="1,1" begin="mouseout" dur="0.2s" fill="freeze" additive="sum"/>
            <rect width="85" height="30" rx="8" fill="url(#pillGradDark)" stroke="rgba(124, 58, 237, 0.5)" stroke-width="1" />
            <rect width="85" height="30" rx="8" fill="url(#accentGradDark)" opacity="0" filter="url(#glow)">
              <animate attributeName="opacity" to="0.5" begin="mouseover" dur="0.2s" fill="freeze" />
              <animate attributeName="opacity" to="0" begin="mouseout" dur="0.2s" fill="freeze" />
            </rect>
            <text x="42.5" y="20" font-size="12" fill="#E2E8F0" text-anchor="middle" font-family="system-ui">Postgres</text>
          </g>
          <g transform="translate(105, 0)">
            <animateTransform attributeName="transform" type="scale" from="1,1" to="1.1,1.1" begin="mouseover" dur="0.2s" fill="freeze" additive="sum"/>
            <animateTransform attributeName="transform" type="scale" from="1.1,1.1" to="1,1" begin="mouseout" dur="0.2s" fill="freeze" additive="sum"/>
            <rect width="65" height="30" rx="8" fill="url(#pillGradDark)" stroke="rgba(124, 58, 237, 0.5)" stroke-width="1" />
            <rect width="65" height="30" rx="8" fill="url(#accentGradDark)" opacity="0" filter="url(#glow)">
              <animate attributeName="opacity" to="0.5" begin="mouseover" dur="0.2s" fill="freeze" />
              <animate attributeName="opacity" to="0" begin="mouseout" dur="0.2s" fill="freeze" />
            </rect>
            <text x="32.5" y="20" font-size="12" fill="#E2E8F0" text-anchor="middle" font-family="system-ui">AWS</text>
          </g>
          <g transform="translate(190, 0)">
            <animateTransform attributeName="transform" type="scale" from="1,1" to="1.1,1.1" begin="mouseover" dur="0.2s" fill="freeze" additive="sum"/>
            <animateTransform attributeName="transform" type="scale" from="1.1,1.1" to="1,1" begin="mouseout" dur="0.2s" fill="freeze" additive="sum"/>
            <rect width="55" height="30" rx="8" fill="url(#pillGradDark)" stroke="rgba(124, 58, 237, 0.5)" stroke-width="1" />
            <rect width="55" height="30" rx="8" fill="url(#accentGradDark)" opacity="0" filter="url(#glow)">
              <animate attributeName="opacity" to="0.5" begin="mouseover" dur="0.2s" fill="freeze" />
              <animate attributeName="opacity" to="0" begin="mouseout" dur="0.2s" fill="freeze" />
            </rect>
            <text x="27.5" y="20" font-size="12" fill="#E2E8F0" text-anchor="middle" font-family="system-ui">Git</text>
          </g>
        </g>
      </g>
    </g>
  </g>

  <!-- Social Icons (Bottom Right) -->
  <g transform="translate(490, 40)" font-family="system-ui, -apple-system, sans-serif">
    <g opacity="0">
      <animate attributeName="opacity" from="0" to="1" begin="6.5s" dur="0.5s" fill="freeze" />
      
      <!-- GitHub -->
      <a href="https://github.com/mohammedsaqlain" target="_blank">
        <g transform="translate(530, 510)">
          <rect x="-15" y="-15" width="30" height="30" rx="8" fill="transparent" />
          <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z" fill="#94A3B8" filter="url(#softGlow)">
            <animate attributeName="fill" values="#94A3B8;#22D3EE;#94A3B8" dur="3s" repeatCount="indefinite" />
          </path>
        </g>
      </a>

      <!-- LinkedIn -->
      <a href="https://linkedin.com/in/mohammedsaqlain" target="_blank">
        <g transform="translate(590, 510)">
          <rect x="-15" y="-15" width="30" height="30" rx="8" fill="transparent" />
          <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z" fill="#94A3B8" filter="url(#softGlow)">
            <animate attributeName="fill" values="#94A3B8;#A78BFA;#94A3B8" dur="4s" repeatCount="indefinite" />
          </path>
        </g>
      </a>

      <!-- Twitter -->
      <a href="https://twitter.com/mohammedsaqlain" target="_blank">
        <g transform="translate(650, 510)">
          <rect x="-15" y="-15" width="30" height="30" rx="8" fill="transparent" />
          <path d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z" fill="#94A3B8" filter="url(#softGlow)">
            <animate attributeName="fill" values="#94A3B8;#06B6D4;#94A3B8" dur="3.5s" repeatCount="indefinite" />
          </path>
        </g>
      </a>

      <!-- Portfolio -->
      <a href="https://mohammedsaqlain.vercel.app" target="_blank">
        <g transform="translate(710, 510)">
          <rect x="-15" y="-15" width="30" height="30" rx="8" fill="transparent" />
          <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 17.93c-3.95-.49-7-3.85-7-7.93 0-.62.08-1.21.21-1.79L9 15v1c0 1.1.9 2 2 2v1.93zm6.9-2.54c-.26-.81-1-1.39-1.9-1.39h-1v-3c0-.55-.45-1-1-1H8v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41c2.93 1.19 5 4.06 5 7.41 0 2.08-.8 3.97-2.1 5.39z" fill="#94A3B8" filter="url(#softGlow)">
            <animate attributeName="fill" values="#94A3B8;#10B981;#94A3B8" dur="4.5s" repeatCount="indefinite" />
          </path>
        </g>
      </a>
    </g>
  </g>

  <!-- Border Shimmer Effect -->
  <rect x="1" y="1" width="1178" height="608" rx="23" fill="none" stroke="url(#borderGradDark)" stroke-width="2" stroke-dasharray="20 40" stroke-dashoffset="0" opacity="0.5">
    <animate attributeName="stroke-dashoffset" from="0" to="-600" dur="15s" repeatCount="indefinite" />
  </rect>

  <!-- Scanline Overlay -->
  <rect width="1180" height="610" rx="24" fill="url(#scanlines)" pointer-events="none" />
  
  <!-- Noise Texture Overlay -->
  <rect width="1180" height="610" rx="24" filter="url(#noise)" pointer-events="none" />
</svg>