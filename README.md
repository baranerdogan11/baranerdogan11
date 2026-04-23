<svg viewBox="0 0 820 280" width="820" height="280" xmlns="http://www.w3.org/2000/svg">

<defs>

  <!-- GRADIENTS -->
  <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
    <stop offset="0%"   stop-color="#0c0c22"/>
    <stop offset="100%" stop-color="#050510"/>
  </linearGradient>

  <linearGradient id="bottomFade" x1="0" y1="0" x2="0" y2="1">
    <stop offset="55%" stop-color="#07071a" stop-opacity="0"/>
    <stop offset="100%" stop-color="#07071a" stop-opacity="1"/>
  </linearGradient>

  <linearGradient id="leftVig" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0%"   stop-color="#07071a" stop-opacity="0.72"/>
    <stop offset="45%"  stop-color="#07071a" stop-opacity="0"/>
  </linearGradient>

  <!-- FILTERS -->
  <filter id="textGlow" x="-8%" y="-30%" width="116%" height="160%">
    <feGaussianBlur stdDeviation="4" result="blur"/>
    <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
  </filter>

  <filter id="redGlow" x="-50%" y="-50%" width="200%" height="200%">
    <feGaussianBlur stdDeviation="5" result="blur"/>
    <feFlood flood-color="#cc1a1a" flood-opacity="0.55" result="col"/>
    <feComposite in="col" in2="blur" operator="in" result="shadow"/>
    <feMerge><feMergeNode in="shadow"/><feMergeNode in="SourceGraphic"/></feMerge>
  </filter>

  <!-- ANIMATIONS -->
  <style><![CDATA[
    @keyframes twinkle {
      0%,100% { opacity:.15; }
      50%      { opacity:.90; }
    }
    @keyframes flickA {
      0%,100% { opacity:.65; }
      40%     { opacity:.28; }
      80%     { opacity:.82; }
    }
    @keyframes flickB {
      0%,100% { opacity:.38; }
      25%     { opacity:.76; }
      65%     { opacity:.18; }
    }
    @keyframes webGrow {
      from { stroke-dashoffset:620; opacity:0; }
      to   { stroke-dashoffset:0;   opacity:1; }
    }
    @keyframes arcGrow {
      from { stroke-dashoffset:420; opacity:0; }
      to   { stroke-dashoffset:0;   opacity:1; }
    }
    @keyframes ropeGrow {
      from { stroke-dashoffset:500; }
      to   { stroke-dashoffset:0;   }
    }
    @keyframes slideUp {
      from { opacity:0; transform:translateY(13px); }
      to   { opacity:1; transform:translateY(0);    }
    }
    @keyframes expandX {
      from { transform:scaleX(0); }
      to   { transform:scaleX(1); }
    }
    @keyframes fadeIn {
      from { opacity:0; }
      to   { opacity:1; }
    }
    @keyframes spiderPulse {
      0%,100% { opacity:.65; transform:scale(1);    }
      50%     { opacity:1;   transform:scale(1.10); }
    }

    .star  { animation: twinkle var(--d,3s) ease-in-out infinite var(--del,0s); }
    .win-a { animation: flickA  var(--d,4s) ease-in-out infinite var(--del,0s); }
    .win-b { animation: flickB  var(--d,3.8s) ease-in-out infinite var(--del,0s); }

    .ws {
      fill:none; stroke:rgba(255,255,255,.48); stroke-width:.9;
      stroke-dasharray:620; stroke-dashoffset:620;
      animation: webGrow 1.3s ease-out both;
      animation-delay: var(--del,0s);
    }
    .wa {
      fill:none; stroke:rgba(255,255,255,.28); stroke-width:.6;
      stroke-dasharray:420; stroke-dashoffset:420;
      animation: arcGrow 1.1s ease-out both;
      animation-delay: var(--del,0s);
    }
    .web-rope {
      fill:none; stroke:rgba(255,255,255,.68); stroke-width:1.1;
      stroke-dasharray:500;
      animation: ropeGrow .75s ease-out 2.1s both;
    }

    .txt-name { animation: slideUp .65s cubic-bezier(.22,1,.36,1)  .55s both; }
    .txt-line { transform-origin:76px 119px; animation: expandX .45s ease-out 1.2s both; }
    .txt-sub  { animation: slideUp .6s  cubic-bezier(.22,1,.36,1) 1.35s both; }
    .txt-tag  { animation: slideUp .6s  cubic-bezier(.22,1,.36,1) 1.65s both; }
    .spidey   { animation: fadeIn  .3s  ease-out 2.1s both; }
    .spider-logo { animation: spiderPulse 3.2s ease-in-out 3.8s infinite both; }
  ]]></style>
</defs>

<!-- ══ BACKGROUND ══ -->
<rect width="820" height="280" fill="url(#bgGrad)"/>

<!-- ══ STARS ══ -->
<circle class="star" cx="28"  cy="14"  r=".8"  fill="#fff" style="--d:3.4s;--del:.3s"/>
<circle class="star" cx="72"  cy="8"   r=".6"  fill="#fff" style="--d:4.1s;--del:1.1s"/>
<circle class="star" cx="115" cy="22"  r="1"   fill="#fff" style="--d:2.7s;--del:.7s"/>
<circle class="star" cx="172" cy="11"  r=".7"  fill="#fff" style="--d:5.2s;--del:2.0s"/>
<circle class="star" cx="228" cy="18"  r=".9"  fill="#fff" style="--d:3.8s;--del:.4s"/>
<circle class="star" cx="292" cy="7"   r=".6"  fill="#fff" style="--d:4.6s;--del:1.6s"/>
<circle class="star" cx="352" cy="24"  r=".8"  fill="#fff" style="--d:3.1s;--del:.9s"/>
<circle class="star" cx="418" cy="10"  r="1"   fill="#fff" style="--d:2.9s;--del:2.3s"/>
<circle class="star" cx="478" cy="19"  r=".7"  fill="#fff" style="--d:5.5s;--del:.2s"/>
<circle class="star" cx="544" cy="6"   r=".9"  fill="#fff" style="--d:3.7s;--del:1.4s"/>
<circle class="star" cx="602" cy="23"  r=".6"  fill="#fff" style="--d:4.3s;--del:.8s"/>
<circle class="star" cx="658" cy="12"  r=".8"  fill="#fff" style="--d:2.6s;--del:1.9s"/>
<circle class="star" cx="718" cy="27"  r="1"   fill="#fff" style="--d:4.8s;--del:.5s"/>
<circle class="star" cx="774" cy="9"   r=".7"  fill="#fff" style="--d:3.3s;--del:2.7s"/>
<circle class="star" cx="808" cy="21"  r=".6"  fill="#fff" style="--d:5.0s;--del:1.2s"/>
<circle class="star" cx="50"  cy="42"  r=".7"  fill="#fff" style="--d:4.0s;--del:1.5s"/>
<circle class="star" cx="138" cy="50"  r=".9"  fill="#fff" style="--d:3.6s;--del:.6s"/>
<circle class="star" cx="214" cy="37"  r=".6"  fill="#fff" style="--d:5.1s;--del:2.1s"/>
<circle class="star" cx="312" cy="55"  r=".8"  fill="#fff" style="--d:2.8s;--del:1.0s"/>
<circle class="star" cx="402" cy="44"  r="1"   fill="#fff" style="--d:4.4s;--del:.3s"/>
<circle class="star" cx="488" cy="52"  r=".7"  fill="#fff" style="--d:3.2s;--del:1.8s"/>
<circle class="star" cx="568" cy="40"  r=".9"  fill="#fff" style="--d:5.7s;--del:2.5s"/>
<circle class="star" cx="638" cy="57"  r=".6"  fill="#fff" style="--d:3.9s;--del:.7s"/>
<circle class="star" cx="712" cy="46"  r=".8"  fill="#fff" style="--d:4.5s;--del:1.3s"/>
<circle class="star" cx="788" cy="38"  r="1"   fill="#fff" style="--d:2.9s;--del:2.9s"/>

<!-- ══ BUILDINGS — far layer ══ -->
<g fill="#0e0e26" opacity=".65">
  <rect x="0"   y="180" width="44"  height="100"/>
  <rect x="40"  y="164" width="28"  height="116"/>
  <rect x="64"  y="174" width="36"  height="106"/>
  <rect x="158" y="166" width="44"  height="114"/>
  <rect x="198" y="176" width="30"  height="104"/>
  <rect x="224" y="158" width="50"  height="122"/>
  <rect x="448" y="169" width="38"  height="111"/>
  <rect x="482" y="156" width="52"  height="124"/>
  <rect x="530" y="171" width="32"  height="109"/>
  <rect x="702" y="176" width="40"  height="104"/>
  <rect x="738" y="163" width="30"  height="117"/>
  <rect x="764" y="171" width="48"  height="109"/>
</g>

<!-- ══ BUILDINGS — main layer ══ -->
<g fill="#0c0c20">
  <rect x="0"   y="146" width="58"  height="134"/>
  <!-- Chrysler-like spire -->
  <polygon points="82,116 86,116 89,129 94,132 96,141 102,141 102,280 78,280 78,141 83,141 85,132 90,129"/>
  <rect x="102" y="149" width="70"  height="131"/>
  <!-- Empire State silhouette -->
  <polygon points="272,84 278,84 281,99 286,101 288,109 290,115 292,121 294,127 302,127 302,280 260,280 260,127 268,127 270,121 272,115 274,109 276,101 281,99"/>
  <rect x="322" y="143" width="56"  height="137"/>
  <rect x="432" y="137" width="68"  height="143"/>
  <rect x="504" y="133" width="82"  height="147"/>
  <!-- Tapered tower -->
  <polygon points="600,96 606,96 610,113 614,116 616,125 620,131 626,131 626,280 592,280 592,131 598,131 602,125 606,116 608,113"/>
  <rect x="642" y="146" width="60"  height="134"/>
  <rect x="700" y="139" width="76"  height="141"/>
  <rect x="774" y="151" width="46"  height="129"/>
</g>

<!-- ══ WINDOWS ══ -->
<g>
  <rect class="win-a" x="6"   y="156" width="3" height="4" fill="#ffd060" style="--d:4.2s;--del:.5s"/>
  <rect class="win-b" x="12"  y="156" width="3" height="4" fill="#ffd060" style="--d:3.8s;--del:1.2s"/>
  <rect class="win-a" x="18"  y="156" width="3" height="4" fill="#ffa040" style="--d:5.1s;--del:.2s"/>
  <rect class="win-b" x="6"   y="164" width="3" height="4" fill="#ffd060" style="--d:3.5s;--del:2.0s"/>
  <rect class="win-a" x="12"  y="164" width="3" height="4" fill="#ffd060" style="--d:4.7s;--del:.8s"/>
  <rect class="win-b" x="18"  y="164" width="3" height="4" fill="#ffa040" style="--d:3.2s;--del:1.5s"/>
  <rect class="win-a" x="6"   y="172" width="3" height="4" fill="#ffd060" style="--d:5.4s;--del:.1s"/>
  <rect class="win-b" x="18"  y="172" width="3" height="4" fill="#ffd060" style="--d:4.0s;--del:2.6s"/>
  <rect class="win-a" x="6"   y="180" width="3" height="4" fill="#ffa040" style="--d:3.3s;--del:1.8s"/>
  <rect class="win-b" x="30"  y="154" width="3" height="4" fill="#ffd060" style="--d:4.8s;--del:.7s"/>
  <rect class="win-a" x="36"  y="154" width="3" height="4" fill="#ffa040" style="--d:3.6s;--del:2.2s"/>
  <rect class="win-b" x="42"  y="154" width="3" height="4" fill="#ffd060" style="--d:5.2s;--del:.3s"/>
  <rect class="win-a" x="30"  y="162" width="3" height="4" fill="#ffd060" style="--d:4.1s;--del:1.4s"/>
  <rect class="win-b" x="42"  y="162" width="3" height="4" fill="#ffa040" style="--d:3.9s;--del:.9s"/>

  <rect class="win-a" x="112" y="159" width="3" height="4" fill="#ffd060" style="--d:4.3s;--del:1.3s"/>
  <rect class="win-b" x="118" y="159" width="3" height="4" fill="#ffd060" style="--d:3.7s;--del:.6s"/>
  <rect class="win-a" x="124" y="159" width="3" height="4" fill="#ffa040" style="--d:5.0s;--del:2.4s"/>
  <rect class="win-b" x="130" y="159" width="3" height="4" fill="#ffd060" style="--d:4.6s;--del:.1s"/>
  <rect class="win-a" x="112" y="167" width="3" height="4" fill="#ffd060" style="--d:3.4s;--del:1.7s"/>
  <rect class="win-b" x="118" y="167" width="3" height="4" fill="#ffa040" style="--d:5.3s;--del:2.8s"/>
  <rect class="win-a" x="124" y="167" width="3" height="4" fill="#ffd060" style="--d:4.0s;--del:.5s"/>
  <rect class="win-b" x="130" y="167" width="3" height="4" fill="#ffd060" style="--d:3.8s;--del:1.1s"/>
  <rect class="win-a" x="112" y="175" width="3" height="4" fill="#ffa040" style="--d:4.9s;--del:.2s"/>
  <rect class="win-b" x="124" y="175" width="3" height="4" fill="#ffd060" style="--d:3.5s;--del:2.3s"/>

  <rect class="win-b" x="265" y="136" width="2" height="3" fill="#ffd060" style="--d:4.1s;--del:1.6s"/>
  <rect class="win-a" x="269" y="136" width="2" height="3" fill="#ffd060" style="--d:3.6s;--del:.4s"/>
  <rect class="win-b" x="273" y="136" width="2" height="3" fill="#ffa040" style="--d:5.5s;--del:2.0s"/>
  <rect class="win-a" x="265" y="142" width="2" height="3" fill="#ffd060" style="--d:4.7s;--del:.8s"/>
  <rect class="win-b" x="273" y="142" width="2" height="3" fill="#ffd060" style="--d:3.2s;--del:1.3s"/>
  <rect class="win-a" x="265" y="148" width="2" height="3" fill="#ffa040" style="--d:5.8s;--del:2.7s"/>
  <rect class="win-b" x="269" y="148" width="2" height="3" fill="#ffd060" style="--d:4.3s;--del:.2s"/>
  <rect class="win-a" x="273" y="148" width="2" height="3" fill="#ffd060" style="--d:3.9s;--del:1.9s"/>

  <rect class="win-a" x="512" y="143" width="3" height="4" fill="#ffd060" style="--d:4.5s;--del:1.4s"/>
  <rect class="win-b" x="518" y="143" width="3" height="4" fill="#ffa040" style="--d:3.3s;--del:.6s"/>
  <rect class="win-a" x="524" y="143" width="3" height="4" fill="#ffd060" style="--d:5.6s;--del:2.2s"/>
  <rect class="win-b" x="530" y="143" width="3" height="4" fill="#ffd060" style="--d:4.2s;--del:.3s"/>
  <rect class="win-a" x="536" y="143" width="3" height="4" fill="#ffa040" style="--d:3.7s;--del:1.8s"/>
  <rect class="win-b" x="512" y="151" width="3" height="4" fill="#ffd060" style="--d:4.8s;--del:.9s"/>
  <rect class="win-a" x="524" y="151" width="3" height="4" fill="#ffd060" style="--d:3.4s;--del:2.5s"/>
  <rect class="win-b" x="536" y="151" width="3" height="4" fill="#ffa040" style="--d:5.1s;--del:.5s"/>
  <rect class="win-a" x="512" y="159" width="3" height="4" fill="#ffd060" style="--d:4.0s;--del:1.2s"/>
  <rect class="win-b" x="524" y="159" width="3" height="4" fill="#ffd060" style="--d:3.6s;--del:2.9s"/>
  <rect class="win-a" x="536" y="159" width="3" height="4" fill="#ffa040" style="--d:3.1s;--del:1.6s"/>

  <rect class="win-a" x="652" y="156" width="3" height="4" fill="#ffd060" style="--d:4.4s;--del:2.1s"/>
  <rect class="win-b" x="658" y="156" width="3" height="4" fill="#ffd060" style="--d:3.8s;--del:.4s"/>
  <rect class="win-a" x="664" y="156" width="3" height="4" fill="#ffa040" style="--d:5.3s;--del:1.0s"/>
  <rect class="win-b" x="670" y="156" width="3" height="4" fill="#ffd060" style="--d:4.1s;--del:2.6s"/>
  <rect class="win-a" x="652" y="164" width="3" height="4" fill="#ffd060" style="--d:3.5s;--del:.8s"/>
  <rect class="win-b" x="664" y="164" width="3" height="4" fill="#ffa040" style="--d:4.9s;--del:1.4s"/>
  <rect class="win-a" x="670" y="164" width="3" height="4" fill="#ffd060" style="--d:3.2s;--del:2.0s"/>

  <rect class="win-b" x="708" y="149" width="3" height="4" fill="#ffd060" style="--d:3.7s;--del:.6s"/>
  <rect class="win-a" x="714" y="149" width="3" height="4" fill="#ffa040" style="--d:4.8s;--del:2.3s"/>
  <rect class="win-b" x="720" y="149" width="3" height="4" fill="#ffd060" style="--d:3.3s;--del:.9s"/>
  <rect class="win-a" x="726" y="149" width="3" height="4" fill="#ffd060" style="--d:5.4s;--del:1.5s"/>
  <rect class="win-b" x="708" y="157" width="3" height="4" fill="#ffa040" style="--d:4.0s;--del:2.8s"/>
  <rect class="win-a" x="714" y="157" width="3" height="4" fill="#ffd060" style="--d:3.6s;--del:.2s"/>
  <rect class="win-b" x="726" y="157" width="3" height="4" fill="#ffd060" style="--d:4.7s;--del:1.1s"/>
  <rect class="win-a" x="708" y="165" width="3" height="4" fill="#ffd060" style="--d:3.1s;--del:2.4s"/>
  <rect class="win-b" x="720" y="165" width="3" height="4" fill="#ffa040" style="--d:5.2s;--del:.7s"/>
  <rect class="win-a" x="726" y="165" width="3" height="4" fill="#ffd060" style="--d:4.4s;--del:1.8s"/>
</g>

<!-- ══ WEB — radial strands from top-right ══ -->
<line class="ws" x1="820" y1="0" x2="572" y2="280" style="--del:.38s"/>
<line class="ws" x1="820" y1="0" x2="662" y2="280" style="--del:.52s"/>
<line class="ws" x1="820" y1="0" x2="752" y2="280" style="--del:.66s"/>
<line class="ws" x1="820" y1="0" x2="820" y2="200" style="--del:.80s"/>
<line class="ws" x1="820" y1="0" x2="482" y2="212" style="--del:.46s"/>
<line class="ws" x1="820" y1="0" x2="562" y2="172" style="--del:.60s"/>
<line class="ws" x1="820" y1="0" x2="642" y2="150" style="--del:.74s"/>
<line class="ws" x1="820" y1="0" x2="722" y2="136" style="--del:.88s"/>
<line class="ws" x1="820" y1="0" x2="784" y2="110" style="--del:1.02s"/>

<!-- Web arcs -->
<path class="wa" d="M 758,0  Q 802,34  820,27"  style="--del:1.15s"/>
<path class="wa" d="M 702,0  Q 778,60  820,53"  style="--del:1.28s"/>
<path class="wa" d="M 638,0  Q 750,94  820,86"  style="--del:1.42s"/>
<path class="wa" d="M 562,0  Q 720,130 820,120" style="--del:1.56s"/>
<path class="wa" d="M 478,16 Q 684,165 820,154" style="--del:1.70s"/>
<path class="wa" d="M 396,48 Q 650,198 820,186" style="--del:1.84s"/>
<path class="wa" d="M 676,216 Q 750,250 820,236" style="--del:1.98s"/>

<!-- ══ WEB ROPE (attachment point → Spider-Man landing spot) ══ -->
<line class="web-rope" x1="820" y1="0" x2="258" y2="150"/>

<!-- ══ SPIDER-MAN ══ -->
<g class="spidey">
  <animateTransform attributeName="transform" type="translate"
    values="-65,228; 192,154; 258,150"
    keyTimes="0;.76;1"
    dur="2.0s" begin="2.1s" fill="freeze"
    calcMode="spline" keySplines=".42 0 .58 1;.42 0 .58 1"/>

  <!-- Blue legs -->
  <line x1="-6"  y1="11" x2="-20" y2="32"  stroke="#1a3a8c" stroke-width="6"  stroke-linecap="round"/>
  <line x1="6"   y1="11" x2="15"  y2="34"  stroke="#1a3a8c" stroke-width="6"  stroke-linecap="round"/>
  <ellipse cx="-21" cy="34" rx="5.5" ry="3.2" fill="#1a3a8c" transform="rotate(-28,-21,34)"/>
  <ellipse cx="17"  cy="36" rx="5.5" ry="3.2" fill="#1a3a8c" transform="rotate(14,17,36)"/>

  <!-- Red torso -->
  <ellipse cx="0" cy="0" rx="12" ry="14" fill="#cc1a1a"/>
  <!-- Blue waist band -->
  <rect x="-12" y="7" width="24" height="6" rx="2" fill="#1a3a8c"/>

  <!-- Shoulder circles (blend arms into torso) -->
  <circle cx="11"  cy="-5" r="5.5" fill="#cc1a1a"/>
  <circle cx="-11" cy="-5" r="5.5" fill="#cc1a1a"/>

  <!-- Blue arms -->
  <!-- Right arm: shooting web upward -->
  <line x1="11"  y1="-7" x2="28"  y2="-24" stroke="#1a3a8c" stroke-width="5.5" stroke-linecap="round"/>
  <ellipse cx="30" cy="-26" rx="5"  ry="4"  fill="#1a3a8c" transform="rotate(-42,30,-26)"/>
  <!-- Left arm: trailing behind -->
  <line x1="-11" y1="-7" x2="-24" y2="6"   stroke="#1a3a8c" stroke-width="5.5" stroke-linecap="round"/>
  <ellipse cx="-26" cy="7" rx="5"  ry="4"   fill="#1a3a8c" transform="rotate(28,-26,7)"/>

  <!-- Red head -->
  <circle cx="0" cy="-21" r="11.5" fill="#cc1a1a"/>

  <!-- White eye lenses -->
  <ellipse cx="-4.5" cy="-22" rx="4.8" ry="3.8" fill="#e8e8e8" transform="rotate(-14,-4.5,-22)"/>
  <ellipse cx="4.5"  cy="-22" rx="4.8" ry="3.8" fill="#e8e8e8" transform="rotate(14,4.5,-22)"/>

  <!-- Black web pattern on suit -->
  <line x1="0" y1="-33" x2="0" y2="13"  stroke="#111" stroke-width=".8" opacity=".65"/>
  <line x1="-12" y1="-8" x2="12" y2="-8" stroke="#111" stroke-width=".8" opacity=".65"/>
  <line x1="-12" y1="0"  x2="12" y2="0"  stroke="#111" stroke-width=".8" opacity=".65"/>
  <line x1="-12" y1="7"  x2="12" y2="7"  stroke="#111" stroke-width=".8" opacity=".65"/>
  <path d="M -12,-8 Q 0,-15 12,-8"  stroke="#111" stroke-width=".7" fill="none" opacity=".55"/>
  <path d="M -12,0  Q 0,-6  12,0"   stroke="#111" stroke-width=".7" fill="none" opacity=".55"/>
  <!-- Web lines on head -->
  <line x1="-3" y1="-33" x2="-9"  y2="-18" stroke="#111" stroke-width=".6" opacity=".5"/>
  <line x1="3"  y1="-33" x2="9"   y2="-18" stroke="#111" stroke-width=".6" opacity=".5"/>
  <line x1="-11" y1="-25" x2="11" y2="-25" stroke="#111" stroke-width=".6" opacity=".5"/>
  <line x1="-11" y1="-20" x2="11" y2="-20" stroke="#111" stroke-width=".6" opacity=".5"/>

  <!-- Web line from right wrist upward (part of swing rope) -->
  <line x1="30" y1="-26" x2="562" y2="-276" stroke="rgba(255,255,255,.62)" stroke-width="1"/>
</g>

<!-- ══ TEXT ══ -->
<text class="txt-name"
      x="76" y="108"
      font-family="'Arial Black','Impact','Haettenschweiler',sans-serif"
      font-size="50" font-weight="900" letter-spacing="-1"
      fill="white" filter="url(#textGlow)">BARAN ERDOGAN</text>

<rect class="txt-line"
      x="76" y="119" width="368" height="3" rx="1.5" fill="#cc1a1a"/>

<text class="txt-sub"
      x="78" y="147"
      font-family="'Arial','Helvetica',sans-serif"
      font-size="15" font-weight="400" letter-spacing="3.5"
      fill="rgba(255,255,255,.78)">MSc BUSINESS ANALYTICS · ESADE</text>

<text class="txt-tag"
      x="80" y="169"
      font-family="'Arial','Helvetica',sans-serif"
      font-size="11.5" font-weight="300" letter-spacing="1.8"
      fill="rgba(255,255,255,.46)">ML  ·  CLOUD  ·  DATA ENGINEERING</text>

<!-- ══ SPIDER LOGO (bottom-right corner) ══ -->
<g class="spider-logo" transform="translate(778,248)" filter="url(#redGlow)">
  <ellipse cx="0" cy="1"   rx="5"   ry="7.5" fill="#cc1a1a"/>
  <circle  cx="0" cy="-10" r="4.5"           fill="#cc1a1a"/>
  <line x1="-5" y1="-5"  x2="-16" y2="-13" stroke="#cc1a1a" stroke-width="1.5" stroke-linecap="round"/>
  <line x1="-5" y1="0"   x2="-17" y2="1"   stroke="#cc1a1a" stroke-width="1.5" stroke-linecap="round"/>
  <line x1="-5" y1="5"   x2="-16" y2="13"  stroke="#cc1a1a" stroke-width="1.5" stroke-linecap="round"/>
  <line x1="-2" y1="8"   x2="-5"  y2="19"  stroke="#cc1a1a" stroke-width="1.5" stroke-linecap="round"/>
  <line x1="5"  y1="-5"  x2="16"  y2="-13" stroke="#cc1a1a" stroke-width="1.5" stroke-linecap="round"/>
  <line x1="5"  y1="0"   x2="17"  y2="1"   stroke="#cc1a1a" stroke-width="1.5" stroke-linecap="round"/>
  <line x1="5"  y1="5"   x2="16"  y2="13"  stroke="#cc1a1a" stroke-width="1.5" stroke-linecap="round"/>
  <line x1="2"  y1="8"   x2="5"   y2="19"  stroke="#cc1a1a" stroke-width="1.5" stroke-linecap="round"/>
  <circle cx="0" cy="0" r="22" fill="none" stroke="#cc1a1a" stroke-width=".5" opacity=".32"/>
</g>

<!-- ══ OVERLAYS ══ -->
<rect x="0" y="208" width="820" height="72"  fill="url(#bottomFade)"/>
<rect x="0" y="0"   width="820" height="280" fill="url(#leftVig)"/>

</svg>

<div align="left">

![Header](https://raw.githubusercontent.com/baranerdogan11/baranerdogan11/main/header.svg)

# Hi, I'm Baran👋

### MSc Business Analytics · ESADE Business School

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR_LINKEDIN)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/BaranErdogan)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:YOUR_EMAIL@esade.edu)

</div>

---

## About Me

I'm a Business Analytics student at ESADE with a passion for turning messy, real-world data into systems that actually work in production. I'm particularly drawn to problems where ML meets physical processes — manufacturing, logistics, operations — where a good prediction has a tangible, measurable impact.

I come from **[YOUR BACKGROUND — e.g. a background in industrial engineering / finance / consulting]**, which gave me a strong appreciation for the gap between theoretical models and operational reality. At ESADE I've been closing that gap — building end-to-end pipelines from raw sensor data all the way to cloud-deployed inference endpoints.

- Based in **Barcelona, Spain**
- Fluent in **[YOUR LANGUAGES — e.g. Turkish, English, Spanish]**
- Looking for roles in **data science, ML engineering, or analytics engineering**

---

### 🔧 Tech Stack

*Languages & Analysis*  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)

*Cloud & Infrastructure*  
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)
![SageMaker](https://img.shields.io/badge/SageMaker-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)

*Data & ML*  
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-0071C5?style=flat-square&logo=xgboost&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

---

## 🔨 What I Build

Below are selected repositories.

<table>
<tr>
<td width="50%">

**🏭 VaultTech — Industrial Cycle Time Prediction**  
End-to-end ML pipeline on ~180k PLC sensor readings from a steel forging line. Predicts total bath time after just the 2nd strike (18s into a 58s process), enabling real-time delay alerts before a piece finishes. Medallion architecture (Bronze → Silver → Gold) in PostgreSQL, XGBoost model deployed on AWS SageMaker with a live Streamlit dashboard.

🔗[Repository Link](https://github.com/baranerdogan11/baranerdogan-caws-final-project)

</td>
<td width="50%">

**🌳 San Francisco Urban Forest**   
Data visualisation of 190,300 street trees across San Francisco using R — spatial density, Shannon biodiversity index by census tract, species distribution small multiples, and a 52-year planting timeline. Built an interactive HTML infographic with a click-to-focus panel system and a Mapbox-powered 3D extrusion map.

🔗 [Repository Link](https://github.com/baranerdogan11/dataviz-club)

</td>
</tr>
<tr>
<td width="50%">

**🚀 Kickstarter Campaign Success Prediction**  
Binary classifier trained on ~160k campaigns to predict funding success using only pre-launch information. Compared 6 models (Random Forest, XGBoost, Logistic Regression, MLP, GB, Decision Tree) with chronological train/val/test splits — Logistic Regression won on the test set despite losing on validation, a textbook case of simpler models generalising better under distributional shift.

🔗 [Repository Link](https://github.com/baranerdogan11/AI-II-Final-Project)

</td>
<td width="50%">

**🛒 Eco-Smart AI Grocery Assistant**  
Agentic grocery assistant that combines an LLM for implicit allergen reasoning (e.g. "creamy" → likely dairy) with a logistic regression safety classifier (92.5% accuracy). The LLM outputs constrained JSON rather than free text, which drives a dynamic Streamlit dashboard tracking ingredient safety, CO2 savings, and shelf-life discounts in real time.

🔗 [Repository Link](https://github.com/baranerdogan11/eco-smart-ai-final)

</td>
</tr>
</table>

---

## 📊 GitHub Stats

<div align="left">


![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=baranerdogan11&layout=compact&theme=github_dark&hide_border=true&hide=typescript,javascript,css,html,scss)

</div>

<div align="center">

*Open to opportunities in data science, ML engineering, and analytics engineering — especially where the data is messy and the stakes are real.*

**[LinkedIn](https://linkedin.com/in/YOUR_LINKEDIN) · [Email](mailto:baran.erdogan@alumni.esade.edu)**

</div>

