<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Dhineshkumar G — Dark Theme Preview</title>
<style>
  html, body {
    margin: 0;
    padding: 0;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #05070d;
    font-family: -apple-system, Segoe UI, sans-serif;
  }
  .wrap {
    padding: 40px 20px;
    text-align: center;
  }
  .banner {
    max-width: 1180px;
    width: 100%;
    height: auto;
    display: block;
    margin: 0 auto;
  }
  .caption {
    margin-top: 16px;
    color: #64748b;
    font-size: 13px;
    font-family: SFMono-Regular, Consolas, monospace;
  }
</style>
</head>
<body>
<div class="wrap">
  <div class="banner">
<svg width="1180" height="610" viewBox="0 0 1180 610" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<defs>
  <!-- ============ GRADIENTS ============ -->
  <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
    <stop offset="0%" stop-color="#030712"/>
    <stop offset="100%" stop-color="#050B18"/>
  </linearGradient>

  <linearGradient id="accentGrad" x1="0%" y1="0%" x2="100%" y2="0%">
    <stop offset="0%" stop-color="#7C3AED"/>
    <stop offset="50%" stop-color="#22D3EE"/>
    <stop offset="100%" stop-color="#10B981"/>
    <animateTransform attributeName="gradientTransform" type="translate"
      values="-0.4 0; 0.4 0; -0.4 0" dur="6s" repeatCount="indefinite"/>
  </linearGradient>

  <linearGradient id="asciiGrad" x1="0%" y1="0%" x2="100%" y2="100%">
    <stop offset="0%" stop-color="#22D3EE"/>
    <stop offset="50%" stop-color="#7C3AED"/>
    <stop offset="100%" stop-color="#22D3EE"/>
    <animateTransform attributeName="gradientTransform" type="rotate"
      values="0 0.5 0.5; 360 0.5 0.5" dur="8s" repeatCount="indefinite"/>
  </linearGradient>

  <linearGradient id="borderShimmer" x1="0%" y1="0%" x2="100%" y2="0%">
    <stop offset="0%" stop-color="rgba(255,255,255,0)"/>
    <stop offset="45%" stop-color="rgba(255,255,255,0)"/>
    <stop offset="50%" stop-color="rgba(124,58,237,0.9)"/>
    <stop offset="55%" stop-color="rgba(255,255,255,0)"/>
    <stop offset="100%" stop-color="rgba(255,255,255,0)"/>
    <animateTransform attributeName="gradientTransform" type="translate"
      values="-2 0; 2 0; -2 0" dur="5s" repeatCount="indefinite"/>
  </linearGradient>

  <radialGradient id="glowPurple" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#7C3AED" stop-opacity="0.35"/>
    <stop offset="100%" stop-color="#7C3AED" stop-opacity="0"/>
  </radialGradient>
  <radialGradient id="glowCyan" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#22D3EE" stop-opacity="0.30"/>
    <stop offset="100%" stop-color="#22D3EE" stop-opacity="0"/>
  </radialGradient>
  <radialGradient id="glowEmerald" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#10B981" stop-opacity="0.22"/>
    <stop offset="100%" stop-color="#10B981" stop-opacity="0"/>
  </radialGradient>

  <!-- ============ FILTERS ============ -->
  <filter id="glow" x="-60%" y="-60%" width="220%" height="220%">
    <feGaussianBlur stdDeviation="3.2" result="blur"/>
    <feMerge>
      <feMergeNode in="blur"/>
      <feMergeNode in="SourceGraphic"/>
    </feMerge>
  </filter>

  <filter id="softGlow" x="-80%" y="-80%" width="260%" height="260%">
    <feGaussianBlur stdDeviation="6" result="blur"/>
    <feMerge>
      <feMergeNode in="blur"/>
      <feMergeNode in="SourceGraphic"/>
    </feMerge>
  </filter>

  <filter id="noiseFilter" x="0" y="0" width="100%" height="100%">
    <feTurbulence type="fractalNoise" baseFrequency="0.85" numOctaves="2" stitchTiles="stitch" result="noise"/>
    <feColorMatrix in="noise" type="matrix"
      values="0 0 0 0 1  0 0 0 0 1  0 0 0 0 1  0 0 0 0.02 0"/>
  </filter>

  <clipPath id="roundedCanvas">
    <rect x="0" y="0" width="1180" height="610" rx="26"/>
  </clipPath>
  <clipPath id="leftPanelClip">
    <rect x="24" y="24" width="410" height="562" rx="18"/>
  </clipPath>
  <clipPath id="rightPanelClip">
    <rect x="458" y="24" width="698" height="562" rx="18"/>
  </clipPath>
</defs>

<g clip-path="url(#roundedCanvas)">
  <!-- BACKGROUND -->
  <rect x="0" y="0" width="1180" height="610" fill="url(#bgGrad)"/>
  <rect x="0" y="0" width="1180" height="610" filter="url(#noiseFilter)"/>

  <!-- floating background glows -->
  <circle cx="150" cy="120" r="180" fill="url(#glowPurple)">
    <animate attributeName="cx" values="150;220;150" dur="14s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="120;180;120" dur="16s" repeatCount="indefinite"/>
  </circle>
  <circle cx="1000" cy="480" r="220" fill="url(#glowCyan)">
    <animate attributeName="cx" values="1000;900;1000" dur="18s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="480;420;480" dur="15s" repeatCount="indefinite"/>
  </circle>
  <circle cx="700" cy="60" r="160" fill="url(#glowEmerald)">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="10s" repeatCount="indefinite"/>
  </circle>

  <!-- outer border shimmer -->
  <rect x="1.5" y="1.5" width="1177" height="607" rx="25" fill="none"
    stroke="rgba(255,255,255,0.08)" stroke-width="1.4"/>
  <rect x="1.5" y="1.5" width="1177" height="607" rx="25" fill="none"
    stroke="url(#borderShimmer)" stroke-width="1.6"/>

  <!-- tiny floating particles -->
  <g fill="#22D3EE">
    <circle r="1.6" opacity="0.7">
      <animateMotion path="M120,500 C 300,420 500,540 700,460 S 1000,420 1080,500" dur="20s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.2;0.9;0.2" dur="4s" repeatCount="indefinite"/>
    </circle>
    <circle r="1.2" opacity="0.6" fill="#7C3AED">
      <animateMotion path="M1050,80 C 900,140 750,60 600,120 S 300,180 100,90" dur="24s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.15;0.8;0.15" dur="5s" repeatCount="indefinite"/>
    </circle>
    <circle r="1.4" opacity="0.5" fill="#10B981">
      <animateMotion path="M60,300 C 250,250 400,350 600,300 S 900,260 1120,320" dur="22s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.15;0.7;0.15" dur="6s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- moving scanline (global) -->
  <rect x="0" y="-40" width="1180" height="4" fill="url(#accentGrad)" opacity="0.06">
    <animate attributeName="y" values="-40;650" dur="7s" repeatCount="indefinite"/>
  </rect>

  <!-- =============== LEFT PANEL =============== -->
  <g>
    <rect x="24" y="24" width="410" height="562" rx="18" fill="#0F172A" fill-opacity="0.55" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>
    <g clip-path="url(#leftPanelClip)">
      <!-- glass reflection -->
      <rect x="24" y="24" width="410" height="180" fill="rgba(255,255,255,0.03)"/>

      <text x="52" y="66" font-family="SFMono-Regular, Consolas, monospace" font-size="12" letter-spacing="2" fill="#94A3B8">SYSTEM.PORTRAIT</text>
      <line x1="52" y1="78" x2="382" y2="78" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>

      <!-- floating ascii group -->
      <g font-family="SFMono-Regular, Consolas, 'Courier New', monospace" font-size="17" font-weight="600" fill="url(#asciiGrad)" filter="url(#glow)">
        <animateTransform attributeName="transform" type="translate"
          values="0,0; 0,-7; 0,0" dur="5s" repeatCount="indefinite"/>

        <text x="70" y="150" opacity="0"><tspan>╔══════════════╗</tspan>
          <animate attributeName="opacity" to="1" begin="0.2s" dur="0.01s" fill="freeze"/></text>
        <text x="70" y="175" opacity="0"><tspan>║              ║</tspan>
          <animate attributeName="opacity" to="1" begin="0.5s" dur="0.01s" fill="freeze"/></text>
        <text x="70" y="200" opacity="0"><tspan>║   ┌──────┐   ║</tspan>
          <animate attributeName="opacity" to="1" begin="0.8s" dur="0.01s" fill="freeze"/></text>
        <text x="70" y="225" opacity="0"><tspan>║   │  DG  │   ║</tspan>
          <animate attributeName="opacity" to="1" begin="1.1s" dur="0.01s" fill="freeze"/></text>
        <text x="70" y="250" opacity="0"><tspan>║   └──────┘   ║</tspan>
          <animate attributeName="opacity" to="1" begin="1.4s" dur="0.01s" fill="freeze"/></text>
        <text x="70" y="275" opacity="0"><tspan>║              ║</tspan>
          <animate attributeName="opacity" to="1" begin="1.7s" dur="0.01s" fill="freeze"/></text>
        <text x="70" y="300" opacity="0"><tspan>║  &lt;DEV/&gt;      ║</tspan>
          <animate attributeName="opacity" to="1" begin="2.0s" dur="0.01s" fill="freeze"/></text>
        <text x="70" y="325" opacity="0"><tspan>║  founder;    ║</tspan>
          <animate attributeName="opacity" to="1" begin="2.3s" dur="0.01s" fill="freeze"/></text>
        <text x="70" y="350" opacity="0"><tspan>║  build();    ║</tspan>
          <animate attributeName="opacity" to="1" begin="2.6s" dur="0.01s" fill="freeze"/></text>
        <text x="70" y="375" opacity="0"><tspan>╚══════════════╝</tspan>
          <animate attributeName="opacity" to="1" begin="2.9s" dur="0.01s" fill="freeze"/></text>
      </g>

      <!-- cursor blink under ascii -->
      <rect x="70" y="392" width="10" height="16" fill="#22D3EE" opacity="0">
        <animate attributeName="opacity" begin="3.1s" values="0;1;1;0;0" keyTimes="0;0.01;0.5;0.51;1" dur="1s" repeatCount="indefinite"/>
      </rect>

      <!-- scanline sweep inside portrait -->
      <rect x="52" y="120" width="330" height="3" fill="#22D3EE" opacity="0.18">
        <animate attributeName="y" values="120;400;120" dur="4s" repeatCount="indefinite"/>
      </rect>

      <!-- tagline -->
      <text x="52" y="440" font-family="SFMono-Regular, Consolas, monospace" font-size="13" fill="#94A3B8" opacity="0">
        <animate attributeName="opacity" to="1" begin="3.2s" dur="0.01s" fill="freeze"/>
        root@xerova:~$ whoami
      </text>
      <text x="52" y="462" font-family="SFMono-Regular, Consolas, monospace" font-size="13" fill="#F8FAFC" opacity="0">
        <animate attributeName="opacity" to="1" begin="3.5s" dur="0.01s" fill="freeze"/>
        Digital Architect
      </text>

      <!-- glass reflection diagonal -->
      <polygon points="24,24 130,24 24,220" fill="rgba(255,255,255,0.03)"/>
    </g>
    <rect x="24" y="24" width="410" height="562" rx="18" fill="none" stroke="rgba(124,58,237,0.15)" stroke-width="1"/>
  </g>

  <!-- =============== RIGHT PANEL (terminal) =============== -->
  <g>
    <rect x="458" y="24" width="698" height="562" rx="18" fill="#0F172A" fill-opacity="0.55" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>
    <g clip-path="url(#rightPanelClip)">

      <!-- title bar -->
      <rect x="458" y="24" width="698" height="38" fill="rgba(255,255,255,0.03)"/>
      <circle cx="484" cy="43" r="5.5" fill="#EF4444"/>
      <circle cx="504" cy="43" r="5.5" fill="#F59E0B"/>
      <circle cx="524" cy="43" r="5.5" fill="#10B981"/>
      <text x="1128" y="47" text-anchor="end" font-family="SFMono-Regular, Consolas, monospace" font-size="12" fill="#94A3B8">dhinesh@xerova:~$</text>
      <line x1="458" y1="62" x2="1156" y2="62" stroke="rgba(255,255,255,0.07)" stroke-width="1"/>

      <!-- greeting -->
      <text x="490" y="102" font-family="SFMono-Regular, Consolas, monospace" font-size="20" fill="#F8FAFC" opacity="0">
        <animate attributeName="opacity" to="1" begin="0.3s" dur="0.01s" fill="freeze"/>
        Hi 👋
      </text>
      <text x="490" y="140" font-family="Segoe UI, Inter, sans-serif" font-size="30" font-weight="700" fill="url(#accentGrad)" opacity="0" filter="url(#glow)">
        <animate attributeName="opacity" to="1" begin="0.7s" dur="0.01s" fill="freeze"/>
        I'm Dhineshkumar G
      </text>

      <!-- role rotator -->
      <text x="490" y="172" font-family="SFMono-Regular, Consolas, monospace" font-size="17" fill="#22D3EE" opacity="0">
        <animate attributeName="opacity" to="1" begin="1.1s" dur="0.01s" fill="freeze"/>
        &gt;
      </text>
      <g font-family="SFMono-Regular, Consolas, monospace" font-size="17" fill="#F8FAFC">
        <text x="508" y="172" opacity="0">Founder &amp; CEO, Xerova Digital
          <animate attributeName="opacity" begin="1.2s" dur="8s" values="0;1;1;0;0" keyTimes="0;0.02;0.23;0.25;1" repeatCount="indefinite"/></text>
        <text x="508" y="172" opacity="0">CSBS Engineering Student
          <animate attributeName="opacity" begin="1.2s" dur="8s" values="0;0;1;1;0;0" keyTimes="0;0.25;0.27;0.48;0.5;1" repeatCount="indefinite"/></text>
        <text x="508" y="172" opacity="0">AI / ML &amp; Full-Stack Builder
          <animate attributeName="opacity" begin="1.2s" dur="8s" values="0;0;1;1;0;0" keyTimes="0;0.50;0.52;0.73;0.75;1" repeatCount="indefinite"/></text>
        <text x="508" y="172" opacity="0">Hackathon &amp; Innovation Enthusiast
          <animate attributeName="opacity" begin="1.2s" dur="8s" values="0;0;1;1;0" keyTimes="0;0.75;0.77;0.98;1" repeatCount="indefinite"/></text>
      </g>
      <rect x="785" y="158" width="9" height="16" fill="#22D3EE">
        <animate attributeName="opacity" values="0;1;1;0;0" keyTimes="0;0.01;0.5;0.51;1" dur="1s" repeatCount="indefinite"/>
      </rect>

      <line x1="490" y1="198" x2="1124" y2="198" stroke="rgba(255,255,255,0.06)" stroke-width="1"/>

      <!-- info list -->
      <g font-family="SFMono-Regular, Consolas, monospace" font-size="14">
        <g opacity="0"><animate attributeName="opacity" to="1" begin="1.6s" dur="0.01s" fill="freeze"/>
          <text x="490" y="228" fill="#94A3B8">📍 Location</text>
          <text x="650" y="228" fill="#F8FAFC">Pondicherry, India</text></g>

        <g opacity="0"><animate attributeName="opacity" to="1" begin="1.9s" dur="0.01s" fill="freeze"/>
          <text x="490" y="256" fill="#94A3B8">🎓 Education</text>
          <text x="650" y="256" fill="#F8FAFC">SMVEC · CSBS · Batch 2027</text></g>

        <g opacity="0"><animate attributeName="opacity" to="1" begin="2.2s" dur="0.01s" fill="freeze"/>
          <text x="490" y="284" fill="#94A3B8">⚡ Focus</text>
          <text x="650" y="284" fill="#F8FAFC">Building Xerova Digital Solutions</text></g>

        <g opacity="0"><animate attributeName="opacity" to="1" begin="2.5s" dur="0.01s" fill="freeze"/>
          <text x="490" y="312" fill="#94A3B8">🌐 Portfolio</text>
          <text x="650" y="312" fill="#22D3EE">dhinaportfolio.vercel.app</text></g>

        <g opacity="0"><animate attributeName="opacity" to="1" begin="2.8s" dur="0.01s" fill="freeze"/>
          <text x="490" y="340" fill="#94A3B8">✉️ Email</text>
          <text x="650" y="340" fill="#F8FAFC">your-email@xerovadigitalsolutions.in</text></g>
      </g>

      <line x1="490" y1="362" x2="1124" y2="362" stroke="rgba(255,255,255,0.06)" stroke-width="1"/>
      <text x="490" y="388" font-family="SFMono-Regular, Consolas, monospace" font-size="13" letter-spacing="2" fill="#94A3B8" opacity="0">
        <animate attributeName="opacity" to="1" begin="3.0s" dur="0.01s" fill="freeze"/>
        TECH STACK
      </text>

      <!-- skill pills -->
      <g font-family="Segoe UI, Inter, sans-serif" font-size="13" font-weight="600">
        <!-- row 1 -->
        <g opacity="0"><animate attributeName="opacity" to="1" begin="3.2s" dur="0.01s" fill="freeze"/>
          <rect x="490" y="402" width="88" height="30" rx="15" fill="rgba(124,58,237,0.12)" stroke="#7C3AED" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" repeatCount="indefinite"/></rect>
          <text x="534" y="422" text-anchor="middle" fill="#F8FAFC">React</text></g>

        <g opacity="0"><animate attributeName="opacity" to="1" begin="3.3s" dur="0.01s" fill="freeze"/>
          <rect x="588" y="402" width="92" height="30" rx="15" fill="rgba(34,211,238,0.12)" stroke="#22D3EE" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3.2s" repeatCount="indefinite"/></rect>
          <text x="634" y="422" text-anchor="middle" fill="#F8FAFC">Next.js</text></g>

        <g opacity="0"><animate attributeName="opacity" to="1" begin="3.4s" dur="0.01s" fill="freeze"/>
          <rect x="690" y="402" width="94" height="30" rx="15" fill="rgba(16,185,129,0.12)" stroke="#10B981" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="2.8s" repeatCount="indefinite"/></rect>
          <text x="737" y="422" text-anchor="middle" fill="#F8FAFC">Node.js</text></g>

        <g opacity="0"><animate attributeName="opacity" to="1" begin="3.5s" dur="0.01s" fill="freeze"/>
          <rect x="794" y="402" width="108" height="30" rx="15" fill="rgba(124,58,237,0.12)" stroke="#7C3AED" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3.4s" repeatCount="indefinite"/></rect>
          <text x="848" y="422" text-anchor="middle" fill="#F8FAFC">TypeScript</text></g>

        <g opacity="0"><animate attributeName="opacity" to="1" begin="3.6s" dur="0.01s" fill="freeze"/>
          <rect x="912" y="402" width="100" height="30" rx="15" fill="rgba(34,211,238,0.12)" stroke="#22D3EE" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" repeatCount="indefinite"/></rect>
          <text x="962" y="422" text-anchor="middle" fill="#F8FAFC">Tailwind</text></g>

        <g opacity="0"><animate attributeName="opacity" to="1" begin="3.7s" dur="0.01s" fill="freeze"/>
          <rect x="1022" y="402" width="90" height="30" rx="15" fill="rgba(16,185,129,0.12)" stroke="#10B981" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3.1s" repeatCount="indefinite"/></rect>
          <text x="1067" y="422" text-anchor="middle" fill="#F8FAFC">Python</text></g>

        <!-- row 2 -->
        <g opacity="0"><animate attributeName="opacity" to="1" begin="3.8s" dur="0.01s" fill="freeze"/>
          <rect x="490" y="442" width="90" height="30" rx="15" fill="rgba(124,58,237,0.12)" stroke="#7C3AED" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3.3s" repeatCount="indefinite"/></rect>
          <text x="535" y="462" text-anchor="middle" fill="#F8FAFC">Docker</text></g>

        <g opacity="0"><animate attributeName="opacity" to="1" begin="3.9s" dur="0.01s" fill="freeze"/>
          <rect x="590" y="442" width="80" height="30" rx="15" fill="rgba(34,211,238,0.12)" stroke="#22D3EE" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="2.9s" repeatCount="indefinite"/></rect>
          <text x="630" y="462" text-anchor="middle" fill="#F8FAFC">AWS</text></g>

        <g opacity="0"><animate attributeName="opacity" to="1" begin="4.0s" dur="0.01s" fill="freeze"/>
          <rect x="680" y="442" width="70" height="30" rx="15" fill="rgba(16,185,129,0.12)" stroke="#10B981" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3.2s" repeatCount="indefinite"/></rect>
          <text x="715" y="462" text-anchor="middle" fill="#F8FAFC">Git</text></g>

        <g opacity="0"><animate attributeName="opacity" to="1" begin="4.1s" dur="0.01s" fill="freeze"/>
          <rect x="760" y="442" width="82" height="30" rx="15" fill="rgba(124,58,237,0.12)" stroke="#7C3AED" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" repeatCount="indefinite"/></rect>
          <text x="801" y="462" text-anchor="middle" fill="#F8FAFC">Figma</text></g>
      </g>

      <line x1="490" y1="494" x2="1124" y2="494" stroke="rgba(255,255,255,0.06)" stroke-width="1"/>

      <!-- social icons -->
      <g opacity="0">
        <animate attributeName="opacity" to="1" begin="4.4s" dur="0.01s" fill="freeze"/>

        <g transform="translate(490,516)">
          <circle r="18" fill="rgba(255,255,255,0.04)" stroke="#94A3B8" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke" values="#94A3B8;#22D3EE;#94A3B8" dur="4s" repeatCount="indefinite"/></circle>
          <path d="M0,-9 C-5,-9 -9,-5 -9,0 C-9,4.5 -6,8 -1.8,9 C-1.3,9.1 -1.1,8.8 -1.1,8.5 L-1.1,6.8 C-4,7.4 -4.6,5.5 -4.6,5.5 C-5,4.5 -5.6,4.2 -5.6,4.2 C-6.4,3.7 -5.5,3.7 -5.5,3.7 C-4.6,3.8 -4.1,4.6 -4.1,4.6 C-3.4,5.9 -2.2,5.5 -1.7,5.3 C-1.6,4.8 -1.4,4.4 -1.1,4.2 C-3.4,4 -5.8,3.1 -5.8,-0.8 C-5.8,-1.9 -5.4,-2.8 -4.7,-3.5 C-4.8,-3.7 -5.2,-4.8 -4.6,-6.2 C-4.6,-6.2 -3.7,-6.5 -1.1,-4.7 C0,-5 1.1,-5 2.2,-4.7 C4.8,-6.5 5.7,-6.2 5.7,-6.2 C6.3,-4.8 5.9,-3.7 5.8,-3.5 C6.5,-2.8 6.9,-1.9 6.9,-0.8 C6.9,3.1 4.5,4 2.2,4.2 C2.6,4.5 2.9,5.2 2.9,6.2 L2.9,8.5 C2.9,8.8 3.1,9.1 3.6,9 C7.9,8 10.9,4.5 10.9,0 C10.9,-5 6.9,-9 0,-9 Z" fill="#F8FAFC" transform="scale(0.9)"/>
        </g>

        <g transform="translate(544,516)">
          <circle r="18" fill="rgba(255,255,255,0.04)" stroke="#94A3B8" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke" values="#94A3B8;#7C3AED;#94A3B8" dur="4.4s" repeatCount="indefinite"/></circle>
          <text x="0" y="4" text-anchor="middle" font-family="Segoe UI, sans-serif" font-size="13" font-weight="700" fill="#F8FAFC">in</text>
        </g>

        <g transform="translate(598,516)">
          <circle r="18" fill="rgba(255,255,255,0.04)" stroke="#94A3B8" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke" values="#94A3B8;#22D3EE;#94A3B8" dur="4.8s" repeatCount="indefinite"/></circle>
          <text x="0" y="4" text-anchor="middle" font-family="Segoe UI, sans-serif" font-size="12" font-weight="700" fill="#F8FAFC">X</text>
        </g>

        <g transform="translate(652,516)">
          <circle r="18" fill="rgba(255,255,255,0.04)" stroke="#94A3B8" stroke-width="1" filter="url(#softGlow)">
            <animate attributeName="stroke" values="#94A3B8;#10B981;#94A3B8" dur="4.2s" repeatCount="indefinite"/></circle>
          <text x="0" y="4" text-anchor="middle" font-family="Segoe UI, sans-serif" font-size="11" font-weight="700" fill="#F8FAFC">🌐</text>
        </g>

        <text x="1124" y="521" text-anchor="end" font-family="SFMono-Regular, Consolas, monospace" font-size="12" fill="#94A3B8">github.com/DhineshkumarG</text>
      </g>

    </g>
    <rect x="458" y="24" width="698" height="562" rx="18" fill="none" stroke="rgba(34,211,238,0.15)" stroke-width="1"/>
  </g>
</g>
</svg>

  </div>
  <div class="caption">dark.svg — GitHub profile README preview</div>
</div>
</body>
</html>
