<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<title>MAVRCK // signal from the edge</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700;900&family=VT323&family=Space+Grotesk:wght@300;400;500;700&display=swap">
<style>
:root {
  --bg-0: #0a0420;
  --bg-1: #1a0638;
  --fg: #ffe8ff;
  --magenta: #ff2a9d;
  --pink: #ff5fd0;
  --cyan: #00f0ff;
  --purple: #8a2be2;
  --sun-top: #ffd84d;
  --sun-mid: #ff5fd0;
  --sun-bot: #8a2be2;
  --scan-alpha: 0.18;
}

* { box-sizing: border-box; }
html, body {
  margin: 0;
  padding: 0;
  background: var(--bg-0);
  color: var(--fg);
  font-family: 'Space Grotesk', system-ui, sans-serif;
  overflow: hidden;
  height: 100%;
  cursor: crosshair;
}
body {
  min-height: 100vh;
  position: relative;
}

/* Stars ------------------------------------------------------- */
.stars, .stars::before, .stars::after {
  position: fixed;
  inset: 0;
  pointer-events: none;
  z-index: 0;
}
.stars {
  background:
    radial-gradient(ellipse at 50% 100%, color-mix(in oklab, var(--purple) 40%, transparent) 0%, transparent 55%),
    radial-gradient(ellipse at 50% 60%, color-mix(in oklab, var(--magenta) 20%, transparent) 0%, transparent 60%),
    linear-gradient(180deg, var(--bg-0) 0%, var(--bg-1) 60%, var(--bg-0) 100%);
}
.star-layer {
  position: fixed; inset: -50px; pointer-events: none; z-index: 1;
  transition: transform .2s ease-out;
}
.star-layer svg { width: 100%; height: 100%; display: block; }

/* Scanlines + CRT vignette ------------------------------------ */
.scanlines {
  position: fixed; inset: 0; pointer-events: none; z-index: 100;
  background:
    repeating-linear-gradient(
      0deg,
      rgba(0,0,0,var(--scan-alpha)) 0px,
      rgba(0,0,0,var(--scan-alpha)) 1px,
      transparent 1px,
      transparent 3px
    );
  mix-blend-mode: multiply;
}
.vignette {
  position: fixed; inset: 0; pointer-events: none; z-index: 99;
  background: radial-gradient(ellipse at center, transparent 40%, rgba(0,0,0,0.6) 100%);
}
.noise {
  position: fixed; inset:0; pointer-events:none; z-index: 98;
  opacity: 0.06; mix-blend-mode: overlay;
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='200' height='200'><filter id='n'><feTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='2' stitchTiles='stitch'/></filter><rect width='100%' height='100%' filter='url(%23n)'/></svg>");
}

/* Main stage -------------------------------------------------- */
.stage {
  position: relative;
  z-index: 10;
  width: 100%;
  height: 100vh;
  min-height: 560px;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 70px 40px;
  overflow: hidden;
}

/* Top/bottom chrome */
.topbar, .bottombar {
  position: fixed;
  left: 0; right: 0;
  z-index: 50;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 28px;
  font-family: 'VT323', monospace;
  font-size: 18px;
  color: var(--cyan);
  text-shadow: 0 0 8px var(--cyan);
  pointer-events: none;
  letter-spacing: 0.08em;
}
.topbar { top: 0; }
.bottombar { bottom: 0; }
.chrome-dot {
  display: inline-block;
  width: 8px; height: 8px; border-radius: 50%;
  background: var(--magenta);
  box-shadow: 0 0 8px var(--magenta);
  margin-right: 8px;
  animation: blink 1.2s steps(2) infinite;
}
@keyframes blink { 50% { opacity: .2; } }

/* Cockpit HUD ------------------------------------------------- */
.hud {
  width: min(1200px, 94vw);
  max-height: 86vh;
  border: 2px solid var(--cyan);
  border-radius: 8px;
  background:
    linear-gradient(180deg, color-mix(in oklab, var(--bg-1) 90%, transparent), color-mix(in oklab, var(--bg-0) 90%, transparent));
  padding: 24px;
  display: grid;
  grid-template-columns: 1fr 1.4fr 1fr;
  grid-template-rows: auto 1fr auto;
  gap: 18px;
  box-shadow:
    0 0 0 1px color-mix(in oklab, var(--cyan) 30%, transparent),
    0 0 40px color-mix(in oklab, var(--cyan) 25%, transparent),
    inset 0 0 60px color-mix(in oklab, var(--purple) 15%, transparent);
  position: relative;
  backdrop-filter: blur(2px);
}
.hud::before {
  content:''; position:absolute;
  top:-10px; left:20px; right:20px; height: 2px;
  background: var(--magenta); box-shadow: 0 0 12px var(--magenta);
}
.hud-header {
  grid-column: 1 / -1;
  display:flex; justify-content: space-between; align-items: center;
  border-bottom: 1px dashed color-mix(in oklab, var(--cyan) 50%, transparent);
  padding-bottom: 10px;
}
.hud-title {
  font-family: 'VT323', monospace;
  color: var(--cyan);
  font-size: 20px;
  letter-spacing: 0.2em;
  text-shadow: 0 0 6px var(--cyan);
}
.hud-title .chrome-dot { background: var(--magenta); box-shadow: 0 0 8px var(--magenta);}
.hud-meta {
  font-family: 'VT323', monospace;
  color: var(--magenta);
  font-size: 16px;
  letter-spacing: 0.1em;
  text-shadow: 0 0 6px var(--magenta);
}

.hud-left, .hud-right {
  border: 1px solid color-mix(in oklab, var(--cyan) 40%, transparent);
  padding: 16px;
  font-family: 'VT323', monospace;
  color: var(--fg);
  font-size: 18px;
  line-height: 1.5;
  background: color-mix(in oklab, var(--cyan) 3%, transparent);
  min-height: 260px;
}
.hud-label {
  font-size: 13px;
  color: var(--cyan);
  letter-spacing: 0.2em;
  text-transform: uppercase;
  margin-bottom: 8px;
  opacity: .8;
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 500;
}
.hud-kv { display: flex; justify-content: space-between; margin: 4px 0; }
.hud-kv span:last-child { color: var(--sun-top); }

.hud-center {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 16px;
  padding: 20px;
  border: 1px solid color-mix(in oklab, var(--magenta) 40%, transparent);
  background: radial-gradient(ellipse at center, color-mix(in oklab, var(--magenta) 12%, transparent), transparent 70%);
  min-height: 260px;
  position: relative;
}
.hud-center::before, .hud-center::after{
  content:''; position:absolute;
  width:20px; height:20px;
  border: 2px solid var(--magenta);
}
.hud-center::before { top:6px; left:6px; border-right:0; border-bottom:0;}
.hud-center::after { bottom:6px; right:6px; border-left:0; border-top:0;}

.hud-wordmark {
  font-family: 'Orbitron', sans-serif;
  font-weight: 900;
  font-size: clamp(40px, 7vw, 96px);
  letter-spacing: 0.06em;
  background: linear-gradient(180deg, var(--sun-top), var(--sun-mid), var(--sun-bot));
  -webkit-background-clip: text; background-clip: text; color: transparent;
  filter: drop-shadow(0 0 12px color-mix(in oklab, var(--magenta) 70%, transparent));
  margin: 0;
  line-height: 1;
}
.hud-callsign {
  font-family: 'VT323', monospace;
  color: var(--cyan);
  font-size: 18px;
  letter-spacing: 0.3em;
  text-shadow: 0 0 6px var(--cyan);
}
.hud-tagline {
  font-family: 'Space Grotesk', sans-serif;
  color: var(--fg);
  font-size: 14px;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  text-align: center;
  opacity: .85;
  max-width: 320px;
}

.hud-socials {
  grid-column: 1 / -1;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 12px;
}
.hud-social {
  --c: var(--cyan);
  border: 1px solid var(--c);
  padding: 14px 16px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  text-decoration: none;
  color: var(--c);
  font-family: 'VT323', monospace;
  letter-spacing: 0.15em;
  font-size: 18px;
  background: color-mix(in oklab, var(--c) 5%, transparent);
  transition: all .25s;
  position: relative;
}
.hud-social:hover {
  background: var(--c);
  color: var(--bg-0);
  box-shadow: 0 0 25px var(--c), inset 0 0 20px rgba(255,255,255,.3);
}
.hud-social:nth-child(1){ --c: var(--cyan); }
.hud-social:nth-child(2){ --c: var(--magenta); }
.hud-social:nth-child(3){ --c: var(--sun-top); }
.hud-social:nth-child(4){ --c: var(--pink); }
.hud-social svg { width: 20px; height: 20px; }
.hud-social-handle { font-size: 13px; opacity: .75; letter-spacing: 0.1em; }

/* Radar */
.radar {
  width: 160px; height: 160px;
  border-radius: 50%;
  border: 1px solid var(--cyan);
  position: relative;
  background: radial-gradient(circle, transparent 0%, transparent 60%, color-mix(in oklab, var(--cyan) 15%, transparent) 100%);
  box-shadow: inset 0 0 20px color-mix(in oklab, var(--cyan) 30%, transparent);
  overflow: hidden;
}
.radar::before, .radar::after {
  content:''; position: absolute; inset: 0;
  border-radius: 50%;
  border: 1px dashed color-mix(in oklab, var(--cyan) 35%, transparent);
}
.radar::before { inset: 25%;}
.radar::after { inset: 50%;}
.radar-sweep {
  position: absolute; inset: 0;
  background: conic-gradient(from 0deg, color-mix(in oklab, var(--magenta) 50%, transparent), transparent 30%);
  border-radius: 50%;
  animation: sweep 4s linear infinite;
}
@keyframes sweep { to { transform: rotate(360deg); } }
.radar-dot {
  position:absolute;
  width:6px; height:6px; border-radius:50%;
  background: var(--magenta);
  box-shadow: 0 0 6px var(--magenta);
  animation: blip 4s linear infinite;
}
.radar-dot:nth-child(2){ top: 22%; left: 60%; animation-delay: .5s;}
.radar-dot:nth-child(3){ top: 50%; left: 30%; animation-delay: 1.5s;}
.radar-dot:nth-child(4){ top: 70%; left: 70%; animation-delay: 2.5s;}
@keyframes blip {
  0%, 40% { opacity: 0; }
  45% { opacity: 1; transform: scale(1.8);}
  60%, 100% { opacity: .5; transform: scale(1);}
}

/* Responsive — tablet ----------------------------------------- */
@media (max-width: 820px) {
  html, body { overflow: auto; }
  .stage {
    height: auto;
    min-height: 100vh;
    padding: 60px 20px;
    overflow: visible;
  }
  .hud {
    grid-template-columns: 1fr;
    max-height: none;
    padding: 18px;
    gap: 14px;
  }
  .hud-left, .hud-right { min-height: auto; }
  .hud-center { min-height: auto; }
  .hud-socials { grid-template-columns: 1fr 1fr; }
  .topbar, .bottombar { font-size: 13px; padding: 14px 18px; }
  .radar { width: 120px; height: 120px; }
}

/* Responsive — phone ------------------------------------------ */
@media (max-width: 480px) {
  .stage { padding: 50px 10px; }
  .hud { padding: 14px; gap: 10px; }
  .hud-header { flex-direction: column; align-items: flex-start; gap: 4px; }
  .hud-title { font-size: 16px; letter-spacing: 0.12em; }
  .hud-meta { font-size: 13px; }
  .hud-left, .hud-right { padding: 12px; font-size: 16px; }
  .hud-center { padding: 16px; gap: 12px; }
  .hud-wordmark { font-size: clamp(32px, 12vw, 56px); }
  .hud-callsign { font-size: 15px; letter-spacing: 0.2em; }
  .hud-tagline { font-size: 12px; letter-spacing: 0.1em; }
  .radar { width: 100px; height: 100px; }
  .hud-socials { grid-template-columns: 1fr; gap: 8px; }
  .hud-social { padding: 12px 14px; font-size: 16px; }
  .topbar, .bottombar { font-size: 11px; padding: 10px 12px; }
  .bottombar div:last-child { display: none; }
}
</style>
</head>
<body>

<!-- Background layers -->
<div class="stars"></div>
<div class="star-layer" id="starLayer"></div>

<!-- Top/bottom chrome -->
<div class="topbar">
  <div><span class="chrome-dot"></span>TRANSMISSION // LIVE</div>
  <div id="clock">T+ 00:00:00</div>
</div>
<div class="bottombar">
  <div>SYS.MAVRCK.v2.6 // ALT 34,000FT // HDG 270&deg;</div>
  <div>SIGNAL LOCKED</div>
</div>

<!-- Stage -->
<div class="stage">
  <div class="hud">
    <div class="hud-header">
      <div class="hud-title"><span class="chrome-dot"></span>FLIGHT CONSOLE :: MVK-01</div>
      <div class="hud-meta">HDG 270&deg;  ALT 34K  SPD 540KT</div>
    </div>
    <div class="hud-left">
      <div class="hud-label">// TELEMETRY</div>
      <div class="hud-kv"><span>CALLSIGN</span><span>@MAVRCK</span></div>
      <div class="hud-kv"><span>STATUS</span><span>ONLINE</span></div>
      <div class="hud-kv"><span>MODE</span><span>BUILD</span></div>
      <div class="hud-kv"><span>FUEL</span><span>&infin;</span></div>
      <div class="hud-kv"><span>SIGNAL</span><span>STRONG</span></div>
      <div class="hud-kv"><span>LOCK</span><span>ACQUIRED</span></div>
      <div class="hud-kv"><span>UPLINK</span><span>LIVE</span></div>
    </div>
    <div class="hud-center">
      <div class="hud-callsign">// MVK-01</div>
      <h1 class="hud-wordmark">MAVRCK</h1>
      <p class="hud-tagline">maker. student pilot. engineer. photographer.</p>
      <div class="radar">
        <div class="radar-sweep"></div>
        <div class="radar-dot"></div>
        <div class="radar-dot"></div>
        <div class="radar-dot"></div>
      </div>
    </div>
    <div class="hud-right">
      <div class="hud-label">// LOGBOOK</div>
      <div style="opacity:.85;">&gt; boot sequence ok</div>
      <div style="opacity:.85;">&gt; systems nominal</div>
      <div style="opacity:.85;">&gt; visor polarized</div>
      <div style="opacity:.85;">&gt; receiving signal...</div>
      <div style="opacity:.85;">&gt; making things</div>
      <div style="opacity:.85;">&gt; flying things</div>
      <div style="opacity:.85;color:var(--cyan);">&gt; _</div>
    </div>
    <div class="hud-socials">
      <a class="hud-social" href="https://github.com/mavrck" target="_blank" rel="noopener">
        <span style="display:inline-flex;align-items:center;gap:10px;"><svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 .5C5.65.5.5 5.65.5 12c0 5.08 3.29 9.39 7.86 10.91.58.1.79-.25.79-.56 0-.27-.01-1-.02-1.96-3.2.7-3.87-1.54-3.87-1.54-.52-1.33-1.28-1.68-1.28-1.68-1.05-.72.08-.7.08-.7 1.16.08 1.77 1.19 1.77 1.19 1.03 1.77 2.7 1.26 3.36.96.1-.75.4-1.26.73-1.55-2.55-.29-5.24-1.28-5.24-5.69 0-1.26.45-2.28 1.19-3.09-.12-.29-.52-1.46.11-3.05 0 0 .97-.31 3.18 1.18.92-.26 1.91-.38 2.9-.39.98.01 1.97.13 2.9.39 2.21-1.49 3.18-1.18 3.18-1.18.63 1.59.23 2.76.11 3.05.74.81 1.19 1.83 1.19 3.09 0 4.42-2.69 5.39-5.25 5.68.41.35.77 1.04.77 2.1 0 1.51-.01 2.73-.01 3.1 0 .31.21.67.8.56A11.51 11.51 0 0 0 23.5 12C23.5 5.65 18.35.5 12 .5z"/></svg>GITHUB</span>
        <span class="hud-social-handle">@mavrck</span>
      </a>
      <a class="hud-social" href="https://bsky.app/profile/mavrck.com" target="_blank" rel="noopener">
        <span style="display:inline-flex;align-items:center;gap:10px;"><svg viewBox="0 0 24 24" fill="currentColor"><path d="M6.3 3.9C8.8 5.8 11.5 9.5 12 11.5c.5-2 3.2-5.7 5.7-7.6 1.8-1.4 4.8-2.5 4.8 1 0 .7-.4 5.7-.6 6.5-.7 2.9-3.6 3.6-6.1 3.2 4.5.8 5.6 3.3 3.1 5.9-4.7 4.8-6.8-1.2-7.3-2.8-.1-.3-.1-.4-.1-.2 0-.2-.1-.1-.1.2-.5 1.6-2.6 7.6-7.3 2.8-2.5-2.6-1.4-5.1 3.1-5.9-2.5.4-5.4-.3-6.1-3.2-.2-.8-.6-5.8-.6-6.5 0-3.5 3-2.4 4.8-1z"/></svg>BLUESKY</span>
        <span class="hud-social-handle">@mavrck</span>
      </a>
      <a class="hud-social" href="https://linkedin.com/in/billcondo" target="_blank" rel="noopener">
        <span style="display:inline-flex;align-items:center;gap:10px;"><svg viewBox="0 0 24 24" fill="currentColor"><path d="M20.45 20.45h-3.55v-5.57c0-1.33-.03-3.04-1.85-3.04-1.86 0-2.14 1.45-2.14 2.95v5.66H9.35V9h3.41v1.56h.05c.48-.9 1.64-1.85 3.37-1.85 3.6 0 4.27 2.37 4.27 5.45v6.29zM5.34 7.43a2.06 2.06 0 1 1 0-4.12 2.06 2.06 0 0 1 0 4.12zm1.78 13.02H3.56V9h3.56v11.45zM22.22 0H1.77C.79 0 0 .77 0 1.72v20.56C0 23.23.79 24 1.77 24h20.45c.98 0 1.78-.77 1.78-1.72V1.72C24 .77 23.2 0 22.22 0z"/></svg>LINKEDIN</span>
        <span class="hud-social-handle">billcondo</span>
      </a>
      <a class="hud-social" href="https://instagram.com/mavrck" target="_blank" rel="noopener">
        <span style="display:inline-flex;align-items:center;gap:10px;"><svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2.16c3.2 0 3.58.01 4.85.07 1.17.05 1.8.25 2.23.41.56.22.96.48 1.38.9.42.42.68.82.9 1.38.16.42.36 1.06.41 2.23.06 1.27.07 1.65.07 4.85s-.01 3.58-.07 4.85c-.05 1.17-.25 1.8-.41 2.23-.22.56-.48.96-.9 1.38-.42.42-.82.68-1.38.9-.42.16-1.06.36-2.23.41-1.27.06-1.65.07-4.85.07s-3.58-.01-4.85-.07c-1.17-.05-1.8-.25-2.23-.41a3.7 3.7 0 0 1-1.38-.9 3.7 3.7 0 0 1-.9-1.38c-.16-.42-.36-1.06-.41-2.23-.06-1.27-.07-1.65-.07-4.85s.01-3.58.07-4.85c.05-1.17.25-1.8.41-2.23.22-.56.48-.96.9-1.38.42-.42.82-.68 1.38-.9.42-.16 1.06-.36 2.23-.41 1.27-.06 1.65-.07 4.85-.07M12 0C8.74 0 8.33.01 7.05.07 5.78.13 4.9.33 4.14.63a5.9 5.9 0 0 0-2.13 1.38A5.9 5.9 0 0 0 .63 4.14C.33 4.9.13 5.78.07 7.05.01 8.33 0 8.74 0 12s.01 3.67.07 4.95c.06 1.27.26 2.15.56 2.91.31.79.73 1.46 1.38 2.13.67.65 1.34 1.07 2.13 1.38.76.3 1.64.5 2.91.56C8.33 23.99 8.74 24 12 24s3.67-.01 4.95-.07c1.27-.06 2.15-.26 2.91-.56.79-.31 1.46-.73 2.13-1.38.65-.67 1.07-1.34 1.38-2.13.3-.76.5-1.64.56-2.91.06-1.28.07-1.69.07-4.95s-.01-3.67-.07-4.95c-.06-1.27-.26-2.15-.56-2.91a5.9 5.9 0 0 0-1.38-2.13A5.9 5.9 0 0 0 19.86.63C19.1.33 18.22.13 16.95.07 15.67.01 15.26 0 12 0zm0 5.84A6.16 6.16 0 1 0 12 18.16 6.16 6.16 0 0 0 12 5.84zm0 10.16A4 4 0 1 1 12 8a4 4 0 0 1 0 8zm6.41-11.85a1.44 1.44 0 1 0 0 2.88 1.44 1.44 0 0 0 0-2.88z"/></svg>INSTAGRAM</span>
        <span class="hud-social-handle">@mavrck</span>
      </a>
    </div>
  </div>
</div>

<!-- Overlays -->
<div class="noise"></div>
<div class="vignette"></div>
<div class="scanlines"></div>

<script>
/* Stars */
(function() {
  const n = 140;
  let s = '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1920 1080" preserveAspectRatio="xMidYMid slice">';
  for (let i = 0; i < n; i++) {
    const x = Math.random()*1920;
    const y = Math.random()*680;
    const r = Math.random() < 0.1 ? 1.6 : 0.8;
    const o = 0.3 + Math.random()*0.7;
    s += `<circle cx="${x}" cy="${y}" r="${r}" fill="white" opacity="${o}"/>`;
  }
  s += '</svg>';
  document.getElementById('starLayer').innerHTML = s;
})();

/* Parallax */
let targetX = 0, targetY = 0, curX = 0, curY = 0;
window.addEventListener('mousemove', e => {
  targetX = (e.clientX / window.innerWidth - 0.5);
  targetY = (e.clientY / window.innerHeight - 0.5);
});
(function tick() {
  curX += (targetX - curX) * 0.08;
  curY += (targetY - curY) * 0.08;
  const stars = document.getElementById('starLayer');
  if (stars) stars.style.transform = `translate(${curX * -30}px, ${curY * -20}px)`;
  requestAnimationFrame(tick);
})();

/* Clock */
const startT = Date.now();
setInterval(() => {
  const d = Math.floor((Date.now() - startT) / 1000);
  const hh = String(Math.floor(d/3600)).padStart(2,'0');
  const mm = String(Math.floor((d%3600)/60)).padStart(2,'0');
  const ss = String(d%60).padStart(2,'0');
  document.getElementById('clock').textContent = `T+ ${hh}:${mm}:${ss}`;
}, 1000);
</script>
</body>
</html>
